# Docker Selenium Pi

Thanks to [SeleniumHQ/docker-selenium](https://github.com/SeleniumHQ/docker-selenium) for dockerizing of selenium.
Thanks to [kynetiv/docker-selenium-pi](https://github.com/kynetiv/docker-selenium-pi) for porting to ARMv7 architecture.

The current project aims to get StandaloneChrome worked on the Raspberry Pi 4.

## Supported operation systems

It has been tested on:

``` bash
Linux ubuntu 5.3.0-1021-raspi2 #23~18.04.1-Ubuntu SMP Fri Mar 27 16:16:12 UTC 2020 aarch64 aarch64 aarch64 GNU/Linux
```
``` bash
Linux raspberrypi 4.19.97-v7l+ #1294 SMP Thu Jan 30 13:21:14 GMT 2020 armv7l GNU/Linux
```

## Running the images

``` bash
$ docker run -d -p 4444:4444 -v /dev/shm:/dev/shm vladislavzubov/selenium-standalone-chromium-pi
#OR
$ docker run -d -p 4444:4444 --shm-size=2g vladislavzubov/selenium-standalone-chromium-pi
```
