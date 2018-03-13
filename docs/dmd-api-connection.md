# DMD API CONNECTION:

DMD API Connection checks for tokens from the API

-If token is already available then it uses the token but if token is not available then it fetches new one.

-Next it gets the ping response, if ping is unauthorized then it fetches new token but if ping is authorized then it downloads DO Order Proposal Headers from DO API to PF new Linux server 172.17.0.19 with .sgh1 extension.

![](/assets/Untitled.png)Fig: DMD API Connection

To establish authorized secure connection we need to give App Name and App Key which are username and password. Based on that information we successfully generate token.

The sgh1 file which are received from DMD are stored in

```
"/work/edi/[dbname]/STARGATE.OUT/"
```

** **The sgh1 file contains JSON data with the information about order proposal header number, sku data and state.

