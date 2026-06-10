# ghostty-patched

Personal CI builder: upstream [Ghostty](https://github.com/ghostty-org/ghostty)
stable releases + `new_tab_with_command` keybind action patch.

```ini
keybind = super+ctrl+digit_1=new_tab_with_command:ssh zabbix
```

- Weekly cron checks for a new upstream `v*` tag; builds only when one appears.
- Manual: Actions → Build patched Ghostty → Run workflow (optionally pin a tag).
- Output: GitHub Release `<tag>-patched` with `Ghostty-patched.zip`.
- Local install: `ghostty-sync` (downloads latest release, swaps /Applications/Ghostty.app).

Patch authored with Claude Code (AI-assisted), reviewed locally. For private use.
