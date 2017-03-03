# tiny-bootstrap

This is a tiny, fully working "bootloader" for x86 IBM-PC computers, which basically does nothing more than print some text to the screen. Mostly a teaching tool. Full writeup is available [on my blog](http://www.joebergeron.io/posts/post_two.html). If you just want to see it in action though, just run

     bochs -f bochsrc.txt

which runs bochs with the correct config file.



# 我的修改

## install
sudo apt-get install bochs   
sudo apt-get install bochs-sdl

## edit bochsrc.txt
```
megs: 32
romimage: file=/usr/share/bochs/BIOS-bochs-latest, address=0xfffe0000
vgaromimage: file=/usr/share/bochs/VGABIOS-lgpl-latest
floppya: 1_44=boot.com, status=inserted
boot: a
log: bochsout.txt
mouse: enabled=0
display_library: sdl
```
