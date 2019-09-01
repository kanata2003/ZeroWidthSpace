# ZeroWidthSpace
Unicode steganography tool using zero-width space. Unicodeゼロ幅スペースを利用した情報の隠蔽ツール

## 詳細はこちらを参照(See below for details)
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

# Author

[@kanata2003](https://twitter.com/kanata201612)

# Special thanks

