![Timber Tales SMP Shop Permits](/gh-banner.jpg "Timber Tales SMP Shop Permits banner image")

# Timber Tales SMP Permits

This is the official resource pack for shop permits on the Timber Tales SMP server.

Credit to [SaplingEmo366](https://www.curseforge.com/members/saplingemo366/projects) for creating the Hermit Permits resource pack, which was used in the creation of this pack.

## Permit Commands

Below are command templates you can use to create your own custom-named permits. If you are interested in creating a whole set of pre-defined permits, check out our [Permit Manager]() datapack!

OP permissions are required for all commands listed below.

### Command Template

This is the structure of the command to follow. Be sure to replace the placeholder values in this template when using the command!

- **<PLAYER>**: The player name, or `@s`/`@p`
- **<TIER>**: Must be one of `diamond`, `gold`, or `iron`
- **<TIER_COLOR>**: Can be any Minecraft color name, recommended to use `aqua`, `yellow`, or `gray` - respective to the selected tier.
- **<TITLE>**: The title/name of the permit.
- **<LORE>**: Lore is optional, two examples are provided for the lore as the command will differ based on the number of lines you include in the lore.

The values assigned to "text" in both the TITLE and LORE can be any Minecraft-allowed text characters.

**Title Only**

```
/give <PLAYER> minecraft:paper[minecraft:custom_model_data={strings:['<TIER>']},:custom_name='{"text":"<TITLE>","color":"<TIER_COLOR>","italic":true}']
```

**Single Line Lore**

```
/give <PLAYER> minecraft:paper[minecraft:custom_model_data={strings:['<TIER>']},:custom_name='{"text":"<TITLE>","color":"<TIER_COLOR>","italic":true}',minecraft:lore=['[{text:"This is the lore/description",italic:false}]']]
```

**Multiple Line Lore**

```
/give <PLAYER> minecraft:paper[minecraft:custom_model_data={strings:['<TIER>']},:custom_name='{"text":"<TITLE>","color":"<TIER_COLOR>","italic":true}',minecraft:lore=['[{text:"This is the lore/description",italic:true}]','[{text:"This is the second lore line",italic:true}]']]
```

Please be aware both the in-game chat and server console have character limits. You can quickly exceed the in-game chat character limit when adding lore to permits. Here are some quick guidelines on where you can send these commands based on character count:

- 256 characters or less: In-game chat
- Over 256 characters: Server console

### Example Commands

Below are some example commands you can copy & paste directly into your world. 

**Sample Diamond with Multi-Line Lore**

```
/give @s minecraft:paper[minecraft:custom_model_data={strings:['diamond']},:custom_name='{"text":"⟡ Diamond Permit Sample ⟡","color":"aqua","italic":true}',minecraft:lore=['[{"text":"This is just an example permit and holds no value!","italic":true}]']]
```

**Sample Gold with Single-Line Lore**

```
/give @s minecraft:paper[minecraft:custom_model_data={strings:['gold']},:custom_name='{"text":"⟡ Gold Permit Sample ⟡","color":"yellow","italic":true}',minecraft:lore=['[{"text":"This example permit holds no value","italic":true}]']]
```

**Sample Iron with no Lore**

```
/give CoconuttMonkey minecraft:paper[minecraft:custom_model_data={strings:['iron']},:custom_name='{"text":"⟡ Iron Permit Sample ⟡","color":"aqua","italic":true}',minecraft:lore=['[{text:"This example permit",italic:true}]','[{text:"holds no value",italic:true}]']]
```

## Customizing the Permits

To customize the permits, you will need to use a tool like Blockbench (recommended), MCreator, or another image editing tool.

1. Unzip the resource pack
2. Navigate to the `assets/textures/item` directory
3. Open each the PNG files in your editor of choice, and customize as needed. 
4. When ready, save each of the files with the same name in the same folder, they should each be exactly 64px by 64px in size.
5. Upload the Timber Tales SMP Permits directory to your `/resourcepacks` directory. You do not need to ZIP it, however, if you prefer to you must select and compress the files & folders inside the root directory. Don't just right-click on the Timber Talse SMP Permits folder and click "ZIP" or "compress" - that won't work.