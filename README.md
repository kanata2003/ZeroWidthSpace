# ZeroWidthSpace
Unicode Steganography tool using zero-width space. Unicodeゼロ幅スペースを利用した情報の隠蔽ツール

## 詳細はこちらを参照(See below for details)
[A painter and a black cat - ZeroWidthSpace](https://raintrees.net/projects/a-painter-and-a-black-cat/wiki/ZeroWidthSpace)

## Easy installation

```bash
$ git clone https://github.com/kanata2003/ZeroWidthSpace
$ cd ZeroWidthSpace
$ chmod u+x zws
```

## Usage

### Encode

```bash
$ ./zws unko
'‌⁢‌‌​​‍‍‌‍⁢‍​​‍‍‌‍‍⁢​​‍‍‌‍⁢⁢​​‍‍'
```

or

```bash
$ echo "unko"|./zws
'‌⁢‌‌​​‍‍‌‍⁢‍​​‍‍‌‍‍⁢​​‍‍‌‍⁢⁢​​‍‍'
```

### Decode

"this is a pen" included Zero Width Space.

```bash
$ ./zws -d 'this is a pen‌⁢‌‌​​‍‍‌‍⁢‍​​‍‍‌‍‍⁢​​‍‍‌‍⁢⁢​​‍‍'
unko
```

or

```bash
$ echo '‌⁢‌‌​​‍‍‌‍⁢‍​​‍‍‌‍‍⁢​​‍‍‌‍⁢⁢​​‍‍'|./zws -d
unko
```
