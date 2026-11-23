# Centtrix packages

Package index for Centtrix OS. The built-in command `cenpkg` reads
`index.txt` and downloads package files from `pkgs/`.

    cenpkg list
    cenpkg install hello
    cenpkg install testland
    run /base/pkg/hello.xep

`index.txt` has one package per line: `NAME    DESCRIPTION`.
The file for a package is `pkgs/NAME.xep` (an XPL script), or a native
program ending in `.c` / `.rs` (C / Rust). `testland.rs` is the tiling
session package: after installing it, `testland main` makes it the desktop
that starts after login.

Native programs live under `/home/pkg` once installed and run with:

    run /home/pkg/hello.c
    run /home/pkg/hello.rs
