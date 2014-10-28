1. 新建repo
- - - - - -
  1. 把reveal.js的[源代码](https://github.com/hakimel/reveal.js)克隆到本地  
  1. 删除.git文件，清除历史  
  2. 新建远程库  
``` bash
  git clone https://github.com/hakimel/reveal.js  
  cd reveal.js
  rm -Rf .git 
  curl -u "$username:$token" https://api.github.com/user/repos -d '{"name":"'$repo_name'"}' 
  # create the remote repo. [More information](http://blog.csdn.net/zl4546474849l/article/details/37497085) of creating remote repo purely by codes. 
```



1. 上传本地库，新建gh-pages分支  
- - - - - - - 
  1. 基本操作，不解释  
  2. 新建gh-pages分支，合并分支（此步骤及以后步骤均可在浏览器实现）
```
    git remote add origin https://github.com/$username/$repo_name.git
    git add .
    git commit -m "Initial commit"
    git push origin master
    git checkout gh-pages
    git merge master
    git push origin master
```



1. 查看，修改
- - - - - - - - - 
  1. 直接在浏览器输入 [github_username].github.io/[repo_name]， 或者点击repo的设置可找到此链接。
  1. 只有gh-pages分支修改才生效

