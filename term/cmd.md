1. Resize image 

> Resize image directly use `imagemagick` tool.

```bash
$ convert original.png -resize 100x100 new.png
```

2. To pdf 

> Use to convert filetype like doc, xlxs, ppt to pdf.

*Dependencies*
+ [libreoffice](https://www.libreoffice.org/)

```bash
$ libreoffice --headless --convert-to pdf *.{docx, xls, ppt}
```

3. View log use `journalctl`

> u know, can't find postgres's log file :v, show if u need to see this, you can try used `journalctl`

```bash
$ journalctl -u postgresql --since "600 min ago"
```

4. Reload coreaudio Hackintosh

> Sometime when sleep and wake up, sound of my hackintosh laptop is so weird. Y should reload sound card:

```bash
$ ps aux | grep 'coreaudio[d]' | awk '{print $2}' | xargs sudo kill
```
or 
```bash
$ sudo killall coreaudiod
```

