# Taskmaster Plugin for Obsidian

Centralizes all tasks in your vault into an easy-to-reference index.

## Features

- Tracks standard Markdown tasks (`- [ ]`, `* [ ]`) and custom formats across all notes
- Groups tasks by source note and context
- Preserves header hierarchy
- Auto-updates when notes change
- Quick links to source locations

## Installation

1. In Obsidian, go to Settings → Community plugins → Browse
2. Search for "Taskmaster"
3. Click Install
4. Enable the plugin in Community plugins

## Usage

### Initial Setup

1. Enable the plugin
2. Configure settings if needed (Settings → Taskmaster)
3. Click the checkbox icon in the ribbon or run "Refresh Taskmaster" command

### Default Settings

- Task Formats: `- [ ]`, `* [ ]` (plus any custom formats)
- Index Location: `Taskmaster.md`
- Auto Refresh: Enabled
- Include Headers: Enabled
- Refresh Interval: 5min

### Commands

- `Refresh Taskmaster`: Manually update the index
- Ribbon icon (File with checkmark): Same as above

### Index Format

```markdown
# Taskmaster

### example.md
**Context: [[example.md#Project-Planning|Daily Notes > Project Planning]]**
☐ Review project timeline (L137)
☐ Update team documentation (L138)

### tasks.md
☐ Contact vendor about delivery (L45)
```

## Development

1. Clone repo
2. `npm i`
3. `npm run dev` for development
4. `npm run build` for production

## License

MIT
