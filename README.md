store-skins
============

### Description
Store module that allows players to buy custom skins in the store to customize the appearance of their character.

### Requirements

* [Store](https://forums.alliedmods.net/showthread.php?t=207157)
* [SMJansson](https://forums.alliedmods.net/showthread.php?t=184604)

### Installation

Download the `store-skins.zip` archive from the plugin thread and extract to your `sourcemod` folder intact. Then, navigate to `configs/store/sql-init-scripts/` and execute `skins.sql` in your database.

### Adding More Skins

Until the web panel for the store will be ready, you'll need to update the database directly to add more items. To do that, open your phpMyAdmin and create a new row in `store_items`. Change `name`, `display_name`, `description` and `attrs` to customize the new skin. In `type` and `loadout_slot`, type **skin**. 

Example of an attrs field for skins:

    {
        "model": "models/player/kirby/admin/umbrella_leet.mdl",
        "teams": [2, 3]
    }
