1. 重命名本地仓库 git branch -m oldname newname
2. 将文件添加到暂存区 git add xxx xxx xxx ...
3. 将暂存区的修改提交 git commit -m "xxxxxx"
4. 查看最近3条修改记录(会显示commit id和commit信息) git log; git reflog显示全部
5. 回退到当前版本的上一个版本 git reset --hard HEAD^
6. 回退到指定commit id版本 git reset --hard commit_id
7. 撤销工作区的修改 git checkout -- test.md
8. 删除文件,先在工作区中删除, 然后 git rm test.md; git commit; 想取消删除可以使用 git checkout --
9. 重命名分支 git branch -M newname
10. 与远程仓库关联, 鼠标在github创建仓库，根据指示push即可, git remote add origin https:...; git push -u origin main
