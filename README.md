# Scanner

Rapidly turn your stack of notes into multi-page PDFs.


Usage:

```
py scan.py -h                   
usage: scan.py [-h] [--capture_device_id CAPTURE_DEVICE_ID] [--storage_path STORAGE_PATH] [--list_capture_devices]

Capture and store document scans

optional arguments:
  -h, --help            show this help message and exit
  --capture_device_id CAPTURE_DEVICE_ID
                        The ID of the capture device to scan with
  --storage_path STORAGE_PATH
                        The final storage location of the scanned PDF
  --list_capture_devices
                        List all working capture devices
```

Start off by identifying your capture devices:

```
py scan.py --list_capture_devices
# outputs: Working capture devices = [0,1,2]
```

And then start the scan workflow:

```
py scan.py --capture_device_id 2 --storage_path "c:\users\Developer\Work Scans"
```

1. Press [SPACE] to scan each page
2. Press [ESC] to indicate the end the document
3. Type a filename
4. Get the full file path to the multi-page PDF copied to your clipboard
