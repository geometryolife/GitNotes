# Lazygit 基本使用

## Files panel

- `a` all stage/unstage
- `space` => single stage/unstage file
- Part of the stage file
  - `Enter` => `Unstaged changes`/`Staged changes`
    - `Space` => select lines to stage
    - `d` in `Staged panel` => select lines to unstage
    - `d` in `Unstaged panel` => select lines to delete
    - `a` => 选中整段 hunk
  - `Tab` switch to other panel
  - `Left/Right` => previous/next hunk
  - `Esc`/`C-[` => 返回文件面板
- `A` => 修改上一次提交
- `C` => 使用编辑器编辑提交更改
- `d` => discard changes (丢弃更改)
- `D` => 更多放弃更改的选项
- `s` => 全部隐藏 stash all
- `S` => 隐藏选项 stash options

## Branch panel

- `n` => 新建分支 new branch
- `Space` => 切换分支 checkout
- `P` => 发布 push
- `p` => pull
- `M` => 把选中的分支合并到当前分支
- `[`/`]` => 在面板标签之间跳转
- `d` => 删除分支

## Commits panel

- `d` => delete commit
- `c` => cherry-pack
- `Enter` => 进入某个提交中
  - `c` => checkout file
  - `d` => 丢弃这次提交的更改
  - `Enter` in select => 创建自定义补丁
- `,`/`.` => previous/next page
- `<`/`>` => 顶端/低端 top/bottom
- `/` => 搜索
- `r` => 更改提交信息
- `R` => 在编辑器中更改提交信息，注意如果已经发布出去，需要 force push
- `Space` => 回滚任意提交 checkout commit
- `g` => 回滚提交方式2 view reset options
- 合并操作
  - `s` => squash down 这个操作不会删除 commits 内容，会合到一起
  - `f` => fixup commit 但是这个操作不保留提交信息，常用于补充上一次提交的补充
- `e` => edit commit => `m` 执行选择好的内容，批量操作
  - `p` => `pick` => 什么都不改，保留原来的状态
  - `s` => `squash` => 压缩
  - `f` => `fixup` => 修补
  - `d` => `drop` => 丢弃
  - `m` => `continue`/`abort`/`skip`/`cancel` => 继续（执行）/中断（放弃）/跳过/取消
- `Enter` 进入某个提交 => `Ctrl-s` => filtering => 查看某个文件的所有提交记录
- `W` => 显示 diff 选项 => 可配合上面这个针对某个文件比较

## Reflog

- `g` => reset options


35 minutes interactive rebasing
38 fix conflict

## Fix conflicts

- `Files panel` => `Enter`
- `上/下` => 选择保留哪一次更改
- `左/右` => 冲突间跳转
- `Space` => 选取选中的代码段
- `b` => 两种更改都选择保留
