# GW2 Addon Releases

The addon manager checks each addon's direct download URL by requesting the same URL with
`.md5` appended. To publish an update, replace the relevant DLL and its
32-character lowercase MD5 file together:

- `timers.dll` and `timers.dll.md5`
- `fight_analysis_danger.dll` and `fight_analysis_danger.dll.md5`
- `gw2_builds.dll` and `gw2_builds.dll.md5`

They use  Direct update provider and point to their own
DLL. The MD5 sidecars are used by the addon manager to detect
a changed DLL. Do not publish source code or PDB files here.

Find latest dlls at [releases](https://github.com/cbart-cmd/gw2addonsreleases/releases)

MADE WITH AI (Astra, Deepseek, Sonet, Claude chat, Gemini chat).

## Timers 

Timers

## WvW Insights

Similar to Wvw Analysys, personalized for my needs.

## GW2 Builds and rotations

Shows WvW Builds and rotations. It does NOT press the skills for you.
