## git新手操作

> 20180430

- 对于一般repo第一次上传操作

```bash
git init
git add .
git commit -m 'first try'
git remote rm origin
git remote add origin git@github.com:hibetterheyj/XXX_repo.git
git pull origin master 
git push -f origin master
```

- 对于后续操作

```
git add -A
git commit -m 'xxx'
git pull origin master
git push origin master
```
