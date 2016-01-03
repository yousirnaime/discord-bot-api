Install
---
1. Copy the plugin to the `_plugins` directory.
2. Run `npm install` in the plugin directory itself
3. Start up the your bot and enable the plugin with `!enable music-bot`

Commands
---
* `!music add <link>` - Adds a song to the playlist (currently only YouTube supported)
    + Example: `!music add https://www.youtube.com/watch?v=iyqfHvoUtkU`
* `!music remove <link>` - Removes a song to the playlist
    + Example: `!music remove https://www.youtube.com/watch?v=iyqfHvoUtkU`
* `!music skip` - Skips the current song
* `!music play` - Starts the playlist
* `!music stop` - Stops the playlist
* `!music current` - Displays the current song
* `!music playlist` - Displays all songs on the playlist
* `!music enter <Channel name>` - Let the bot enter a voice channel
    + Example: `!music enter General`

Config
---
You can configure the `music-bot` by extending your `config.json` with the following:

With `commandPrefix` you can set a custom command prefix for this plugin (optional). It defaults to `music`  
With `library` you can define where the songs should be downloaded to.  
With `skipLimit` you can define how many users you need to skip the current song (optional). It defaults to `1`  
With `announceSongs` you can enable or disable the announcing of the current song (optional). It defaults to `true`  
With `autoJoinVoiceChannel` you can define a voice channel which the bot trys to enter when it starts up.

Example
---
```json
"plugins": {
    "music-bot": {
        "commandPrefix": "custom-command-prefix",
        "library": "../music",
        "skipLimit": 1,
        "announceSongs": true,
        "autoJoinVoiceChannel": "Channel name"
    }
}
```

Need help?
---
Join my Discord server: https://discord.gg/0jV29zKlvdJbDx3f