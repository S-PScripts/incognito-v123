# incognito-v123
The incognito exploit is back on v123!

# History:
-> This was found by https://github.com/s0urce-c0de from https://crbug.com/341245382. <br> 
-> https://github.com/s0urce-c0de wrote a writeup on it on 3kh0's repo but it didn't contain all the information. <br> 
-> I (https://github.com/S-PScripts) created a new writeup. <br> 

-> Option 1 is now on Titanium Network's Oxide Docs! (without credit...) <br>
-> I didn't find the incognito myself, but they could've credited Cohen... <br>

# Requirements:
-> Access to chrome://flags <br> 
-> Be on chromeOS v123 - v127 (but you can still use 'incognito' on v128+) <br> 

# Instructions:
### IF YOU ARE ON chromeOS v126-v127, GO TO THE v126-v127 SECTION!
### IF YOU ARE ON chromeOS v128+, GO TO THE v128+ SECTION!
1. Go to chrome://flags/#captive-portal-popup-window. <br>
   -> If you're on v126-v127, go to the v126-v127 section. <br>
   -> If you're on v128+, you need to downgrade to v123-v127 or use the v128+ 'incognito' method. <br> 
4. Enable it. <br>
5. Restart.
6. If the flag didn’t reset, you can continue. Else you cannot.

Now, follow one of the two methods:

## Option 1:
1. Go to Settings.
2. Click Wifi in the Network section.
3. Click your wifi.
4. Click Network.
5. Set Name servers to Custom name servers.
6. Set the first box to detectportal.firefox.com OR captive.apple.com OR 150.136.163.0 (yes you can use the v105 dns)
7. A sign in pop up should appear from your wifi. Click Sign in.
8. Do CTRL+T and you're now in Incognito mode! <br>
   -> You can also right click the top of the tab then click "Show as tab" to open Incognito. <br>
9. Set Name servers back to what it was before. You will also need to disconnect and reconnect to your wifi. <br>

## Option 2:
1. If you have access to EE Wifi in the UK, connect to it.
2. A sign in pop up should appear from your WiFi. Click Sign in.
3. Do CTRL+T and you're now in Incognito mode! <br>
4. Reconnect to your normal Wifi. <br>
 -> You can also right click the top of the tab then click "Show as tab" to open Incognito. <br>

# Instructions (v127-v128):
1. Go to:
   -> chrome://flags#temporary-unexpire-flags-m124 if you are on v126 <br>
   -> chrome://flags/#temporary-unexpire-flags-m125 if you are on v127 (or v126) <br>
3. Enable it. <br>
4. Restart.
5. Follow the rest of the original instructions.

# Instructions (v128):
Please go to https://s-pscripts.github.io/incognito-v128/ 

# Notes:
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
https://crbug.com/341245382 (cohen) for the original post <br>
https://github.com/s0urce-c0de for finding the post, writing the original writeup on 3kh0's repo and adding CAUB to my writeup <br>
https://github.com/S-PScripts (me) for finding a DNS that opens a captive portal window and writing this writeup <br>
https://github.com/Brandon421-ops for reminding me that the temporary unexpire flags exist. <br>
https://github.com/jee1mr/captive-portal because that's where I found the DNS <br>
