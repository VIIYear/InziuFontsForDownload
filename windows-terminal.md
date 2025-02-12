```json
// This file was initially generated by Windows Terminal 1.3.2651.0
// It should still be usable in newer versions, but newer versions might have additional
// settings, help text, or changes that you will not see unless you clear this file
// and let us generate a new one for you.

// To view the default settings, hold "alt" while clicking on the "Settings" button.
// For documentation on these settings, see: https://aka.ms/terminal-documentation
{
    "$schema": "https://aka.ms/terminal-profiles-schema",

    "defaultProfile": "{e305623a-ba58-401e-b0af-6654477dfa67}",

    // You can add more global application settings here.
    // To learn more about global settings, visit https://aka.ms/terminal-global-settings

    // If enabled, selections are automatically copied to your clipboard.
    "copyOnSelect": false,

    // If enabled, formatted data is also copied to your clipboard
    "copyFormatting": false,

    // A profile specifies a command to execute paired with information about how it should look and feel.
    // Each one of them will appear in the 'New Tab' dropdown,
    //   and can be invoked from the commandline with `wt.exe -p xxx`
    // To learn more about profiles, visit https://aka.ms/terminal-profile-settings
    "profiles":
    {
        "defaults":
        {
            // Put settings here that you want to apply to all profiles.
            "useAcrylic":true,
            "acrylicOpacity": 0.75,
            "historySize": 9001,
            "fontFace": "Sarasa Term Slab SC",
            "startingDirectory": "D:\\",
            "colorScheme": "BlulocoLight",
            "backgroundImageOpacity": 0.2,
            "backgroundImage": "D:\\Picture\\miku.png",
            "backgroundImageAlignment": "bottomRight",
            "backgroundImageStretchMode": "uniform",
            "cursorColor":"#6d1bed"
        },
        "list":
        [
            {
                // Make changes here to the powershell.exe profile.
                "guid": "{61c54bbd-c2c6-5271-96e7-009a87ff44bf}",
                "name": "Windows PowerShell",
                "commandline": "powershell.exe",
                "hidden": false
            },
            {
                // Make changes here to the cmd.exe profile.
                "guid": "{0caa0dad-35be-5f56-a8ff-afceeeaa6101}",
                "name": "命令提示符",
                "commandline": "cmd.exe",
                "hidden": false
            },
            {
                "guid": "{b453ae62-4e3d-5e58-b989-0a998ec441b8}",
                "hidden": false,
                "name": "Azure Cloud Shell",
                "source": "Windows.Terminal.Azure"
            },
            {
                "guid": "{e305623a-ba58-401e-b0af-6654477dfa67}",
                "name": "Git Bash",
                "commandline": "C:\\Program Files\\Git\\bin\\bash.exe -i -l",
                "icon": "C:\\Program Files\\Git\\mingw64\\share\\git\\git-for-windows.ico",
                "closeOnExit": "always",
            }
        ]
    },

    // Add custom color schemes to this array.
    // To learn more about color schemes, visit https://aka.ms/terminal-color-schemes
    "schemes": [
          {
            "name": "BlulocoLight",
            "black": "#cbccd5",
            "red": "#c90e42",
            "green": "#21883a",
            "yellow": "#d54d17",
            "blue": "#1e44dd",
            "purple": "#6d1bed",
            "cyan": "#1f4d7a",
            "white": "#000000",
            "brightBlack": "#dedfe8",
            "brightRed": "#fc4a6d",
            "brightGreen": "#34b354",
            "brightYellow": "#b89427",
            "brightBlue": "#1085d9",
            "brightPurple": "#c00db3",
            "brightCyan": "#5b80ad",
            "brightWhite": "#1d1d22",
            "background": "#f7f7f7",
            "foreground": "#2a2c33"
          },
          {
            "name": "BlulocoDark",
            "black": "#4a505d",
            "red": "#f81141",
            "green": "#23974a",
            "yellow": "#fd7e57",
            "blue": "#285bff",
            "purple": "#8c62fd",
            "cyan": "#366f9a",
            "white": "#ccd5e5",
            "brightBlack": "#61697a",
            "brightRed": "#fc4a6d",
            "brightGreen": "#37bd58",
            "brightYellow": "#f6be48",
            "brightBlue": "#199ffd",
            "brightPurple": "#fc58f6",
            "brightCyan": "#50acae",
            "brightWhite": "#ffffff",
            "background": "#1e2127",
            "foreground": "#abb2bf"
          },
          {
            "name": "Adventure",
            "black": "#040404",
            "red": "#d84a33",
            "green": "#5da602",
            "yellow": "#eebb6e",
            "blue": "#417ab3",
            "purple": "#e5c499",
            "cyan": "#bdcfe5",
            "white": "#dbded8",
            "brightBlack": "#685656",
            "brightRed": "#d76b42",
            "brightGreen": "#99b52c",
            "brightYellow": "#ffb670",
            "brightBlue": "#97d7ef",
            "brightPurple": "#aa7900",
            "brightCyan": "#bdcfe5",
            "brightWhite": "#e4d5c7",
            "background": "#040404",
            "foreground": "#feffff"
          }
    ],

    // Add custom actions and keybindings to this array.
    // To unbind a key combination from your defaults.json, set the command to "unbound".
    // To learn more about actions and keybindings, visit https://aka.ms/terminal-keybindings
    "actions":
    [
        // Copy and paste are bound to Ctrl+Shift+C and Ctrl+Shift+V in your defaults.json.
        // These two lines additionally bind them to Ctrl+C and Ctrl+V.
        // To learn more about selection, visit https://aka.ms/terminal-selection
        { "command": {"action": "copy", "singleLine": false }, "keys": "ctrl+c" },
        { "command": "paste", "keys": "ctrl+v" },

        // Press Ctrl+Shift+F to open the search box
        { "command": "find", "keys": "ctrl+shift+f" },

        // Press Alt+Shift+D to open a new pane.
        // - "split": "auto" makes this pane open in the direction that provides the most surface area.
        // - "splitMode": "duplicate" makes the new pane use the focused pane's profile.
        // To learn more about panes, visit https://aka.ms/terminal-panes
        { "command": { "action": "splitPane", "split": "auto", "splitMode": "duplicate" }, "keys": "alt+shift+d" }
    ]
}
```

- inputrc

  添加set bell-style none

- vimrc

  添加set t_vb=