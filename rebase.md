
```
1. 从master检出your分支, 假设名字feat/v1

git checkout -b feat/v1

2. 写代码 && 提交

git add *;  
git commit -m '';   

3. 如果你的开发时间比较长，或者master有线上紧急bug fix。
此时master上会有别人的这些commit。与你分支的commit时间交叉。

4. 你的分支feat/v1开发完毕，需要从master合并 master的最新内容
此时禁止使用Git merge master
使用：git rebase master

最核心的一步！！！！！

5. 你的分支git push origin feat/v1

6. 在gitlab上提pull request（PR）；

7. pr approve后。项目的maintainer会merge你的分支进master。
```

rebase使用注意：只在自己的分支上执行，不要在master分支上执行rebase。