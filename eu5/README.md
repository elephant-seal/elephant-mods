# Europa Universalis V

Keep each mod in its own folder under `eu5/`. Each mod folder is a standalone game-facing root with its own `.metadata/metadata.json` and any content directories it needs.

```text
eu5/
└── mod-name/
    ├── .metadata/
    │   └── metadata.json
    └── in_game/
```

For local testing on Windows, create a directory junction from the game's `Documents\Paradox Interactive\Europa Universalis V\mod\` folder to the individual mod folder, then enable the mod in your playset.
