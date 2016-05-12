```bash
$ cat black.wav | xxd -cols 2 -g 2 -bits -s 44 -l 40 -p
ffff
0000
0200
0000
fdff
0000
0300
ffff
fdff
0200
0200
fdff
ffff
0400
0000
fcff
0000
0300
0000
fdff

```
