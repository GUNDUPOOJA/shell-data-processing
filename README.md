## Big Data Shell-data-processing assignment
## Steps to get started with : 
1. Open powershell here as administrator in windows, Create a new subfolder named shell-data-processing using
2. mkdir - Creates a new folder
``` 
mkdir shell-data-processing
```
3. Change directory into your sub folder.
4. ni - Creates a new item.
``` powershell 
ni .gitignore
ni README.md
```
5. ls - lists the items 

## commands used to get the data.
``` bash
curl "
curl "http://shakespeare.mit.edu/romeo_juliet/full.html" -O "data.txt"
```
- The curl command will return the source for that URL - not the displayed page contents. 


## The command you used to find the most common words, sorted.
- tr transforms the file content 
``` tr commands 
tr ' ' '\12' < data.txt | sort 
tr ' ' '\12' < result.txt | sort | uniq -c | sort -nr > result.txt
```

## Resources 
- https://www.markdownguide.org/cheat-sheet/
- https://nwmissouri.instructure.com/courses/36074/discussion_topics/242724
- https://stackoverflow.com/questions/35777319/extract-the-source-of-the-webpage-without-tags-using-bash
- https://www.itprotoday.com/powershell/differences-between-running-powershell-normal-mode-versus-administrator-mode
