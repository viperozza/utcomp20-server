# Install UTComp v20 on a dedicated server

## 1. Install the package files

Copy both files from `System/` into the server's `System` directory:

```text
UTCompv20.u
UTCompv20.ucl
```

For a PhasecoreX Docker server, use the host-side addon directory:

```text
/home/ubuntu/ut2004-data/addons/System/
```

## 2. Create the UTComp configuration

Copy `examples/UTCompv20.ini.example` to the server's configuration directory
as `UTCompv20.ini`, then review the settings.

On a traditional installation the configuration directory is `System/`. On a
PhasecoreX Docker server it is normally:

```text
/home/ubuntu/ut2004-data/config/
```

## 3. Register and enable the mutator

Merge the settings in `examples/UT2004.ini.example` into the server's existing
`UT2004.ini`. Do not replace the full server file with the example fragment.

Activate this mutator class:

```text
UTCompv20.UTCompv20_MutUTComp
```

For PhasecoreX, add it to the `MUTATORS` environment value. Separate multiple
mutators with commas and no spaces.

## 4. Redirect downloads

If clients download packages directly from the game server, keep
`AllowDownloads=True` under `[IpDrv.TcpNetDriver]`. For an HTTP redirect,
compress and publish `UTCompv20.u.uz2` whenever the package is updated.

Every rebuild has a new package identity. Update the server, redirect, and any
manually installed client copies together to avoid version mismatch errors.

## 5. Verify

Restart the server using its normal administration process and check its log.
There should be no `Failed to load 'UTCompv20'` errors. Confirm that the server
browser lists `UTComp v20` and that `mymenu` opens the UTComp menu in game.
