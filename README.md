# BeePharma — releases

Public Windows release binaries for **BeePharma**, the pharmacy POS by
[BEE Solutions IQ](https://github.com/mustafaeminof), Kirkuk, Iraq.

The source lives in a private repository. This one exists so a pharmacy — and
the app's own auto-updater — can download an installer without a GitHub account.

## Installing

Open [Releases](../../releases) and download
`BeePharma-Setup-<version>.exe`, then run it. It installs into the folder an
existing copy already uses, and leaves the database, backups and licence
untouched.

`BeePharma-Windows-<version>.zip` is the raw build for a machine that cannot run
the installer. It does not install itself — unpack it over the existing folder
by hand.

## `latest.json`

The in-app updater reads this manifest from `raw.githubusercontent.com` and
`cdn.jsdelivr.net` as fallbacks for `api.github.com`, so a pharmacy whose ISP
throttles or blocks the GitHub API still sees new releases. CI rewrites it on
every publish — do not edit it by hand.
