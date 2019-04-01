#### 本地创建版本库：

本地初始化git：

```
 git init
```

高速Git把文件或文件夹添加到仓库：

```
git add {filename}
git add {folder}
```

把文件提交到仓库

```
git commit -m {message}
```



#### 把本地仓库内容推送到GitHub仓库：

github上创建一个新的repository，然后：

- 在本地使用命令行创建一个新的仓库：


```
echo "# learn-git" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/ralphchen/learn-git.git
git push -u origin master
```

- 推送（push）一个已经存在的repository 


```
git remote add origin https://github.com/ralphchen/learn-git.git
git push -u origin master
```

- github上已经存在项目，把远程仓库里面的项目拉下来：


```
git pull origin master #将远程仓库里面的项目拉下来
```



#### 删除github上的目录

```
git pull origin master #将远程仓库里面的项目拉下来
dir
git rm -r --cached target # 删除target文件夹
git commit -m "message" #提交并添加操作说明
git push -u origin master
```



#### 添加github上的目录

```
git add 文件夹/  #添加整个文件夹及内容
git add *.文件类型  #添加目录中所有文件类型的文件
```

#### 重命名文件和文件夹
```
git mv -f oldfolder newfolder
git add -u newfolder  #-u 选项会更新已经追踪的文件和文件夹。

```

