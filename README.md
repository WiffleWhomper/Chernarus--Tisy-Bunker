Custom Structure JSON Files For Console and PC Instructions ONLY WORKS ON DAYZ 1.28 AND LATER!!! NOT EARLIER VERSIONS!!!

Something of a personal passion project that i've always wanted to do; My own version of the Livonia bunker placed within Chernarus. Entirely custom made by myself. Ive put together a layout for the bunker, surrounded it in p3d rocks, added landmarks, a tunnel, nooks, and a narrow pathway around the bunker, all of which offers an entire exploration jsut getting around the outside. 
rather than always having the same items spawn in the same locations every reset, I've created four separate loot files for server owners. This was done in the hopes of offering a more dynamic experience to exploring the bunker, and offering a reason to return for several bunker runs. 
ive also given the TisyBunkerLootSpawns.json as a means of seeing how i've personally created my loot files. 
  -using the apples for coordinates, you can navigate the entirety of the bunker in the DayZ Editor and create your own custom loot files to make an even MORE dynamic experience for your players.
    -- I load the TisyBunker.json, lock all items, import the TisyBunkerLootSpawns.json, then move from the lower sections to the upper sections changing all "apple"s to an item i would prefer be placed there. Once satisfied, i locate the l carefully unlock the TisyBunker items, then delete them. This leaves me with a floating sea of items that can be saved as your newest TisyBunkerLoot file. 
        HAPPY EDITING <3

Limited testing was conducted on Xbox Series S using DayZ Version 1.28 as of June 2025.

Created by @WiffleWhomper. For bug reports or issues, please email WiffleWorkShop@gmail.com with relevant screenshots.

If you'd like to edit any file, simply upload the .DZE/.JSON file into the DayZ Editor.

TERMS OF USE THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Using these modded JSON files and instructions could break the functioning of your DAYZ server, requiring a reinstall that would wipe all player progress.

Using these modded files necessitates increased regular restarts to prevent server crashing.

It is strongly recommended that you thoroughly test your server after applying these files to ensure the proper functioning of your server.

I always recommend validating your files at:

**https://www.xmlvalidation.com/
  https://jsonlint.com/**

Instructions:

1.) Stop Your Server!!

Ensure your server is offline before proceeding.

2.) Activate cfggameplay.json

**Nitrado Console Servers:
Settings >> General >> tick Enable cfggameplay.json.**

For PC Servers, add the following line to your serverDZ.cfg:
enableCfgGameplayFile = 1;
(Note: For some PC servers, including Nitrado, the serverDZ.cfg may be hidden. To access it, enable "Expert Mode" in your settings, then navigate to "Expert Settings" to find serverDZ.cfg. Remember to stop the server before making changes.)


3.) Upload your file:

**Tools >> File Browser >> dayzxb_missions >> dayzOffline.Chernarus >> custom >> "Upload Bunker + All loot fiiles"**
(If a custom folder doesn't exist, create one.)

4.) Call to the custom file using the cfggameplay.json

Tools >> File Browser >> dayzxb_missions >> dayzOffline.Chernarus >> cfggameplay.json

"WorldsData":
	{
		"lightingConfig": 2,
		"objectSpawnersArr": [],
		"environmentMinTemps": [-3, -2, 0, 4, 9, 14, 18, 17, 13, 11, 9, 0],
		"environmentMaxTemps": [3, 5, 7, 14, 19, 24, 26, 25, 18, 14, 10, 5],
		"wetnessWeightModifiers": [1.0, 1.0, 1.33, 1.66, 2.0]
	},
 
Edit the objectSpawnerArr to look like this:

   "objectSpawnersArr": ["custom/TisyBunker.json", "TisyBunkerLoot4.json"]
If you're already calling other custom JSONs to spawn items or buildings, please remember to separate them with commas except for the very last json. i.e.:

"objectSpawnersArr": ["custom/TisyBunker.json", "TisyBunkerLoot4.json", "custom/differentfile.json"],

EXAMPLE OF YOUR NEW FILE

      "WorldsData":
    	{
    		"lightingConfig": 2,
    		"objectSpawnersArr": ["custom/TisyBunker.json", "TisyBunkerLoot4.json", "custom/differentfile.json"],
		    "environmentMinTemps": [-3, -2, 0, 4, 9, 14, 18, 17, 13, 11, 9, 0],
		    "environmentMaxTemps": [3, 5, 7, 14, 19, 24, 26, 25, 18, 14, 10, 5],
		    "wetnessWeightModifiers": [1.0, 1.0, 1.33, 1.66, 2.0]
    	},
5.) SAVE YOUR FILE

6.) Restart your server and the new store will spawn with all items ready for use.

with all the loot files installed, you only need to call to one at a time. When you are ready to change your loot, simply stop your server, go to your cfgameplay.json, and change the number on the TisyBunkerLoot file to which ever you desire. [I change weekly and go in ascending order, restarting at one after i reach 4]

Thanks, and happy gaming! Created by @WiffleWhomper For support or inquiries: WiffleWorkShop@gmail.com
