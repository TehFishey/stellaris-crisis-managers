###################################################################
###################################################################
######														#####
######	The way to make user templates of Crisis Manager	#####
######														#####
###################################################################
###################################################################
#
#####################################################
####  Warning !!: this mod is beta version now!!  ###
#####################################################
#
#	Some of configurations in the templates are invalied now.
#	Information of this is written in web-page of Crisis Manager - End-Game Edition in Steam.
#
#
##############################
####  Version Information  ###
##############################
#
#	this description
#		23/Jun/2018: Items "3.2", "3.3" and "5.1" are updated.
#		 1/Jul/2018: Footnote is updated
#		13/Jul/2018: An item "5.1" is updated.
#		20/Jul/2018: Items "2", "3.1" and footnote are updated.
#		17/Aug/2018: Some of text is fixed.
#		25/Aug/2018: Footnote is deleted: a transition period of this mod is expired. Now all items in the templates are implemented.
#		22/Dec/2018: Items "1" and "5.1" are updated. Information of this mod being beta version is added.
#
#	The templates
#		 2/Jun/2018	Ver.1.0
#			Initial upload.
#		 9/Jun/2018	Ver.1.0d
#			"Crisis at Earliest" surports new values:  EGSY +75, -50, -75, -100
#		23/Jun/2018	Ver.1.1
#			New Parameter: Worn-Out Guardians (Advanced Configurations -> Guardians of Galaxy)
#			The template files are overhauled and old one cannot be applied now.
#		 1/Jul/2018	Ver.1.1c
#			An item is updated: Lifespan of Khan
#			Old template files can be used if updated item is overwritten by new one.
#		 7/Jul/2018	Ver.1.2
#			All items in "Awakening of Sleepers" and "War in Heaven" are updated.
#			Followings are required for using old template in new version of this mod.
#				(1) Copy all items in above 2 groups from new template to old one.
#				(2) Change "1.01" in "@CmtT***_ConstVersionInfo = 1.01" to "1.02".
#				* These configurations for fallen empires are going to be implemented around Jun/15 as "Sleeper Edition".
#		13/Jul/2018	Ver.1.2b
#			Name of an item is updated: "Probability of Crisis Triggered per Elapsed Time" -> "MTTH for Crisis Triggered"
#				-> Old template files can be used without updated.
#		21/Jul/2018	Ver.1.3
#			- New template file is added for "Manual Operation" -> "Create/Delete Fleets for Fallen Empires",
#			- New Parameters: Faster Combat Ships, Faster Constructor (Basic Configuration of End-Game Crisis)
#			- New Parameters: Strength of Ghost Signal (Advanced Configurations -> Contingency)
#			- Followings are required for using old template in new version of this mod.
#				(1) Copy above 2 items from new templates to old ones.
#				(2) Change "1.02" in "@CmtT***_ConstVersionInfo = 1.02" to "1.03".
#				(3) Copy a group "Template for Fleets of Fallen Empires"
#					in "CrisisManagerTemplate_l_<language>.yml" from old file to new one.
#		25/Aug/2018	Ver.1.4
#			- New Parameters: Configurations for L-Gate
#			- Followings are required for using old template in new version of this mod.
#				(1) Copy all items in the group of "Advanced Configurations: L-Gate" from new templates to old ones.
#				(2) Replace following 2 items
#					- "@CmtT***_ConstFleetPower_GrayGoo" -> "@CmtT***_ConstFleetPower_Graygoo"
#					- "@CmtT***_ConstFleetNumber_GrayGoo" -> "@CmtT***_ConstFleetNumber_Graygoo"
#						* "GrayGoo" -> "Graygoo"
#				(3) Change "1.03" in "@CmtT***_ConstVersionInfo = 1.03" to "1.04".
#		 2/Sep/2018	Ver.1.5
#			- New Parameter: Occupy & Purge Planet
#			- New Parameters: 2 parameters for Total War Pack
#			- Followings are required for using old template in new version of this mod.
#				(1) Delele all items "Basic Configurations for End-Game Crisis"
#				(2) Copy all items in the groups of "Event Conditions for End-Game Crises" and "Configurations for Expansion of Crisis Factions" from new templates to old ones.
#				(3) Change "1.04" in "@CmtT***_ConstVersionInfo = 1.04" to "1.05".
#		15/Sep/2018	Ver.1.6
#			- New Parameter: Unstable Portal
#			- Parameters of L-Gate Events Overholed
#			- New Parameters: Crisis Power of L-Gates Empire (Dessanu)
#			- Followings are required for using old template in new version of this mod.
#				(1) Replace all items in "Advanced Configurations: L-Gate" from old template to new one.
#				(2) Copy "Unstable Portal" in "Advanced Configurations: Extradimensionals" from new template and paste it to old one.
#				(3) Copy following 2 items in "Crisis Power" from new template and paste it to old one.
#					- @CmtT***_ConstFleetPower_Dessanu
#					- @CmtT***_ConstCombatFleetNumber_Dessanu
#				(4) Change "1.05" in "@CmtT***_ConstVersionInfo = 1.05" to "1.06".
#		 2/Oct/2018	Ver.1.7
#			- New Parameters: Awakenable Sleepers, Awakenable Ancient Rival
#			- Parameter Updated: Dual Guardians
#			- Followings are required for using old template in new version of this mod.
#				(1) Copy "Awakenable Sleepers" and "Awakenable Ancient Rival" from new template and paste it to old one.
#				(2) Copy "Dual Guardians" from new template and replace old one with new one
#				(3) Change "1.06" in "@CmtT***_ConstVersionInfo = 1.06" to "1.07".
#		27/Oct/2018	Ver.1.8
#			- New Parameters: Less Reinforcements on Anchors Built, Latent Strength of Horde in Adversity
#			- Followings are required for using old template in new version of this mod.
#				(1) Copy above 2 items from new template and paste it to old one.
#				(2) Change "1.07" in "@CmtT***_ConstVersionInfo = 1.07" to "1.08".
#		10/Mar/2019	Ver.1.10
#			- A paratmeter of "Occupy & Purge Planets" is separated to "Occupy Planets" and "Purge Speed"
#			- Followings are required for using old template in new version of this mod.
#				(1) Delete "Occupy & Purge Planets" from old template.
#				(2) Copy above new 2 items from new template and paste it to old one.
#				(3) Change "1.08" or "1.09" in "@CmtT***_ConstVersionInfo = 1.0*" to "1.10".
#
#
#
######################
####  Way to Make  ###
######################
#
#	1. Create empty mod.
#		- It can be created from 'Create Mod' in 'Mod tools' of Stellaris Launcher.
#		- Memorize the directory inputted here.
#		- Recommended to name your mod to be shown at close to Crisis Manager in the Stellaris Launcher.
#
#	2. Copy all folders and files in "CrisisManagerEndGame\For_User_Template"
#		- <folder of Your mod>
#			- common
#				- scripted_variables
#					- Cmt-001_PrimacyTemplate_scripted_variables.txt
#					- Cmt-101_Template-01_scripted_variables.txt
#					- ...
#					- Cmt-116_Template-16_scripted_variables.txt
#					- Cmt-201_TemplateSleeperInitialization_scripted_variables.txt
#			- localisation
#				- <Each language>
#					- CrisisManagerTemplate_l_<language>.yml
#		* Never change names of files nor folders.
#		* Copy all files even if you do not edit all of 17 templates.
#
#	3. Edit template files in "common\scripted effect"
#		3.1. Select files to edit.
#			- Cmt-001_PrimacyTemplate_scripted_variables.txt
#				-> this template is applied automatically on game start.
#			- "Cmt-101_..." ~ "Cmt-116_..."
#				-> These templates are listed up into "Other configuration template"
#			- "Cmt-201_TemplateSleeperInitialization_scripted_variables.txt"
#				-> this is a template for "Manual Operation" -> "Create/Delete Fleets for Fallen Empires",
#				   that control fleet of fallen empires.
#		3.2. Change "@CmtT***_ConstActivated******** = no" to "@CmtT***_ConstActivated******** = yes"
#			- If all of them are "no", this template is ignored.
#		3.3. Edit each options
#			- All parameter is written as "@CmtT***_Const****** = xxx".
#			  You can modify only right side of equals ("xxx").
#			- See also tail of this file. Important footnote is written there.
#		3.4. Edit next files if you want.
#
#	4. Edit localisation files.
#		3.1. Edit "CrisisManagerTemplate_l_<language>.yml"
#
#	5. Edit "<File Name>.mod" file
#		- <File Name> is the directory inputted at '1. Create empty mod.'
#		5.1. Add dependency list.
#			------------------------------------------------
#			dependencies={
#				"Crisis Manager"
#				"Crisis Manager - End-Game Edition"
#				"Crisis Manager - End-Game Edition [BETA]"
#			}
#			------------------------------------------------
#		5.2 Edit any other you want.
#			- Recommended tags: "Balance", "Events", "Overhaul", "Crisis"
#
#	6. Testing: highly recommended to launch Stellaris and check followings.
#		6.1. Check "Other Configuration Templates" in the menu of Crisis Manager.
#			-> Are there all created templates?
#		6.2. Apply each template and check settings from "Configuration Viewer"
#			-> Are no errors shown?
#			-> Are each configurations set as your desires?
#
#	7. Upload to Steam if you want.
#	8. That's all. Enjoy the crisis and/or a breakdown of the galaxy.
#
#
#
