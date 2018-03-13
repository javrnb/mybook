### Import DO SKU Data

Import DO SKU Data checks for tokens for supply and sales sku data from the API

```
-If token is already available then it uses the token but if token is not available then it fetches new one.
```

-Next it gets the ping response, if ping is unauthorized then it fetches new token but if ping is authorized then it downloads Supply SKU Data and Sales SKU Data from DO API to PF new Linux server 172.17.0.19 with .ssd and .ssd1 extension.

![](file:///C:\Users\nbarnwal\AppData\Local\Temp\msohtmlclip1\01\clip_image002.jpg)

Fig:Import DO SKU Data

To establish authorized secured connection we need to give App Name and App Key which are username and password. Based on that information we successfully generate token.

The ssd and ssd1 files contain JSON data with the information about Supply SKU Data and Sales SKU Data respectively.

The ssd and ssd1 files which are received from DMD are stored in Server 172.17.0.19 at path provided below:

```
"/work/edi/[dbname]/STARGATE.OUT/"
```



