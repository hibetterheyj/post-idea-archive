## git新手操作

> 创建于20180430
>
> 最后更新于20180513

- 对于已有文件的repo重新覆盖上传操作

```bash
git init
git add .
git commit -m 'first try'
git remote rm origin
git remote add origin git@github.com:hibetterheyj/XXX_repo.git
git pull origin master 
git push -f origin master
```

- 第一次上传

```
git init
git add .
git commit -m "first commit"
git remote add origin git@github.com:hibetterheyj/Chinese-Podcast-Ideas.git
git push -u origin master
```

- 对于后续操作

```
git add -A
git commit -m 'xxx'
git pull origin master
git push origin master
```
