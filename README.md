_*How to setup a Raspberry Pi with kiwix to serve Wikipedia LAN-wide*_
----
- download the content (e.g. **English Wikipedia** `zim` file: `wikipedia_en_all_maxi_2021-12.zim`) from [here](https://wiki.kiwix.org/wiki/Content_in_all_languages)
- download the server: `kiwix-tools_linux-armhf-2022-01-06.tar.gz` from [here](https://download.kiwix.org/nightly/2022-01-06/)
  - extract/create dir structure below, as described [here](https://chrischapman.co/projects/wikipi.html), oh actually.. most of these notes were derived from that page!
```
pi@goldenchild:/media/pi/d5e76c06-5d89-420a-acd6-2fa7fff2edde/kiwix $ tree .
├── bin
│   ├── kiwix-manage
│   ├── kiwix-read
│   ├── kiwix-search
│   └── kiwix-serve
└── wikipedia_en_all_maxi_2021-12.zim
```
- run it, yeah search magically works too:
```
pi@goldenchild:/media/pi/d5e76c06-5d89-420a-acd6-2fa7fff2edde/kiwix $ sudo bin/kiwix-serve wikipedia_en_all_maxi_2021-12.zim &
The Kiwix server is running and can be accessed in the local network at: http://192.168.0.123:80
```

