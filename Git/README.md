```bash
git init
git add .
git commit -m 'description'

git remote rm Alias
git remote add Alias Url

git pull --rebase origin main

git checkout -b gh-pages
git add -f dist
git subtree push --prefix dist origin gh-pages
```

