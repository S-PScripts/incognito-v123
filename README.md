# incognito-v123
The incognito exploit is back on v123!

# History:
-> This was found by https://github.com/s0urce-c0de from https://crbug.com/341245382. <br> 
-> https://github.com/s0urce-c0de wrote a writeup on it on 3kh0's repo but it didn't contain all the information. <br> 
-> I (https://github.com/S-PScripts) created a new writeup. <br> 

# Requirements:
-> Access to chrome://flags <br> 
-> Be on chromeOS v123 - v127 <br> 

# Instructions:
## Skip to "Instructions - chromeOS v126-v127" if you're on v126-v127
1. Go to chrome://flags/#captive-portal-popup-window.
2. If it doesn’t exist, make sure to be on chromeOS v123-125. <br> 
   -> If you're on v126-v127, go to the "Instructions - chromeOS v126-v127" section. <br> 
   -> If you're on v128+, you need to downgrade to v123-v127. <br> 
3. Enable it.
4. Restart.
5. If the flag didn’t reset, you can continue. Else you cannot.
6. Go to Settings.
7. Click Wifi in the Network section.
8. Click your wifi.
9. Click Network.
10. Set Name servers to Custom name servers.
11. Set the first box to detectportal.firefox.com OR captive.apple.com OR 150.136.163.0 (yes you can use the v105 dns)
12. A sign in pop up should appear from your wifi. Click Sign in.
13. Do CTRL+T and you're now in Incognito mode!
14. Set Name servers back to what it was before. You will also need to disconnect and reconnect to your wifi.

## Instructions - chromeOS v126-v127:
1. Go to chrome://flags#temporary-unexpire-flags-m124 if you are on v126 <br> 
         chrome://flags/#temporary-unexpire-flags-m125 if you are on v127 (or v126) <br> 
2. Enable it.
3. Restart.
4. Follow the rest of the original instructions.

# Notes:
-> For me, the original method still worked with v126!
-> Extensions can't block you! <br>
-> No search history! <br>

## You can use CAUB to allow changing DNS/Name servers if policies like:

{
   "NetworkConfigurations": [ {
      "GUID": "{<redacted>}",
      "Name": "<redacted>",
      "ProxySettings": {
         "Type": "Direct"
      },
      "Type": "WiFi",
      "WiFi": {
         "AutoConnect": true,
         "HiddenSSID": false,
         "Passphrase": "<redacted>",
         "SSID": "<redacted>",
         "Security": "WPA-PSK"
      }
   } ]
}


# Credits:
https://crbug.com/341245382 for the original post <br>
https://github.com/s0urce-c0de for finding the post, writing the original writeup on 3kh0's repo and adding CAUB to my writeup <br>
https://github.com/S-PScripts (me) for finding a DNS that opens a captive portal window and writing this writeup <br>
https://github.com/Brandon421-ops for reminding me that the temporary unexpire flags exist. <br>
https://github.com/jee1mr/captive-portal because that's where I found the DNS <br>
