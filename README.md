# incognito-v124
The incognito exploit is back on v124!

## Instructions:
1. Go to chrome://flags/#captive-portal-popup-window.
2. If it doesn't exist, make sure to update chromeOS to the latest version.
3. Enable it.
4. Restart.
5. If the flag didn't reset, you can continue. Else you cannot.
6. Go to Settings.
7. Click Wifi in the Network section.
8. Click your wifi.
9. Click Network.
10. Set Name servers to Custom name servers.
11. Set the first box to detectportal.firefox.com.
12. A sign in pop up should appear from your wifi. Click Sign in.
13. Do CTRL+T - YOU'RE NOW IN INCOGNITO MODE!
14. Set Name servers back to what it was before.

## Notes:
-> Extensions can't block you!
-> No search history!

## Credits:
https://crbug.com/341245382
https://github.com/s0urce-c0de for finding the post

## Weird thing: (you can ignore this)
I did this exploit and I noticed when I checked my windows that the OLD sign in window exploit thing was there (v105). I had tried using its DNS to get a captive window but it didn't work since it was down. But apparently not. What was weird was that I hadn't even got a sign in pop up. I got one when I used the firefox one, but that opened a different captive tab. That tab wasn't there, so maybe the two DNS merged?
