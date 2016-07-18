# git

## Managing History

### View commit summaries
git log --oneline

### Overlay branch history on commit summaries
git log --oneline --decorate

### See _all_ branches and a graph of unmerged branches
git log --oneline --decorate --graph --all

### Format the log:
git log --pretty-format:'[format]'

### Searching the log (in summaries)
git log -E -i --grep '[regex search]'

### Searching the log (in the code)
git log -S [code]

### View the log of a file
git log --oneline -- [filename]

### See last commit of each line of a file
git blame [filename]

### Show the complete commit information
git show [hash]

## Making Aliases

### Making an alias
git config --global alias.[alias] '[commands]

### Example Aliases

#### "Short log all"
git config --global alias.sla 'log --oneline --decorate --graph --all'

#### "Grep log"
git config --global alias.glog 'log -E -i --grep
