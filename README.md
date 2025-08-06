# Constant Enchant Level Scaling

# Brief Overview
*  Automatically scales the constant effect offset GameSetting with the players Level.

# Changelog
1.0 
* Initial Release

1.1
* Added scaling for the gold cost of enchantments

1.2
* Rewrote Script to run more efficiently
* Added Display Current Settings and Refresh Settings CommandButtons to the menu.

## Description
![Constant Effect](/image/Level_45_Constant.png "Grand Constant Effect")

* Includes MCM Functionality to customize the scaling factor.
	
### Compatibility

* This mod's changes will take priority if using another MCM (Like my [Comprehensive GameSettings MCM](https://www.nexusmods.com/oblivionremastered/mods/4948) that changes the same GameSettings that this does. This mod changes these GameSettings using Console Command whenever the player levels up, and whenever the multiplier is changed in the attached MCM, so any manual changes you've made to the settings will be overwritten by that mechanism. 
* Basically incompatible with any esp that modifies the same GameSettings since the Console Commands will overwrite those values immediately. 

### Prerequisites
1. [UE4SS](https://www.nexusmods.com/oblivionremastered/mods/32)
	1. [Mad OBScript Extender v2.0a or Later](https://www.nexusmods.com/oblivionremastered/mods/4819)
	2. [Mad Config Menu MCM](https://www.nexusmods.com/oblivionremastered/mods/4810)
2. [OBSE](https://www.nexusmods.com/oblivionremastered/mods/282)
	1. [NL-Tag Remover](https://www.nexusmods.com/oblivionremastered/mods/473)
	
### Installation
0. Install Prerequisites
1. Copy Constant_Effect_Scaling.esp to `\Oblivion Remastered\OblivionRemastered\Content\Dev\ObvData\Data`
	1. Add `Constant_Effect_Scaling.esp` to your Plugins.txt
2. Copy Constant_Effect_Scaling_MCM.ini to `\Oblivion Remastered\OblivionRemastered\Binaries\Win64\MadConfigs`

### Uninstallation
0. This mod alters Game Settings. If you need to uninstall this, do the following after the plugin is removed.
	1. While In-game, press the ~ key to open the console, type `SetGameSetting fMagicCEEnchantMagOffset 5` and press enter.
	
### Compatibility
0. Mods that manually set GameSettings seemingly will overwrite anything set by console command
1. This also seemingly applies to Settings set by [GameSettings Loader](https://www.nexusmods.com/oblivionremastered/mods/746) ini files.

## Credits
1. Utilizes ObScript Extender created by [MadAborModding](https://next.nexusmods.com/profile/MadAborModding)
2. Utilizes MCM created by [MadAborModding](https://next.nexusmods.com/profile/MadAborModding)