# Git 小抄

## 查看状态与差异

```bash
git status                 # 查看文件处于什么状态
git diff                   # 查看未暂存的改动
git diff --cached          # 查看已暂存的改动
git diff HEAD              # 比较当前文件与最近一次提交
git diff -- 文件名         # 只查看指定文件
```

## 暂存与提交

```bash
git add notes/meeting.md   # 把文件改动放进暂存区
git commit -m "更新会议记录" # 创建一个提交
git log --oneline          # 查看简短提交历史
```

## 看懂 diff 符号

- `-` 表示旧版本中被移除的行。
- `+` 表示新版本中新增的行。
- `@@` 标记变化所在的行号范围。
