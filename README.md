# dn - Daily notes command line tool

# Usage

`dn` writes a bullet-pointed string to a file with today's date in YYYY-MM-DD format in a `~/dn/` folder.

`dnview` displays those files.

# Example

```
$ dn "The same thing we do every night"
$ dnview
2019-11-01
 * Made dn
2019-11-02
 * The same thing we do every night
$ dnview 2019-11-02
2019-11-02
 * The same thing we do every night

$ dno 1977-10-28 "Saw star wars"
$ dnview
1977-10-28
 * Saw star wars
2019-11-01
 * Made dn
2019-11-02
 * The same thing we do every night
$ dnview 2019-11
2019-11-01
 * Made dn
2019-11-02
 * The same thing we do every night
```

If you want search, my recommendation is that you install a tool like `ripgrep`, which lists filenames and only echoes the relevant lines.

# Setup

```
mkdir ~/dn
cat dn >> ~/.zshrc
```

Replace .zshrc with the config file for your shell of choice!
