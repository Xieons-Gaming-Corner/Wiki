# Pokémon Showcase

The Pokémon Showcase lets users add, view, and delete Pokémon entries in a personal gallery.

## Commands

### `/pokemonshowcaseadd`
Add a Pokémon to your personal showcase.

**Options**
- `image` — Optional image or screenshot to attach to the entry.

**What you provide**
- Pokémon name.
- Shiny status.
- Optional note.

**Example**
- Pokémon: `Solgaleo`
- Shiny: `yes`
- Note: `My favorite legendary`

**What happens**
- The bot saves the entry to your Pokémon showcase.
- A private confirmation embed is shown.
- The embed includes the caller’s user information.

---

### `/pokemonshowcaseview`
View a scrollable gallery of a user’s Pokémon showcase.

**Options**
- `member` — Optional user whose showcase you want to view. Defaults to yourself.

**What it shows**
- Pokémon name.
- Shiny status.
- Notes.
- Image, if attached.

**Controls**
- `◀` and `▶` to move through entries.

---

### `/pokemonshowcasedelete`
Delete one of your Pokémon showcase entries.

**What it does**
- Opens a private gallery of your entries.
- Lets you scroll through them.
- Press **Delete** on the entry you want removed.

**Notes**
- Only the entry owner can use this flow.
- If the last entry is deleted, the flow closes.

---

## Fields

Each Pokémon entry may include:
- **Pokémon** — The Pokémon name.
- **Shiny** — Yes or No.
- **Notes** — Optional text.
- **Image** — Optional attached image.

## Behavior

- Showcase data is stored separately from BO7 relic data.
- View and delete flows are owner-locked.
- Command logs are sent to the log channel as embeds.
- Response embeds include the caller’s user information.

## Tips

- Use clear names for entries so they are easy to browse later.
- Attach an image when possible for better presentation.
- Keep notes short and descriptive.
