# awesome-djhardware-unchained [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome future-facing research, enhancements and projects for DJ hardware. It started with the
abandoned TORAIZ ecosystem (SP-16, SQUID, AS-1) and the DJS-1000, and now covers related devices such as the
RMX-1000 and EFX-1000, subcontroller support and integration (DDJ-XP1, DDJ-XP2, DDJ-SP1), CDJs and DJMs, PRO DJ
LINK, DIY builds, and repos sympathetic to the cause: pieces waiting to be put together in new ways.

Repo dedicated to Prometheus, Eris, and all those actively creating a better world by creating and collaborating,
not destroying and alienating.

Unofficial. Not affiliated with or endorsed by Pioneer DJ or AlphaTheta; product names belong to their owners. This list
links to projects; it hosts no firmware. Each project's licence is its own: many below state none, which means all
rights reserved (read and cite, don't copy).

## Contents

- [TORAIZ SP-16](#toraiz-sp-16)
- [DJS-1000](#djs-1000)
- [TORAIZ SQUID](#toraiz-squid)
- [TORAIZ AS-1](#toraiz-as-1)
- [CDJ and DJM](#cdj-and-djm)
- [RMX-1000 and EFX-1000](#rmx-1000-and-efx-1000)
- [DDJ Subcontrollers: DDJ-XP1, DDJ-XP2, DDJ-SP1](#ddj-subcontrollers-ddj-xp1-ddj-xp2-ddj-sp1)
- [Helper apps](#helper-apps)
- [PRO DJ LINK](#pro-dj-link)
- [3D printing](#3d-printing)
- [Other](#other)
- [See also](#see-also)
- [Contributing](#contributing)

## TORAIZ SP-16

- [sp16-emulator](https://github.com/noturderek/sp16-emulator) - Runs the SP-16's own firmware update on a computer, with a virtual panel. Unlicense.

## DJS-1000

- [djs1000-emulator](https://github.com/noturderek/djs1000-emulator) - DJS-1000 port of the SP-16 emulator. Unlicense.
- [djs1000-emu](https://github.com/commit-collective/djs1000-emu) - Independent emulator under QEMU user mode (Linux / WSL2) with PRO DJ LINK, live sampling and headphone output. GPL-2.0-or-later.
- [deckbench](https://github.com/commit-collective/deckbench) - Simulated CDJs for testing the DJS-1000's SYNC and MASTER against.
- [djsvisuals](https://github.com/DirtySecretz/djsvisuals) - DJS-1000 visuals.

## TORAIZ SQUID

- [squid-editor](https://github.com/oldwired/squid-editor) - Browser editor for `.prj` projects, with MIDI import / export and WebHID transfers. MIT.
- [squid-firmware](https://github.com/canadianblaken/squid-firmware) - Firmware 1.13 static analysis notes and an offline patcher. Flashing patched images can brick the unit.

## TORAIZ AS-1

- [ToraizDump](https://github.com/KnightHill/ToraizDump) - Dumps the 64-step sequencer over MIDI SysEx.
- [TORAIZ-AS-1-MIDI-Toolkit](https://github.com/TheMicronauts/TORAIZ-AS-1-MIDI-Toolkit) - MIDI cheat sheet (CC / NRPN), patch sheets and Cubase / Nuendo parts.
- [KnobKraft-orm](https://github.com/christofmuc/KnobKraft-orm) - Cross-platform MIDI SysEx librarian with a TORAIZ AS-1 adaptation. AGPL-3.0.
- [CtrlrPanelSequential](https://github.com/synthmutt/CtrlrPanelSequential) - Ctrlr editor panels for Sequential synths, including the AS-1. GPL-3.0.
- [m4l-AS1](https://github.com/m43d4k/m4l-AS1) - Max for Live MIDI effects for the AS-1, such as a bank / program changer (README in Japanese).

## CDJ and DJM

The players and mixers a TORAIZ sits next to.

### Emulators

Same approach as the TORAIZ emulators: the unit's own firmware under QEMU.

- [cdj3k-emu](https://github.com/nsaintot/cdj3k-emu) - CDJ-3000 with emulated controls, jog LCD, USB and DJ Link.
- [cdj3k-emu-windows](https://github.com/bazda999/cdj3k-emu-windows) - Windows port of cdj3k-emu.
- [cdj2000-emulator](https://github.com/cdj2k-revival/cdj2000-emulator) - CDJ-2000 on emulated processors.
- [cdj-nxs2-qemu](https://github.com/Stijn-Jacobs/cdj-nxs2-qemu) - CDJ and XDJ emulator.

### Firmware research

- [1500X-Research](https://github.com/DRCRecoveryData/1500X-Research) - CDJ-1500X firmware and GPL source analysis log.

### Mods

These change the software on a real unit. Read each project's warnings; a failed flash can brick the player.

- [cdj3k-mods](https://github.com/nsaintot/cdj3k-mods) - Quality-of-life features for the CDJ-3000.
- [xdj-az-mods](https://github.com/Kyle-Hosman/xdj-az-mods) - XDJ-AZ root and community mods.
- [rx3-toolkit](https://github.com/Tratosca/rx3-toolkit) - XDJ-RX3 mods.

### USB drives and rekordbox

- [booth](https://github.com/jwilkins/booth) - Writes CDJ USB drives without rekordbox, in both the legacy and the newer on-drive format.
- [rbxport](https://github.com/chrisle/rbxport) - Music library manager with USB export and DJ Link.
- [crate-digger](https://github.com/Deep-Symmetry/crate-digger) - Java library for rekordbox exports and analysis (ANLZ) files.
- [rekordcrate](https://github.com/Holzhaus/rekordcrate) - Rust parser for rekordbox device exports.
- [pyrekordbox](https://github.com/dylanljones/pyrekordbox) - Python package for the rekordbox database, XML, ANLZ and My Settings files.
- [rekordbox-parser](https://github.com/evanpurkhiser/rekordbox-parser) - JavaScript parser for `export.pdb` files.
- [onelibrary](https://github.com/v1vendi/onelibrary) - Tooling for the OneLibrary format.
- [onelibrary-connect](https://github.com/chrisle/onelibrary-connect) - Reads OneLibrary (`exportLibrary.db`) databases.

### Mixers

- [Pioneer-DJM-850-driver-reverse-engineering](https://github.com/nm2107/Pioneer-DJM-850-driver-reverse-engineering) - Notes on the DJM-850 Windows driver.
- [DJM-850Audio](https://github.com/zavorka/DJM-850Audio) - DJM-850 USB audio driver for macOS.
- [DJMT1Driver](https://github.com/cYpherBass/DJMT1Driver) - DriverKit audio driver for the DJM-T1 on current macOS.

## RMX-1000 and EFX-1000

No projects for the units themselves yet. Software inspired by the RMX-1000:

- [x-1000](https://github.com/manoelpiovesan/x-1000) - Software X-PAD section with Ableton Link.
- [AFX-1000](https://github.com/AxelMcKenna/AFX-1000) - RMX-style effects for macOS as AU / VST3.
- [fx-station](https://github.com/victorbazet/fx-station) - Browser effects station for a mixer send / return.
- [RMXXXL](https://github.com/sunskiefer/RMXXXL) - RMX-style remix effect for MPC OS on the Akai Force.
- [rmx1000](https://github.com/MarvinKropf2/rmx1000) - RMX-style sampler on a DDJ-FLX4's PAD FX 2 mode in rekordbox (README in German).
- [xpad](https://github.com/ojdvw124/xpad) - X-PAD drum-roll sampler for iPad.

## DDJ Subcontrollers: DDJ-XP1, DDJ-XP2, DDJ-SP1

Pad controllers that could drive a TORAIZ or a TORAIZ emulator over MIDI.

- [StepXP1](https://github.com/AlChen31974/StepXP1) - 32-step MIDI sequencer played from a DDJ-XP1, in Python, synced to Ableton Live (README in French).
- [sp1](https://github.com/theaugy/sp1) - Mixxx controller script for the DDJ-SP1.
- [DDJ-SP1](https://github.com/dmvjs/DDJ-SP1) - DDJ-SP1 interface for a web client.
- [autopilot-mappings](https://github.com/chrisle/autopilot-mappings) - Controller map collection with maps for the DDJ-XP1, DDJ-XP2, DDJ-SP1 and the TORAIZ SP-16.
- [DJ-MIDI-Studio](https://github.com/guillain/DJ-MIDI-Studio) - Manages DJ MIDI mappings, with a DDJ-XP2 layout and controller emulator.
- [rekordbox-dj](https://github.com/alexrster/rekordbox-dj) - rekordbox MIDI mappings and scripts, with notes on the DDJ-XP1's Slide FX and RMX-1000-style effects.
- [RekordTrakt](https://github.com/Morgazmo/RekordTrakt) - MIDI bridge for other controllers in rekordbox, using a DDJ-XP1 as the hardware unlock. GPL-3.0.

## Helper apps

Apps that work with more than one TORAIZ unit.

- [Strands](https://github.com/ezoray/Strands) - Turns a song or its stems into a project for the SP-16 and DJS-1000.
- [playable-gear-manuals](https://github.com/canadianblaken/playable-gear-manuals) - Playable browser recreation of the SQUID panel with guided tours (also Blackbox, Hapax, KeyStep Pro). MIT.

## PRO DJ LINK

The SP-16 and DJS-1000 sync to CDJs over PRO DJ LINK; these let a computer join in, watch, or bridge the clock to
gear without DJ Link (a SQUID or AS-1 over MIDI, for example).

### Clock and sync bridges

- [CDJ_Clock](https://github.com/g-zi/CDJ_Clock) - DJ Link to Ableton Live clock.
- [canihazmidi](https://github.com/IljaN/canihazmidi) - Box that turns DJ Link clock into MIDI clock.
- [beat-carabiner](https://github.com/Deep-Symmetry/beat-carabiner) - Tempo bridge between DJ Link and Ableton Link.
- [SuperTimecodeConverter](https://github.com/fiverecords/SuperTimecodeConverter) - Timecode router: MTC, Art-Net, LTC and DJ Link.
- [autoblink](https://github.com/strikeout/autoblink) - DJ Link to MIDI clock, MTC, CC, OSC and MIDI notes, for DAWs, drum machines, synths and DMX.
- [ORVIK](https://github.com/Zesminseok/ORVIK) - DJ hardware to Resolume sync over TCNet.
- [beat-link-trigger](https://github.com/Deep-Symmetry/beat-link-trigger) - Triggers events and automates shows from what the players are doing.
- [open-beat-control](https://github.com/Deep-Symmetry/open-beat-control) - A subset of beat-link over Open Sound Control.

### Monitoring

- [prolink-tools](https://github.com/evanpurkhiser/prolink-tools) - Now-playing overlays and other DJ Link tools.
- [prolink-monitor](https://github.com/fidow/prolink-monitor) - Live view of loaded tracks and playheads.
- [vizlink](https://github.com/nzoschke/vizlink) - Reads DJ Link devices and emits JSON.
- [cdj-music-link](https://github.com/silmin/cdj-music-link) - Raspberry Pi joins as a virtual CDJ and serves player state as a read-only HTTP / SSE API. MIT.

### Virtual players

Software CDJs and mixers on the network: something for a DJS-1000 or SP-16 to sync to without a booth.

- [CDJ_DJM_Emulator](https://github.com/OllieCross/CDJ_DJM_Emulator) - Up to four virtual CDJs and a DJM on a software LAN, for DJ Link consumers.
- [vynull](https://github.com/vynulldev/vynull) - Virtual CDJ and rekordbox source for Linux: serves music to CDJs with waveforms, beat grids and cues. GPL-3.0.

### Libraries

- [beat-link](https://github.com/Deep-Symmetry/beat-link) - Java; the reference implementation.
- [prolink-connect](https://github.com/evanpurkhiser/prolink-connect) - TypeScript / JavaScript.
- [prolink-go](https://github.com/evanpurkhiser/prolink-go) - Go.
- [python-prodj-link](https://github.com/flesniak/python-prodj-link) - Python.
- [node-pro-dj-link](https://github.com/maxjoehnk/node-pro-dj-link) - Node.js.
- [prolink](https://github.com/usr-ein/prolink) - Rust.
- [prodjlink-rs](https://github.com/Compellerai/prodjlink-rs) - Rust, for monitoring.
- [prolink-cpp](https://github.com/grantHarris/prolink-cpp) - C++.

### Protocol analysis

- [dysentery](https://github.com/Deep-Symmetry/dysentery) - The protocol analysis everything else builds on.
- [pioneer-link-wireshark](https://github.com/b5i/pioneer-link-wireshark) - Wireshark Lua dissector for ports 50000 to 50004 and the DBServer.
- [wireshark-prodj-dissectors](https://github.com/nudge/wireshark-prodj-dissectors) - Another set of Wireshark dissectors.
- [opus-quad-pro-dj-link-analysis](https://github.com/kyleawayan/opus-quad-pro-dj-link-analysis) - What the OPUS-QUAD sends on DJ Link.

## 3D printing

Stands, covers, knobs and cases. Nothing verified yet: if you have a model (Printables, MakerWorld, Thingiverse or a
repo), please add it.

## Other

Out-there possibilities.

- [Sampler-DJS-500](https://github.com/djgreeb/Sampler-DJS-500) - DIY PRO DJ LINK sampler in the nexus style on an STM32F746G-DISCO with Akai LPD8 pads: master-deck BPM and beat sync, quantised triggers, WAV samples from SD, CNC case files.
- [CDJ-1000mk3_new_life_project](https://github.com/djgreeb/CDJ-1000mk3_new_life_project) - Revives a CDJ-1000mk3 with a dead drive: an STM32F746G-DISCO plays from micro SD with a CDJ-2000NXS-style screen, driven by the original controls.
- [XDJ-X](https://github.com/djgreeb/XDJ-X) - Home-built two-channel all-in-one DJ system from CDJ-1000mk3 parts: VFD jog displays, DJM-900NXS-style mixer, optical crossfader, battery, rekordbox playlists from SD; own schematics and PCB.
- [OneLibraryCompanion](https://github.com/hdelplan/OneLibraryCompanion) - Plays music on older CDJs from a Mac or Raspberry Pi.
- [XDJ100SX](https://github.com/marcmonka/XDJ100SX) - Standalone open-source deck built from an old CDJ-100S.
- [CDJ-100S-STM32F7-Display](https://github.com/spectran/CDJ-100S-STM32F7-Display) - STM32F746-Discovery board project for the CDJ-100S, with SD playback.
- [ESPDJ-3000](https://github.com/johnnyclem/ESPDJ-3000) - CDJ-3000 look-alike on an ESP32 with a 1.28" round display.

## See also

- [awesome-dj-producer](https://github.com/classcompliant/awesome-dj-producer) - Curated tools for nerdy DJs and producers; links an early DJS-1000 hack write-up.

## Contributing

Suggestions and edits welcome by issue or pull request, including new sections. One line per project: name, link,
what it does, licence if stated. Public projects only; no firmware, keys or vendor files.

## License

[CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/): to the extent possible, the list is in the public domain.
