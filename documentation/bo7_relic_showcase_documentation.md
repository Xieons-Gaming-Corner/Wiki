# BO7 Relic Showcase

The BO7 Relic Showcase lets users add, view, and delete BO7 relic entries in a personal gallery.

## Commands

### `/relicshowcaseadd`
Add a BO7 relic to your personal showcase.

**Options**
- `image` — Optional image or screenshot to attach to the entry.

**What you provide**
- Relic name.
- Tier.
- Map.
- Shiny status.
- Optional note.

**Supported tiers**
- `Grim`
- `Wicked`
- `Sinister`

**Supported maps**
- `Ashes`
- `Astra`
- `Nuketown`
- `Totenreich`
- `Kowakujo`

**Example**
- Relic name: `Samantha's Drawing`
- Tier: `Sinister`
- Map: `Astra`
- Shiny: `yes`
- Note: `Pulled after a long run`

**What happens**
- The bot saves the entry to your BO7 relic showcase.
- A private confirmation embed is shown.
- The embed includes the caller’s user information.

---

### `/relicshowcaseview`
View a scrollable gallery of a user’s BO7 relic showcase.

**Options**
- `member` — Optional user whose relic showcase you want to view. Defaults to yourself.

**What it shows**
- Relic name.
- Tier.
- Map.
- Shiny status.
- Notes.
- Image, if attached.

**Controls**
- `◀` and `▶` to move through entries.

---

### `/relicshowcasedelete`
Delete one of your BO7 relic showcase entries.

**What it does**
- Opens a private gallery of your entries.
- Lets you scroll through them.
- Press **Delete** on the entry you want removed.

**Notes**
- Only the entry owner can use this flow.
- If the last entry is deleted, the flow closes.

---

## Fields

Each BO7 relic entry may include:
- **Relic** — The relic name.
- **Tier** — Grim, Wicked, or Sinister.
- **Map** — The map name.
- **Shiny** — Yes or No.
- **Notes** — Optional text.
- **Image** — Optional attached image.

## Behavior

- Showcase data is stored separately from Pokémon data.
- View and delete flows are owner-locked.
- Command logs are sent to the log channel as embeds.
- Response embeds include the caller’s user information.

## Tips

- Choose the correct tier and map before submitting.
- Attach an image when possible for better presentation.
- Keep notes short and descriptive.
