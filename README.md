# git-commands

## To Sort

git log --no-walk --tags --pretty="%H  %cd  %D  %s" --decorate=full > tags.txt

git log --pretty=medium  --no-merges > log.txt

Git - pretty-formats Documentation
https://git-scm.com/docs/pretty-formats

git log --no-walk --tags --pretty="%cd %D" --decorate=full > tags.txt

npm run script
    "changelog": "echo \"# Change Log\" > changelog.md && git log --pretty=\"*%ad* **%s**%n%b%n\"  --no-merges --date=format:\"%d %b %Y\" >> changelog.md"

git log --no-walk --tags --pretty="%D | %cd" --decorate=full --date=format:"%D %b %Y" > tags.md && sed -i '' 's/tag: refs\/tags\///g' tags.md
