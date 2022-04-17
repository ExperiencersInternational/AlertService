# Setting up NotificationService in your plugin

You can set up NotificationService to use in your plugin by just adding one line of code. Here's how you can do that:

Warning: Unless you want to make NotificationService a required dependancy, I would recommend adding an if statement that checks if it's there, if it is there, then it will require the module and send the notification, but if it isn't, you could print a message to the output.

```
require(game.PluginGuiService.NotificationService.DockWidgetGUI.Module.MainModule).Send()
```

That's it. Although, it requires 4 parameters, let me explain what each one is:

Parameter 1: Notification title (string)

Parameter 2: Notification icon (string, use this: 'http://www.roblox.com/asset/?id=(imageidhere)'

Parameter 3: Notification Description (string, required)

Parameter 4: Notification Duration (string or number)

Parameters 1, 2 and 4 will automatically revert to a default if it is not submitted.
