
Yaml- yet another markup language

We'll create notes with metadata

Dataview creates some [metadata](https://blacksmithgu.github.io/obsidian-dataview/annotation/add-metadata/) on its own

Set Show frontmatter to on in the dataview settings

```
yaml syntax:
---
key: value
listkey: [list1value, list2value]
---

```


## Dataview rules

two parts to dataview- tags and querying

```
\```dataview
TABLE | LIST | TASK
\```

```

### List
if you just type list in the query, it'll list every note in your vault


### Table

Tables show with a header.
add a key after table to add a column to the table
```
TABLE author, genre
```

you can rename the column with 'as' like:
```
TABLE author as AUTHOR
```

### Tasks
You need tasks in your vault to use this part of obsidian


# FILTERING

## FROM
 use from to filter 




