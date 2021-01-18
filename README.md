Flappy Pig
====================
<br/>
<p align="center">
  <img width="300" src="https://github.com/gianmarcopicarella/flappy-pig/blob/master/flappy_pig.gif?raw=true">
</p>
<br/>

[Flappy pig](https://github.com/gianmarcopicarella/flappy-pig) is an **Arduino Uno hyper casual game**. It has been developed as a side project during the university class "Arduino and multicore programming" at [Sapienza](https://www.uniroma1.it/en/pagina-strutturale/home). It uses [U8g2](https://github.com/olikraus/u8g2) to communicate, via the SPI protocol, directly to the screen hardware without worring about low level details.

## Usage
Download the progetto.ino file and install the latest U8g2 library version. Add the following lines inside these library files.
```c++
// inside U8g2lib.h right after nextPage definition
void customPage(uint8_t page) { u8g2_customPage(&u8g2, page); }

// inside u8g2.h right after u8g2_NextPage declaration
void u8g2_customPage(u8g2_t *u8g2, uint8_t page);

// inside u8g2_buffer.c right after u8g2_NextPage definition
void u8g2_customPage(u8g2_t *u8g2, uint8_t page) {
  if ( u8g2->is_auto_page_clear )
  {
    u8g2_ClearBuffer(u8g2);
  }
  u8g2_SetBufferCurrTileRow(u8g2, page);
}
```
You can now compile and try the game!

### Features:
* 8bit sound effects when the player dies or earns a point
* Easy to use controls
* 14fps on average with a clock speed of 16mhz, 2kb of sram and a 1.5inch oled screen
* Compatible with every monochrome SPI Arduino display

## Contributing
Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contribution you make to Flappy pig is **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
Flappy-pig is released under the under terms of the [MIT License](LICENSE).
