# Bash Graphics Rendering

Simple Image renderer using calculations to output raw bytes into a .bmp file to create bitmaps.

## Functionality

The most important logic lives in lib/bash-bmp
- It calculates filesize
- formats bytes in the right order

It is the backbone of this whole project as without it you would just calculate for nothing.

In /src you will find 3 examples
- simple-bmp 
    creates a 2 by 2 bitmaps, this is a quick showcase of the functions in bash-bmp, and how to generate a bitmap file
- gradient-bmp
    the first complex example and also the one with a real use case you can basically use it to generate a gradient (for presentations or whatever)
- sprite-to-bmp
    this is the most powerful of all you can take any asci art and turn it into pixel art, by transforming it into a bitmaps there are assets provided in /assets so you can test it 

## Project start

I started this project on a journey to find out what is possible with pure bash and I came to the conclusion that pretty much everything is possible with bash, another example is the [http server](https://github.com/Amir-jpg-png/pure-bash-http-server) built in bash if you want to check that out. 

## Installation and Usage

To install it you can copy this github repo

```bash
git clone https://github.com/Amir-jpg-png/pure-bash-http-server.git
```

To use these programs you just need to make them executable and execute them. 

sprite-to-bmp is a bit more tricky in the directory where your sprite-to-bmp script is execute

```bash
/path/to/asciArt.txt | ./sprite-to-bmp -p /path/to/pallete.txt /path/to/desired/output.bmp
```

## Other

Feel free to fork this repo and create different use cases.
