# Project Ghostlink v1.4.0 — Windows

These notes list changes added after v1.3.8.

## Much faster teleports and writes

The new **Fast Body** method makes teleports much faster by writing the target position directly to the live physics body and waking it. Auto and Physics Body remain available.

Ghostlink is much faster for eligible writes. **Fast Writes** removes the fixed 100 ms transfer pause and is enabled by default for new settings. Some small, single-address changes skip the backup read and readback, so those writes are quicker but are not verified in the same way as larger edits.

## Main Mods and layout

- Main Mods now groups controls into **Simple Mods**, **Player & Gear**, **Movement & World**, **Visuals**, **Activities**, and **Tools**.
- The separate Console page has been retired. Advanced controls are grouped under Testing, and Main Mods controls take priority where features overlap.
- **Pinned** is its own sidebar page. Pin individual controls or sections, arrange them into custom sections, drag to reorder, and unpin them. Pinned controls remain usable on that page.
- **On Connect** can queue supported actions, including changing the player name and enabling Anti-Matchmaking. More queued options are planned for future updates.

## Character Editor improvements

- Raw addresses, offsets, and byte changes stay hidden unless **Show Technical Details** is enabled in Settings.
- Edit messages identify the changed item and slot.
- **Appearance Only** compares mapped pattern, art, and model-part data. Cross-type appearance copies are restricted because copied fields can change gameplay behavior.

## Loot

- **Use This Preset** installs the selected Pickup Filter and turns it on.
- **Swap Assist** can apply the selected filter after Full Swap and Cross-Slot changes. Infinite Ammo remains a separate manual control.

## Gameplay tools

- **Void Enemies** and **Relative OPK** are always available at **Main Mods → Tools → Player Effects**. They do not require Show Experimental Tools. The modes share one hook and require a supported game fingerprint. Relative OPK accepts X/Y/Z offsets from −30 to 30.
- Warpriest Start and Randomize Consumables are experimental tools. The randomizer's field meanings are not fully verified.
