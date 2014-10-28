1. 新建repo
===========================
  1. 把reveal.js的[源代码](https://github.com/hakimel/reveal.js)克隆到本地  
  1. 删除.git文件，清除历史  
  
``` bash
    git clone https://github.com/hakimel/reveal.js
    rm -Rf .git 
```

    git remote add origin git@github.com:tikalk-cookbooks/chef_workshop_presentation.git
    git add .
    git commit -m "Initial commit"
    git push origin master
  1. 新建gh-pages分支  
  1. 把gh-pages分支合并到master分支
