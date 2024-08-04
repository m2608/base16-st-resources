# base16-st-resources

[Base16](http://chriskempson.com/projects/base16/) themes template for [st](https://st.suckless.org/) [xresources](https://st.suckless.org/patches/xresources-with-reload-signal/) patch.

## How to use

* Generate a set of color themes in `xresources` format. Probably you could use any base16 theme generator, I've only tested [mine](https://gist.github.com/m2608/48185612f371a7a0803ad1c329e59933).
* Merge some theme with `xrdb -merge /path/to/theme/file`.
* Reload resources for `st` by sending `USR1` signal:
  * Linux: `pkill -USR1 -x st`
  * FreeBSD: `pkill -SIGUSR1 -ax st`
* To load specific theme at boot, put it into `~/.Xresources` file.
