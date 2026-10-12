# GW2 Addon Releases

Public binary distribution for Guild Wars 2 Nexus addons. This repository contains
only compiled addon DLLs and their MD5 sidecars; source code remains in the
respective private repositories.

Nexus checks each addon's direct download URL by requesting the same URL with
`.md5` appended. To publish an update, replace the relevant DLL and its
32-character lowercase MD5 file together:

- `timers.dll` and `timers.dll.md5`
- `fight_analysis_danger.dll` and `fight_analysis_danger.dll.md5`

The addon projects use Nexus's Direct update provider and point to their own DLL,
so each addon receives only its matching binary. The MD5 sidecars are used by
Nexus to detect a changed DLL.
