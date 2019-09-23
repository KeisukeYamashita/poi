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
        
        curl -s "www.google.com" | poi poi --title google_page --tag html,google

    [Restore tmp file: command mode]

        poi find SUM_COMMAND google_page

    [Search file: command mode]

        poi find SUM_COMMAND googl
    
    [Search by tag: command mode]

        poi find SUM_COMMAND html
    
    [Search by file: interactive mode]

        poi find SUM_COMMAND -i

    [Search by tag: interactve mode]

        poi find SUM_COMMAND -i

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

## Author

* KeisukeYamashita
