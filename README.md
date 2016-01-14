# sublimetext2-aruba
A Sublime Text 2 syntax highlighter for Aruba Networks configs.

I made this highlighter in order to make it easier to glance through configs and find specific sections quickly.  It doesn't catch everything but will grab the vast majority of a config.
This syntax highlighter just shades certain portions of the config to all for easy skimming. For example, all "ip access-list" entries are shaded with one pair of colors and all "interface" entries are a different set of colors.

![screenshot](http://mww012.github.io/sublimetext2-aruba/aruba_config.png)

Installation:
1. Copy the ArubaSyntax folder to the Sublime Text 2 plugin repository on your machine.
	Mac:		Menu Bar: Sublime Text 2 => Preferences => Browse Packages...
				Default Location: /Users/[user]/Library/Application Support/Sublime Text 2/Packages
	Windows:	Menu Bar: Sublime Text 2 => Preferences => Browse Packages...
				C:\Users\\\[user]\AppData\Roaming\Sublime Text 2\Packages

2. Move arubasyntax.sublime-settings to the Packages/User folder.

3. You should now have a functioning syntax highlighter called Aruba Config.  Just change your syntax to Aruba Config

For any edits, you'll need the AAAPackageDev plugin installed.
All coloring is found in the .tmTheme file while the syntax definition are all in the .tmLanguage file.
The .tmTheme file can be edited directly.
The .tmLanguage file should not be edited directly.  It should have a corresponding .YAML-tmLanguage file that is where any edits should be made. Then use AAAPackageDev's Build function to generate the .tmLanguage file that Sublime Text 2 will use.

If anyone has any suggestion on improving this don't hesitate to let me know. :)

For more info, see here(http://docs.sublimetext.info/en/latest/extensibility/syntaxdefs.html).