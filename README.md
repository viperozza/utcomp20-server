# UTComp v20 server package

This repository contains the files needed to install UTComp v20 on an Unreal
Tournament 2004 dedicated server. The UnrealScript source and build tooling are
maintained separately in [viperozza/utcomp2_0](https://github.com/viperozza/utcomp2_0).

## Contents

```text
System/
  UTCompv20.u
  UTCompv20.ucl
examples/
  UT2004.ini.example
  UTCompv20.ini.example
SERVER_INSTALL.md
```

Start with [SERVER_INSTALL.md](SERVER_INSTALL.md). The files under `examples/`
are templates: review them before applying them to a live server, and never
replace a server's complete `UT2004.ini` with the short example fragment.

## Screenshots

### Colored-name editor

![UTComp v20 colored-name editor](assets/colored-name-editor.png)

### UTComp 2.0 settings

![UTComp v20 settings and nickname flag selector](assets/utcomp20-settings.png)

### Scoreboard and weapon statistics

![UTComp v20 scoreboard, weapon statistics, pickups, and spectators](assets/scoreboard-and-stats.png)

## License

UTComp v20 is distributed under the GNU General Public License v3.0. See
[LICENSE](LICENSE).
