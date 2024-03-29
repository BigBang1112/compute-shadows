## What is the point of this title pack?
Whenever you want to recalculate map shadows from the old versions of ManiaPlanet, or convert Stadium tracks from older Trackmania games, this title pack can do this easily in bulk.

## What is a MapType?
It's a special script that tells you if the map is correctly build. Maps that don't accept the requirements are forbidden by the game to use in singleplayer or multiplayer.

## Why even MapType?
This feature was made especially to correctly convert TM1's Platform, Stunt and Puzzle maps to ManiaPlanet, but it can be used in many other ways of course. For example making maps playable if their MapType is lost etc.

## How to use the tool?
First things first, you need to specify the folder where your maps are, relative to Maps/. You can leave it empty to calculate shadows for all maps you have. Next, you can additionally specify MapType which will apply to the calculated maps, or turn this feature off by the little tick button in the top corner. Then you're ready to go by clicking Compute them all.
To terminate the tool, click on the Terminate button in the menu. You have 2 seconds to click on it before another calculation starts. If you're in a calculation process, you can simply click the Back button here (nothing will break by that) and you will be returned to menu to click Terminate. **Note: Shadows will be uncalculated but MapType will still change.**

## What are the exact problems of turning off the saving of already computed maps?
Previous map file containing calculated shadows can sometimes be replaced with one having no shadows, which could make things even longer than manual work for the user. However, turning this off makes the tool usable for mass MapType changing or things like these. Still, I recommend doing a map backup in this case.
For 100% safety, keep this turned on.

## How is this better than /calculateallshadows?
You're right, /calculateallshadows does a thing, but you have no control or idea what's being calculated.
Before, you also could replicate the same functionality of this title pack with few more commands, but since MP4.1, most of these commands broke.

## I've noticed that the map shadows aren't calculated on High, but Default. Why is that?
This was done due to technical reasons.
If you calculate shadows on higher than Default, the lightmaps aren't saved to the map file, but only to your cache, meaning other people won't see the shadows calculated.
If you want to calculate shadows to highest, I recommend doing it separately only to maps where you really need them.

## My maps use different MapType than Race. What should I do to keep the original MapType for all the maps?
In the MapType step of the tool, click on the little tick button in the top corner. This will turn off the feature. Clicking again will turn the feature on.

## I converted a Stadium map from TM1, but several blocks suddenly disappeared. Why?
I'm not exactly sure either, but I consider this as a ManiaPlanet engine bug, happening especially with sculptures. Same thing would happen if you convert the map manually.
Currently, I'm trying to find a solution for this. For now, you have no other option than to place them manually.

## I minimized the game, but moved nowhere in the calculation when I checked. Why it just stopped?
When you click on the minimize button at the top, all of the scripts that do the calculation freeze. You have to Alt+Tab or switch from the game without actual minimalization.

## After calculation, the map sizes are very small, nice! It that alright though?
No, it actually is not. The shadows weren't saved to the map file. This usually happens when the maps were already calculated in the past. Check your cache in ProgramData/ManiaPlanet/Cache and remove the lightmap files (.Bump.LightMap.zip). They should be one of the newest. If you're not sure, you can clear the whole cache in ManiaPlanet settings, which will do just fine.