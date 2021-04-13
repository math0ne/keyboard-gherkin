## gherkin keyboard firmware
![layout](https://raw.githubusercontent.com/openist/keyboard-gherkin/master/keyboard-layout.png)

You can see my layout here: http://www.keyboard-layout-editor.com/#/gists/5dec436256c0d150b6f5e854bc4c8429

I ran these commands in ubuntu bash for windows which seems to work great but will also work in cygwin or any linux distro.

* How to flash:

```
apt-get install gcc-avr binutils-avr gdb-avr avr-libc avrdude
git clone https://github.com/openist/keyboard-gherkin.git
cd keyboard-gherkin
make
```

* Copy your .hex file to somewhere you can easily access it on your windows machine.
* Download Xloader: http://russemotto.com/xloader/
* Connect your pro micro via usb, you should hear the device connected sound, if you do not you may not be using a proper data micro usb cable.
* Reset the pro micro twice to enter bootloader mode.
* Within 8 seconds load the hex file into xloader and press upload.

Original Creator: https://www.40percent.club/

Originally forked from: https://github.com/di0ib/

Gerber files released under https://creativecommons.org/licenses/by-sa/4.0/

![Creative Commons Attribution-ShareAlike 4.0 International License](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)
