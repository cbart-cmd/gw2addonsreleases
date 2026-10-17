# GW2 Addon Releases

The addon manager checks each addon's direct download URL by requesting the same URL with
`.md5` appended. To publish an update, replace the relevant DLL and its
32-character lowercase MD5 file together:

- `timers.dll` and `timers.dll.md5`
- `fight_analysis_danger.dll` and `fight_analysis_danger.dll.md5`

They use  Direct update provider and point to their own
DLL. The MD5 sidecars are used by the addon manager to detect
a changed DLL. Do not publish source code or PDB files here.

Find latest dlls at [releases](https://github.com/cbart-cmd/gw2addonsreleases/releases/latest)

## Timers v0.3.15

The placement preview now lives in **Boons** and affects boons only. Timers have
their own **Also hear on the default device** setting, separate from Soundboard
and used for both alerts and five-second previews. The previous shared choice is
copied once on upgrade. Simulating Well of Corruption damage also shows two
clearly labelled mock countdowns without altering real counters; at most two
counters are visible in total, with real ones taking priority. Incoming counters
are circles with seconds inside; optional right-button dragging moves the group
and saves its position. Dragging is disabled by default.

## Timers v0.3.14

Optional incoming Well of Corruption counters in **Damage alerts**: up to two
independent 40-second WvW countdowns, smaller than the manual timers by default,
with their own position and size. Pulses from the same attacker are grouped for
6 seconds; a third well does not replace either active counter. Existing flashes
are unchanged. Requires ArcDPS combat events and the enabled damage alert for
skill 10545. Disabled by default.
