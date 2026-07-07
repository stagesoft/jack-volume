# jack-volume (CUEMS fork)

Part of the **CUEMS** ecosystem — see the [`cuems-RELATIONS`](https://github.com/stagesoft/cuems-RELATIONS) repo for the system index, architecture diagram, and protocol/port map.

## Role

Stagesoft fork of `jack-volume` — a JACK client that controls the volume of multiple audio channels via OSC (it forwards input→output channels applying per-channel + master gain, no mixing). In CUEMS this is the **`cuems-jack-volume` / `0_mixer`** volume client that **`cuems-audioplayer` depends on** (audio playback is routed through it over JACK). OSC over UDP/TCP (default port 7600); address = `/<domain>/<application>/<client-name>/<channel|master>`.

Support/library repo; no CUEMS-specific operational gotchas recorded yet. See the cuems-audioplayer CLAUDE.md for how the player uses it.
