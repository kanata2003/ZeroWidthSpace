# ZeroWidthSpace
Unicode steganography tool using zero-width space. Unicodeゼロ幅スペースを利用した情報の隠蔽ツール

## See below for details(詳細はこちらを参照)
[A painter and a black cat - ZeroWidthSpace](https://raintrees.net/projects/a-painter-and-a-black-cat/wiki/ZeroWidthSpace)

## Easy installation

```bash
$ git clone https://github.com/kanata2003/ZeroWidthSpace
$ cd ZeroWidthSpace
$ chmod u+x zws
$ cp zws /usr/local/bin/zws
```

## Usage

Like base64 command.

### Encode

```bash
$ echo unko > file
$ zws file
'‌⁢‌‌​​‍‍‌‍⁢‍​​‍‍‌‍‍⁢​​‍‍‌‍⁢⁢​​‍‍'
```

or

```bash
$ echo "unko"|zws
'‌⁢‌‌​​‍‍‌‍⁢‍​​‍‍‌‍‍⁢​​‍‍‌‍⁢⁢​​‍‍'
```

### Decode

"this is a pen" included Zero Width Space.

```bash
$ cat file
this is a pen‌⁢‌‌​​‍‍‌‍⁢‍​​‍‍‌‍‍⁢​​‍‍‌‍⁢⁢​​‍‍
$ zws -d file
unko
```

or

```bash
$ echo '‌⁢‌‌​​‍‍‌‍⁢‍​​‍‍‌‍‍⁢​​‍‍‌‍⁢⁢​​‍‍'|zws -d
unko
```

## For Mac

To run on Mac, you need the following software.

* bash ver 4.2 or higher

```
$ which bash
/usr/local/bin/bash
$ bash --version
GNU bash, バージョン 5.0.2(1)-release (x86_64-apple-darwin17.7.0)
Copyright (C) 2019 Free Software Foundation, Inc.
ライセンス GPLv3+: GNU GPL バージョン 3 またはそれ以降 <http://gnu.org/licenses/gpl.html>

This is free software; you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.
```

* gnu-sed

```
$ which sed
/usr/local/opt/gnu-sed/libexec/gnubin/sed
$ sed --version
sed (GNU sed) 4.5
Copyright (C) 2018 Free Software Foundation, Inc.
License GPLv3+: GNU GPL version 3 or later <https://gnu.org/licenses/gpl.html>.
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.

Written by Jay Fenlason, Tom Lord, Ken Pizzini,
and Paolo Bonzini.
GNU sed home page: <https://www.gnu.org/software/sed/>.
General help using GNU software: <https://www.gnu.org/gethelp/>.
E-mail bug reports to: <bug-sed@gnu.org>.
```

# Author

[@kanata2003](https://twitter.com/kanata201612)

# Special thanks

[@qwertanus](https://twitter.com/qwertanus) # Refactoring

[@yoichi22](https://twitter.com/yoichi22)  # Operation check on Mac

