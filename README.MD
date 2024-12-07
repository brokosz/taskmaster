# Taskmaster Plugin for Obsidian

Creates a centralized index of all tasks in your vault.

## Features

- Tracks tasks (`- [ ]`, `* [ ]`) across all notes
- Groups tasks by source note
- Preserves header context
- Auto-updates when notes change
- Configurable task formats
- Links back to source locations

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

- Task Formats: `- [ ]` and `* [ ]`
- Index Location: `Task index.md`
- Auto Refresh: Enabled
- Include Headers: Enabled
- Refresh Interval: 5min

### Commands

- `Refresh Taskmaster`: Manually update the index
- Ribbon icon (checkbox): Same as above

### Index Format

```markdown
# Taskmaster

### [[note.md]]
Context: Section > Subsection
- [ ] Task text ([[note.md#5]])

### [[note.md]]
- [] Another task ([[note.md#10]])
```

## Development

1. Clone repo
2. `npm i`
3. `npm run dev` for development
4. `npm run build` for production

## License

MIT
