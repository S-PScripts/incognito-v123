# incognito-v123
The incognito exploit is back on v123!

# History:
-> This was found by https://github.com/s0urce-c0de from https://crbug.com/341245382. <br> 
-> https://github.com/s0urce-c0de wrote a writeup on it on 3kh0's repo but it didn't contain all the information. <br> 
-> I (https://github.com/S-PScripts) created a new writeup. <br> 

# Requirements:
-> Access to chrome://flags <br> 
-> Be on chromeOS v123 - v127 (but you can still use 'incognito' on v128+) <br> 

# Instructions:
### IF YOU ARE ON chromeOS v128+, GO TO THE v128+ SECTION!
1. Go to chrome://flags/#captive-portal-popup-window.
2. If it doesn’t exist, make sure to be on chromeOS v123-127. <br> 
   -> If you're on v128+, you need to downgrade to v123-v127 or use the v128+ 'incognito' method. <br> 
3. Enable it.
4. Restart.
5. If the flag didn’t reset, you can continue. Else you cannot.

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
 
# Instructions (v130+):
### THIS WILL ONLY WORK IF YOU HAVE A CAPTIVE PORTAL THAT CAN GET TO GOOGLE. I AM USING EE WIFI IN THE UK.
1. Connect to EE Wifi.
2. A sign in pop up should appear from your Wifi. Click Sign in.
3. CTRL+T is pointless since it now opens a normal tab. You will need to follow the following instructions (and yes, this is the same as the ee-exploit).
4. Accept all cookies.
5. Click Buy Now. You can click any of them.
6. Change your Wifi back.
7. Click the EE icon at the top left of the page. You will be at EE's hotspot home page.
8. Scroll to the bottom. You will see that you can go to the EE STORE. Click Shop now.
9. You will now be at the EE STORE home page. Accept all cookies.
10. Scroll to the bottom and click Privacy policy - this is under the Information header at the right.
11. Click "Please click here to view the BT Privacy Policy."
12. You will now be at BT's privacy policy page. Accept all cookies.
13. Click Contact BT at the bottom of the page - it's at the bottom left.
14. At the bottom of this BT page, click the SMALL Youtube icon - it's at the bottom right.
15. You are now on Youtube! You're very close Click Accept all.
16. In Youtube's sidebar, click Privacy.
17. Scroll to the bottom of Google's privacy page.
18. Click the small Google text.
19. Click Accept Cookies on Google's search page and you have successfully completed this exploit.

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
https://crbug.com/341245382 for the original post <br>
https://github.com/s0urce-c0de for finding the post, writing the original writeup on 3kh0's repo and adding CAUB to my writeup <br>
https://github.com/S-PScripts (me) for finding a DNS that opens a captive portal window and writing this writeup <br>
https://github.com/Brandon421-ops for reminding me that the temporary unexpire flags exist. <br>
https://github.com/jee1mr/captive-portal because that's where I found the DNS <br>
