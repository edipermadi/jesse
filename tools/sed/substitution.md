## sed substitution

### Replace First Occurence

Replace old with new, separator can be anything as long as it's not in the matching pattern.

```bash
# sed from file
sed 's/old/new/' file.txt

# sed literal
echo "old" | sed 's/old/new/'

# sed via pipe
cat file.txt | sed 's/old/new/'

# sed via stdin
sed 's/old/new/' < file.txt
```

### Replace Second Occurences

```bash
echo "hello world, hello friend" | sed 's/hello/hola/2'
```

### Replace All Occurences

```bash
echo "hello world, hello friend" | sed 's/hello/hola/g'
```