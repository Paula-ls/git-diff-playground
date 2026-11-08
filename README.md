# Git Diff 游乐场

欢迎来到一个可以放心折腾的小仓库。这里用几篇 Markdown 文件演示 Git 如何记录变化。

## 建议体验顺序

1. 先看 `git status`，了解工作区和暂存区的状态。
2. 运行 `git diff`，查看尚未暂存的改动。
3. 运行 `git diff --cached`，查看已经暂存、但还没有提交的改动。
4. 运行 `git diff HEAD`，一次比较所有尚未提交的改动。
5. 打开 `git diff -- notes/meeting.md`，只看一篇文件。

这个演示仓库已经有一个基线提交，并预留了一份暂存改动和一份未暂存改动。

## 继续练习

修改任意 Markdown 文件后，再运行 `git diff`。试着暂存其中一份文件：

```bash
git add notes/reading-list.md
git diff --cached
git diff
```

想重新开始时，可以先查看提交记录，再把文件恢复到当前提交状态：

```bash
git log --oneline
git restore .
git restore --staged .
```

注意：恢复操作会丢弃对应的本地改动；练习前可以复制一份仓库。
