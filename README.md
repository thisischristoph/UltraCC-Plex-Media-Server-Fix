# UltraCC-Plex-Media-Server-Fix

If you use Plex Media Server on UltraCC, reset your password, and signed everyone out, you'll have broken the connection to plex and won't be able to claim the media server using the UltraCC link.

There's a few other fixes around and this is mostly the same, but the base URL is normally wrong on other scripts. It's different on UltraCC for some reason.



First SSH into your server using the command:

`ssh username@hostname`

> You'll be prompted for your password, this in the FTP/SSH Credentials in the console



Now, input the following commands separately

`wget https://raw.githubusercontent.com/thisischristoph/UltraCC-Plex-Media-Server-Fix/main/reclaim.sh`

Then 

`bash reclaim.sh`

> You'll be prompted for your claim code, navigate to https://www.plex.tv/claim/ and get the new claim code


Now restart Plex Media Server in the Apps tab in the console and it should be back and connected after it restarts 
