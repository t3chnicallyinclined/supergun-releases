# SUPERGUN releases

Signed downloads of **SUPERGUN** for Windows. This repository holds release files and notes only.
It contains no source code and no game data.

SUPERGUN runs the copy of **Marvel vs. Capcom 2** you already own on Steam, with rollback netcode.
It does not include the game, and you need to own it on Steam to play.

- Website: https://supergun.io
- Report a problem: https://discord.gg/MVjBwkrZdF

## Download

The current build is served at **https://supergun.io/sg_runner.exe**. Download it, put it anywhere,
and double-click it. Once installed, SUPERGUN updates itself.

The release on this repository's Releases page is an older beta (0.3.2) and is kept for reference.
Use supergun.io for the current version.

### If Windows stops you

- **"Windows protected your PC"**: click **More info**, then **Run anyway**. The beta is not signed
  with a paid publisher certificate yet, so Windows does not recognise the publisher.
- **"These files can't be opened"**, with only a Close button: right-click `sg_runner.exe`, choose
  **Properties**, tick **Unblock**, then **OK**. If the file is in a OneDrive folder, move it to a
  plain folder first.

## Verifying a download

Every release is signed with minisign. The signature file is `sg_runner.exe.sig`, so name it with `-x`. SUPERGUN checks this signature itself before it applies an
update. To check a download by hand:

```
minisign -Vm sg_runner.exe -x sg_runner.exe.sig -P RWR25lWcqd3e/Dt+8P3rdfoQrHK2qx8d5ldFpzXDlaiIqQkkXu6akRVX
```

Each release lists the file's SHA-256 so you can compare it with what supergun.io serves.
