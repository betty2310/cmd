# Image Magick

1. Resize image 

```bash
convert original.png -resize 100x100 new.png
```

2. To pdf 

> Use to convert filetype like doc, xlxs, ppt to pdf.

**Dependencies**
+ [libreoffice](https://www.libreoffice.org/)

```bash
libreoffice --headless --convert-to pdf *.{docx, xls, ppt}
```
