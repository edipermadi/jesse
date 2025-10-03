## sed substitution

### Replace First Occurence

Replace old with new, separator can be anything as long as it's not in the matching pattern.

```bash
echo "old" | sed 's/old/new/'
sed 's/old/new/' file.txt
```

### Replace n Occurences

```bash
echo "hello world, hello friend" | sed 's/hello/hola/2'
```