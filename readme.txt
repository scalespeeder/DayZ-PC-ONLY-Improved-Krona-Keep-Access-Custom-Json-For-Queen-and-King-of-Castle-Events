DayZ Chernarus "Improvements To Access Of The Top Of The Keep At Krona Castle" Custom Structure Json File For PC Instructions & Terms Of Use

*******************************************************

PLEASE NOTE THAT THIS CUSTOM OBJECT SPAWNER WILL NOT WORK WITHOUT THE BRIDGES MOD BEING INSTALLED ON YOUR SERVER!!!

BRIDGES MOD ON STEAM: https://steamcommunity.com/workshop/filedetails/?id=2070603516

MANY THANKS TO [Lusk]-hlynge FOR THIS GREAT BRIDGES MOD!

*******************************************************

Spawns extra ways to get to the top of the Keep at Krona Castle ( 1412.38 / 9207.20 ) including rope bridges, external stairs and a high-wire, on Chernarus.

These extra access points have been added to ballance the endgame of Queen / King of the Castle events, where the ultimate aim to win is to
hold the top of the Keep at Krona Castle when the timer runs out. The extra access points take away some of the advantage that a team gets by
going to and holding the keep early - attackers now have four ways to try and breach and take the keep, rather than one.

Limited Testing on PC Chernarus Local Server DAYZ Version 1.19 JAN 2023.

Created by @scalespeeder. Please report bugs & errors to scalespeeder@gmail.com with screenshots.

If you'd like to edit & customize the file, simply load "kronabridgesandstairsforeditor.dze" into DayZ Editor.

Many Thanks To Inclement Dab for his amazing DayZ Editor that makes this all possible: https://steamcommunity.com/sharedfiles/filedetails/?id=2250764298

TERMS OF USE
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN
AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH
THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Using these modded json files and instructions could break the functioning of your DAYZ server, requiring a reinstall that would wipe
all player progress.

Using these modded files neccessitates increased regular restarts to prevent server crashing.

It is suggested you thoroughly test your server after applying these files to ensure proper
functioning of your server.

I always recomend you validate your files at: https://www.xmlvalidation.com/ and https://jsonformatter.curiousconcept.com/

Instructions:

Subscribe to BRIDGES MOD on Steam:

https://steamcommunity.com/workshop/filedetails/?id=2070603516

Start your DayZ Launcher to download the mod files. Using your FTP programme, copy the @Bridges folder from your DayZ !workshop folder
to the root directory of your server. Copy the key from the mods key folder to your servers key folder. Edit your start batch file,
so that your server will load @Bridges mod on startup. (On Nitrado and some other DayZ Server Providers you don't have access to the batch file,
instead you will find an "Additional mods" setting in the settings section of your servers web interface, add @Bridges there.)

Click the "Code" button and "Download Zip" on the Github Repository and extract the files on your local PC for access.

Stop your server.

Ensure your DayZ Server has activated the cfggameplay.json. For console users on Nitrado Servers, go to "General Settings" on your server and tick "Enable cfggameplay.json".

On PC Servers add the following line to your serverDZ.cfg:

enableCfgGameplayFile = 1;

(On some PC servers, including Nitrado, the serverDZ.cfg is "hidden", so you need to enable "expert mode" in settings,
then go to "expert settings", which is the serverDZ.cfg. Stop the server before making changes this way.)

Upload "kronacastlebridgesandstairs.json" from the extracted files to inside the "custom" folder of the mission directory on your server.
(If you haven't got a "custom" folder, create one.)

Open the cfggameplay.json file in the correct mission file for your server and look for the "objectSpawnersArr" line.

This file tells your server to access your custom file.

Edit it to look like this: 

	"objectSpawnersArr": ["custom/kronacastlebridgesandstairs.json"],	
	
If you already are calling custom jsons to spawn items or buildings, seperate the files like this:

	"objectSpawnersArr": ["custom/kronacastlebridgesandstairs.json","custom/anotherfile.json","custom/differentfile.json"],
	
Save your changes & upload if you need to.

Restart your server and the new objects will appear immediatly.

Thanks, Rob.
