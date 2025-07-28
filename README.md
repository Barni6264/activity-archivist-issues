# Activity Archivist - issue tracker
Report issues and bugs regarding **Activity Archivist#4042**, or suggest new features here.<br/>

- ***Quick note: The bot only updates your playtime when your Discord status changes. (e.g., when you exit the game)***
<br/><br/><br/>

## Basic commands to help you get started:

### Help
#### /help [submenu]
Displays the help menu. Use */help* to view the full list, or */help [submenu]* to show details about a specific command. (e.g., */help track*)

### Track
#### /track {user}
Creates a profile for the mentioned user (You can use */track @yourusername* to register yourself or */track @otherusername* to register someone else).
The bot only tracks users who are registered. If you're not registered, just run the command once.

### Stats
#### /stats [user]
Shows saved playtime and activity statistics. Use */stats* to fetch your own data, or */stats @username* to view someone else's.<br/>
**Important:**
- only works on registered users (see */track*)
- you can block others from tracking or accessing your stats (see */block-tracking*)

### Block tracking
#### /block-tracking [block] [user]
Controls who can access your stats and whether your activity is recorded.<br/>
Two main uses:
**(1)** 'un-register' yourself (pause all tracking)
**(2)** block/unblock a specific user from using */stats* on you

Two optional arguments (*block* and *user*).
- *block*:
- - *Block* or *Allow*
- - default is *Block*
- *user*:
- - blocks or unblocks the specified user
- - if left empty, applies to all users globally

Examples:
- */block-tracking @example123*
- - blocks @example123
- */block-tracking*
- - pauses playtime recording and blocks */stats @yourusername* for everyone (same as */block-tracking Block*)
- */block-tracking Allow*
- - 're-register' yourself again (opposite of */block-tracking* or */block-tracking Block*)

### Delete data
#### /delete-data 'DELETE'
Permanently removes all saved playtime stats.<br/>
Note: */delete-data* does not disable tracking and does not unregister you. (see */block-tracking*)

### Remove
#### /remove {game} 'REMOVE'
Resets all saved playtime for the specified game (removes a game from the pie chart)<br/>

### About
#### /about
Shows info about the bot and the developer

### Autostat
#### /autostat
Automatically sends you a DM containing all saved stats every 24 hours (like */stats*). (supporters only)
Toggle autostat on/off with this command.
Note: Message is sent every day at 10:00 PM (22:00) GMT/UTC

### Support
#### /support
Donations, supporter status, and how to become a supporter.
