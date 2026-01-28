## How to Open Image File Through Command Line

Linux allows opening image files
directly from the command line
using graphical or terminal-based tools.

### Using xdg-open (Recommended)
- Opens file with default image viewer

```bash
xdg-open image.png
```

### Using display (ImageMagick)
- Requires ImageMagick package

```bash
dnf install imagemagick -y
display image.jpg
```

### Using eog (GNOME Image Viewer)
- Available on GNOME desktop systems

```bash
eog image.png
```

### Using feh (Lightweight Viewer)
```bash
dnf install feh -y
feh image.jpg
```

### Notes
- Requires a graphical environment
- Not supported on headless servers

### Summary
Command-line tools allow
quick opening of image files
using the system’s default
or specified image viewer.
