```bash
$ parallel --will-cite "dd count=$((2**20)) < /dev/urandom >& /dev/null && echo" ::: one two three
```
