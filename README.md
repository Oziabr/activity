#### input filter
```sh
cat /tmp/shell-output | sed -E 's/.*^G|^[\[[0-9;]+m//g' | egrep '^[a-z0-9]+@[a-z0-9]+' | cat
```