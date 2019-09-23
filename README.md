# Poi

Poi is a useful temporary file manager 🍭🗑⚔️

```
$ poi help
Name
    Poi is a useful temporary file manager 🍭 🗑 ⚔️

Synopsis
    poi COMMAND

COMMANDs:
    [Store tmp file]

        curl -s "www.google.com" | poi poi

        [With Title and tags]
        curl -s "www.google.com" | poi poi --title google_page --tag html,google

    [Restore latest file]
    
        poi pui

    [Show latest file path]

        poi where

    [Show file]

        poi cat FILE_ID

    [Show file]

        poi cat --interactive

    [Search file]

        poi ls 

    [Search file]

        poi ls -i 
    
    [Search by file: interactive mode]

        poi ls SUM_COMMAND --interactive

    [Delete(sweep) cache]

        poi sweep
    
    [Delete all files]

        poi clean

    [Show help]

        poi help

```

## Usage

### Store tmp file

Store file.

```
$ cat README.md | poi poi
```

#### Add title and tag

* Use can add title or tag

```
$ cat README.md | poi poi --title cat_readme --tag cat,doc
```

### Show file

#### Show latest store file

`pui` command shows the latest stored file.

```
$ poi pui
```

#### Show tmp file

Show file can be done by the `cat` command.

```
$ poi cat FILE_ID
```

### List file

#### List all files

List all temporary files.

```
$ poi ls
```

### Delete all temporary files

Use `sweep` command for delete all files in tmp.

```
$ poi sweep
```

### Super delete

Sweep commands does not actually deletes your tmp file. It compresses "sweeped" temporary file and store in another file. To delete, use `clear command`

```
$ poi clear
```

## Author

* KeisukeYamashita
