# LazyPig

A World of Warcraft 1.12 addon for Turtle WoW that automates repetitive tasks. Configure in-game with `/lp` or `/lazypig`.

## Features

### Passive (always active when enabled)

| Feature | Description |
|---------|-------------|
| **Auto Dismount** | Dismounts when casting, interacting with flight masters, etc. Handles Turtle WoW expansion mounts and AQ40 mounts. |
| **Auto Stance** | Automatically switches to the correct stance/form when a spell requires it. |
| **Gossip Processing** | Auto-selects gossip options when talking to NPCs (taxi, battlemaster, innkeeper, vendor, banker). Hold Shift to bypass. |
| **Loot at Cursor** | Positions the loot frame under your cursor. |
| **Improved Right Click** | Right-clicking a bag item while trade, auction, or mail is open places it directly into that window. |
| **Chat Spam Filter** | Hides repeated messages in say/yell/channel chat (70s cooldown per unique message). Also suppresses BigWigs cast spam and `#showtooltip` errors. |
| **Loot Roll Messages** | Optionally hides green/blue roll messages and grey/white loot messages from chat. |
| **World Chat Mute** | Mutes /world channel while in raids, dungeons, or battlegrounds. Automatically rejoins when you leave. |
| **Auto Cancel Duels** | Instantly cancels incoming duel requests. |
| **Auto Accept Invites** | Accepts group invites from guild members, friends, or everyone (configurable). Can be disabled while in BG or BG queue. |
| **Auto Accept Summons** | Accepts summons 2 seconds before they expire. |
| **Auto Accept Resurrections** | Accepts resurrections in instances/BGs when the resurrecter is out of combat. |
| **Extended Camera** | Increases max camera distance to 50 yards. |

### Battlegrounds

| Feature | Description |
|---------|-------------|
| **Auto Queue** | Automatically queues for the battleground when the battlemaster window opens. |
| **Auto Join** | Joins the battleground a few seconds before the invitation expires. |
| **Auto Leave** | Leaves the battleground when a winner is declared. |
| **Auto Release** | Releases spirit on death in battlegrounds. |
| **Block Quest Sharing** | Blocks quest share popups while in battlegrounds. |
| **Queue Announce** | Announces BG queue status to party/raid as leader. |
| **WSG Flag Carrier Tracking** | Tracks the enemy flag carrier. Bind a key to target them or drop the flag. |

### Loot Rolling

All roll options support 4 modes: Off, Need, Greed, Pass.

| Feature | Items |
|---------|-------|
| **ZG** | Hakkari Bijous and Coins |
| **MC** | Blood of the Mountain, Fiery Core, Lava Core |
| **AQ** | Scarabs and Idols |
| **Naxx** | Wartorn Scraps |
| **Corrupted Sand** | Corrupted Sand (auto-need) |
| **Dream Shards** | Dreamscale, Fading Dream Fragment, Small Dream Shard |
| **Green Items** | All uncommon (green) quality items |
| **BG Loot** | Auto-need on everything in Alterac Valley |

Necrotic Runes are always auto-needed.

### Buff Removal

| Feature | Description |
|---------|-------------|
| **Remove Salvation** | Auto-removes Blessing of Salvation. Two modes: always, or only while tanking (warrior with shield, druid in bear form, paladin with Righteous Fury, shaman tank with Spirit Armor). |
| **Remove Mana Buffs** | Auto-removes Blessing of Wisdom, Arcane Intellect/Brilliance, Divine Spirit/Prayer of Spirit. Disabled in battlegrounds. |

When [SuperWoW](https://github.com/balakethelock/SuperWoW) or [Nampower](https://github.com/pepopo978/nampower) are installed, buff removal uses spell IDs instead of tooltip scanning for better performance.

### Active (require modifier keys)

| Keys | Action |
|------|--------|
| **Alt + Ctrl + Shift** | Logout (only if no keybind is set for Logout) |
| **Ctrl + Shift** | Follow target |
| **Alt + Shift** | Inspect target; bid on auction |
| **Alt + Ctrl** | Initiate/accept trade; confirm popups (invite, BG entry, release spirit, corpse recovery, summon, etc.); click send mail / create auction / buyout auction; roll on green items |
| **Shift** (at merchant) | Sell grey items and repair all |
| **Alt** (at quest detail) | Accept quest |

### Stack Splitting

Hold **Shift + Right Click** on a stacked item to enter split mode. Use **Alt** to increase and **Ctrl** to decrease the split count. The display shows the current split value.

### Repeatable Quest Replay

Hold **Alt** while completing a repeatable quest to record it. Next time you talk to the same NPC with Alt held, all previous actions replay automatically. Works with BG mark turn-ins, AD scourge stones/insignias, ZG coins, and Thorium Shells.

## Keybinds

Set these in the standard WoW Key Bindings menu under the **_LazyPig** header:

| Binding | Action |
|---------|--------|
| Logout | Logs out |
| Unstuck | Sends unstuck request |
| Reload UI | Reloads the interface |
| Duel / EFC | In WSG: targets enemy flag carrier. Elsewhere: starts or cancels a duel |
| Drop WSG Flag | Drops the Warsong flag and cancels Slow Fall |
| Menu | Opens the LazyPig options menu |

## Addons You Can Replace

LazyPig covers the functionality of these addons:
- Auto Profit
- Ez Dismount
- Automaton
- Quick Loot
- Block Salvation

If using **MailTo** alongside LazyPig, disable Improved Right Click and Shift Split/Merge in LazyPig to avoid conflicts.
