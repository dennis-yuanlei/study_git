1. 重命名本地仓库 git branch -m oldname newname
2. 将文件添加到暂存区 git add xxx xxx xxx ...
3. 将暂存区的修改提交 git commit -m "xxxxxx"
4. 查看最近3条修改记录(会显示commit id和commit信息) git log; git reflog显示全部
5. 回退到当前版本的上一个版本 git reset --hard HEAD^
6. 回退到指定commit id版本 git reset --hard commit_id
7. 撤销工作区的修改 git checkout -- test.md
8. 删除文件,先在工作区中删除, 然后 git rm test.md; git commit; 想取消删除可以使用 git checkout --
9. 重命名分支 git branch -M newname
10. 与远程仓库关联, 鼠标在github创建仓库，根据指示push所有即可, git remote add origin https:...; git push -u origin main
11. 关联后，只要本地commit后, git push origin main即可push到远程仓库(orgin代指远程主机名，main是分支名)
12. 查看远程库代号(一般为origin) git remote -v
13. 解除本地库与远程库的关联 git remote rm origin
14. 创建分支git checkout dev; 创建并切换分支 git checkout -b dev
15. 查看当前分支 git branch
16. 将dev分支合并到master分支->将master指针指向dev分支 git checkout master, git merge dev
17. 删除dev分支 git branch -d dev
18. 查看分支合并图 git log --graph
