# System App notes

Different items about the maintenance of the sytems running.
eg. Domotica server, file-server, etc.

## Backup File server

The updates on the file server are not very big. It's mainly used to read content i.s.o. writing.
Therefore manual backup stripts are used for the seperate data folders. 2 seperate harddrives are used
as network storage.

### Local network storage

This is a 4T USB drive to store all personal data

``` bash
rsync -avzh herman@192.168.18.22:/home/herman/media/usb4t/PERSONAL/ /run/media/herman/USB4T/PERSONAL
```

``` bash
rsync -avzh herman@192.168.18.22:/home/herman/media/usb4t/MEDIA/ /run/media/herman/USB4T/MEDIA
```

### Cloud storage

This is a 2T USB drive to store all cloud data. The content is Immich data storing the video's and photo's from
the mobile phones. An external library is installed within Immich to provide access to general photo's

``` bash
rsync -avzh herman@192.168.18.22:/home/herman/media/usb2t/IMMICH /run/media/herman/'My Book'/USB2T/
```

The Synthing folder contains data which is synchronized between the mobile phone's and the network cloud storage

``` bash
rsync -avzh herman@192.168.18.22:/home/herman/media/usb2t/SYNCTHING /run/media/herman/'My Book'/USB2T/
```

The MKDOCS folder contains application notes of various topics.

``` bash
rsync -avzh herman@192.168.18.22:/home/herman/media/usb2t/MKDOCS /run/media/herman/'My Book'/USB2T/
```
