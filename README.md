# NextDNS Reinstaller

This is my method to get NextDNS re-installed on my Unifi-OS based consoles such as the UDM, UDR, UDM-Pro, UDM-SE, UDM-Pro-Max, Unifi-Wall after firmware updates.

## Prerequisites

Already have NextDNS installed and configured accordingly.

```  
sh -c 'sh -c "$(curl -sL [https://nextdns.io/install)](https://nextdns.io/install%29)"'  
```

## Installation directions

```  
curl <https://github.com/kb9gxk/unifi-nextdns/raw/main/nextdns-inst> -o /root/nextdns-inst  
chmod +x /root/nextdns-inst  
cp /data/nextdns.conf /root  
```

## After Firmware updates

Just run the command:

```  
/root/nextdns-inst  
```

It will re-run the installer, but you can just hit enter to all the questions as they will be over-written by the saved config in the root folder.
