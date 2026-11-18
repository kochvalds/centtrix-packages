# Centtrix packages

Package index for Centtrix OS. The built-in command `cenpkg` reads
`index.txt` and downloads package files from `pkgs/`.

    cenpkg list
    cenpkg install hello
    run /base/pkg/hello.xep

`index.txt` has one package per line: `NAME    DESCRIPTION`.
The file for a package is `pkgs/NAME.xep` (an XPL script).
