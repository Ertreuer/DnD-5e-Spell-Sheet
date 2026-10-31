# D&D Spell List

A simple, single-file spell list manager for your Dungeons & Dragons characters. Keep one list per character, track your spells, prepared spells and spell slots, and print or export your lists.

> **Disclaimer:** This project was created with the help of AI.

## Features

- Multiple spell lists: one per character, all stored on your device
- Create a list by choosing a class and level (1–20), spell slots are filled in automatically and can be adjusted freely
- Spell cards with level, school, class, casting time, range, components and duration, plus tags for concentration and ritual
- Mark spells as prepared (★) and filter to prepared spells only
- Clickable spell slot counters in a compact row, with a Long Rest button
- Tabs per spell level (cantrips to level 9), plus search
- Compact print layout (two columns, grouped by level)
- Export all lists as a JSON backup, export a single list as Markdown, and import a backup again
- Dark theme (black and grey with purple accents)
- No installation, no server, no accounts, no tracking

## Quick start

1. Download `index.html`.
2. Open it in any modern browser (Chrome, Firefox, Safari, Edge).
3. Click **+ New list** and start adding spells.

That's it. The whole app is one HTML file with no external dependencies.

Or

1. Open the link https://ertreuer.github.io/DnD-5e-Spell-Sheet/ and start with How to use.

## How to use

### Create a list

1. On the start page, click **+ New list**.
2. Fill in the form:
   - **List name**: optional, e.g. *Elara* (defaults to class and level)
   - **Class**: Artificer, Bard, Cleric, Druid, Paladin, Ranger, Sorcerer, Warlock, Wizard, the Eldritch Knight and Arcane Trickster subclasses, or a non-caster
   - **Level**: 1 to 20
   - **Spell slots**: filled in from your class and level, change any number you like
3. Click **Create list**.

> **Note:** Multiclassing is not supported. Create one list per class instead.

Open, rename or delete your lists from the start page. Use **← All lists** to get back from a list.

### Add a spell

1. Open a list and click **+ New spell**.
2. Fill in the form:
   - **Name**: e.g. *Fireball*
   - **Level**: Cantrip or level 1 to 9
   - **School**: the eight schools of magic
   - **Class**: e.g. *Wizard* (prefilled from your list)
   - **Casting time, Range, Components, Duration**: e.g. *1 action*, *150 ft*, *V, S, M*, *Instantaneous*
   - **Concentration / Ritual / Prepared**: tick what applies
   - **Description / notes**: anything you want to remember
3. Click **Save**.

### Track spell slots

The **Spell slots** panel shows all nine levels in one row.

- Type a number under a level to set how many slots you have.
- Click a circle to mark a slot as spent. Click it again to give it back.
- **Long Rest** restores all slots.
- **↺ Class defaults** resets your slots to the values for your class and level.

Warlocks use Pact Magic, so all their slots sit at one level (shown under that level).

### Find things fast

- Use the **tabs** to show only one spell level (the number shows how many entries it has).
- Use **★ Prepared only** to hide everything you haven't prepared.
- Use the **search box** to filter by name, description, school or class.

### Edit or delete

Every card has **Prepare / Unprepare**, **Edit** and **Delete** buttons.

### Print

Click **Print**. The print view always shows all spells of the list, sorted by level, in two compact columns, without buttons or tabs. In the print dialog you can switch to a different paper size or save as PDF.

### Export and import

- **Export backup (JSON)** (start page) saves all your lists to one file. Use this to back up your characters or move them to another device.
- **Export list (Markdown)** (inside a list) saves a readable list grouped by spell level, handy for notes apps or Discord.
- **Import backup** loads a JSON backup. It replaces all your current lists after you confirm.

## Your data

Everything is stored in your browser's local storage on your own device. Nothing is sent anywhere.

- Each person (and each browser) has their own lists.
- Clearing your browser data deletes your lists, so export a backup now and then.
- To use the same lists on another device, export a JSON backup and import it there.
- To share a ready-made character with a friend, send them your JSON file.

## Hosting it for free

Because it's a single static file, you can host it almost anywhere:

- **GitHub Pages**: upload `index.html` to a repository, then go to *Settings → Pages* and select your main branch.
- **Netlify Drop**: drag the file onto [app.netlify.com/drop](https://app.netlify.com/drop).
- **Cloudflare Pages** or any other static host works too.

Share the link with your party. Everyone gets their own private lists.

## Customizing

All colors are defined as CSS variables at the top of `index.html` (`--bg`, `--card`, `--acc`, and so on), so you can change the theme in a few lines. The class list and the slot tables are plain JavaScript arrays near the top of the script, and the schools are an array right above them, so you can edit them directly.

## Credits

Made by Ertreuer.

## Disclaimer

This project was created with the help of AI. It is an unofficial fan tool and is not affiliated with or endorsed by Wizards of the Coast. Dungeons & Dragons is a trademark of Wizards of the Coast LLC. Spell slot tables follow the 5e core rules. Please check rules and numbers against your official sources.
