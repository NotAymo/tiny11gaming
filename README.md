# tiny11gaming
Tiny11 but with Xbox Services (originally made by NTDEV but rebuilt by Aymo)
 



If you ever installed Tiny11, you saw that there is no Xbox Services to play your games with an Microsoft account, so, Tiny11 Gaming will fix this !

Instructions:

Download Windows 11 22621.1265 from UUPDump or 22621.525 or 25300 from the Microsoft website (https://www.microsoft.com/software-download/windows11)
Mount the downloaded ISO image using Windows Explorer.
For .1265, run tiny11 creator.bat as administrator. For .525 or 25300, use the aptly-named script (also as administrator).
Select the drive letter where the image is mounted (only the letter, no colon (:))
Select the SKU that you want the image to be based.
Sit back and relax :)
When the image is completed, you will see it in the folder where the script was extracted, with the name tiny11.iso

What is removed and not :
Clipchamp, News, Weather, GetHelp, GetStarted, Office Hub, Solitaire, PeopleApp, PowerAutomate, ToDo, Alarms, Mail and Calendar, Feedback Hub, Maps, Sound Recorder, Media Player, QuickAssist, Internet Explorer, LA57 support, OCR for en-us, Speech support, TTS for en-us, Media Player Legacy, Tablet PC Math, Wallpapers, Edge*, OneDrive

Xbox and Your Phone is not removed*

(*= For installing a web browser in a new fresh install, do : 

Press WINDOWS KEY + R > powershell > then paste this code into powershell : 
$LocalTempDir = $env:TEMP; $ChromeInstaller = "ChromeInstaller.exe"; (new-object System.Net.WebClient).DownloadFile('http://dl.google.com/chrome/install/375.126/chrome_installer.exe', "$LocalTempDir\$ChromeInstaller"); & "$LocalTempDir\$ChromeInstaller" /silent /install; $Process2Monitor = "ChromeInstaller"; Do { $ProcessesFound = Get-Process | ?{$Process2Monitor -contains $_.Name} | Select-Object -ExpandProperty Name; If ($ProcessesFound) { "Still running: $($ProcessesFound -join ', ')" | Write-Host; Start-Sleep -Seconds 2 } else { rm "$LocalTempDir\$ChromeInstaller" -ErrorAction SilentlyContinue -Verbose } } Until (!$ProcessesFound)
And finished, you successfully installed Google Chrome on your computer using powershell)

(**= Why Your Phone is not removed?
     Beacause if Your Phone is deleted, others Xbox services won't work cause of the phone sync)



