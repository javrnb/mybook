### Load DO Sku Data

This program imports DO Supply SKU data and DO Sales SKU data files into local server from Linux server 172.17.0.19.

 The downloaded ssd and ssd1 files are unreadable by progress so a script is run to convert those files into json and json1 files.

 The script that converts it is 

```
"php -f /work/apl-pc/scr/convertfiledo.php [dir path] [.ssd/.ssd1] [.json/.json1]"
```

 The script reads these json/json1 files instead of ssd/ssd1 files. The data of json and json1 files are then stored into iskudata table.

 The ssd and ssd1 files are moved to **subfolder"/old"** after successful import.

 The DO Supply SKU data and DO Sales SKU data are stored in iskudata table with ‘SUP’ and ‘SAL’ SKU Data types respectively.

 The message in json or json1 file is combination of ‘message’ and ‘SKU status’ split by ‘-’. The message is stored in iskutmessage field and status is stored in iskutstatus field of iskudata table.

 

