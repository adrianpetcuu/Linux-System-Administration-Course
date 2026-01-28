## Download Files or Apps (wget)

The `wget` command is used
to download files and applications
from the internet via the terminal.

### Key Characteristics
- Supports HTTP, HTTPS, and FTP
- Non-interactive download
- Can resume interrupted downloads
- Commonly used on servers

### Download a File
```bash
wget http://example.com/file.zip
```

### Download and Rename File
```bash
wget -O newname.zip http://example.com/file.zip
```

### Resume Download
```bash
wget -c http://example.com/file.zip
```

### Download in Background
```bash
wget -b http://example.com/file.zip
```

### Summary
`wget` is a simple and reliable
tool for downloading files
and applications directly
from the command line.
