Flappy Pig
====================
<br/>
<p align="center">
    <a href="https://sulu.io/" target="_blank">
        <img width="250px" src="https://github.com/gianmarcopicarella/virgo/blob/master/virgo_rounded_logo.png?raw=true" alt="Sulu logo">
    </a>
</p>

<br/>
<p align="center">
    <a href="https://github.com/gianmarcopicarella/flappy-pig/blob/master/LICENSE" target="_blank">
        <img src="https://img.shields.io/github/license/gianmarcopicarella/flappy-pig.svg" alt="GitHub license">
    </a>
    <a href="https://github.com/gianmarcopicarella/flappy-pig/releases" target="_blank">
        <img src="https://img.shields.io/github/tag/gianmarcopicarella/flappy-pig.svg" alt="GitHub tag (latest SemVer)">
    </a>
    <a href="https://github.com/gianmarcopicarella/flappy-pig/graphs/contributors" target="_blank">
        <img src="https://img.shields.io/github/contributors-anon/gianmarcopicarella/flappy-pig.svg" alt="GitHub contributors">
    </a>
</p>
<br/>

[Flappy pig](https://github.com/gianmarcopicarella/flappy-pig) is an **Arduino Uno hyper casual game**. It has been developed as a side project during the university class "Arduino and multicore programming" at [Sapienza](https://www.uniroma1.it/en/pagina-strutturale/home). It uses [U8g2](https://github.com/olikraus/u8g2) to communicate, via the SPI protocol, directly to the screen hardware without worring about low level details.

<img src="https://github.com/gianmarcopicarella/flappy-pig/blob/master/flappy_pig.gif?raw=true" max-width="350px !important" />


### Features:
* 8bit sound effects when the player dies or earns a point
* Easy to use controls
* 14fps on average with a clock speed of 16mhz, 2kb of sram and a 1.5inch oled screen
* Compatible with every monochrome SPI Arduino display
* Make-take move functions supplied with a simple Chessboard object

## Contributing
Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contribution you make to Flappy pig is **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
Flappy-pig is released under the under terms of the [MIT License](LICENSE).
