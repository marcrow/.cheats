# Linux File Operation
% linux, file
#platform/linux #target/local #cat/ENUM/UTILS 
## search file in a source path
```bash
find <src_path> -iname <filename> 2>/dev/null
```

## Search files owned by an user
```bash
find / -type f -user $user 2>/dev/null
```


## Search string in file from a source path
```bash
grep -rnw <src_path> -e <search>
```

## Search string in file from a source path with exclusion
```bash
grep --exclude=\*.{<file_type>} -rnw './' -e "DB_passwd"
```

# Linux String Operation
% linux, string
## get line before and after a string
```bash
grep -i -A<nb_before> -B<nb_after> <search>
```

