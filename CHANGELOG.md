# Changelog

## Unreleased

- Support input methods that report an unknown candidate count, including Rime.
- Consume key releases for handled grid keys and ignore repeated Down events while the grid is opening.
- Show a visible marker and row highlight for the selected grid candidate.
- Document Classic UI layout and global arrow-key settings that can conflict with the addon.

## v0.0.3 — 2026-10-07

- 一行候选时，← → 可以选词，空格上屏高亮的词；到本页末尾自动翻页，到第一个或最后一个就停
- 有候选时 ← → 不再在拼音里移动光标

## v0.0.2 — 2026-10-06

- 列宽按字符宽度计算，英文候选不再把后面的列撑歪
- 网格里 `[` `]` 也可以翻页
- 网格间距改成和原生候选框一致（`1. 是`，用全角空格分隔）
- README 加上截图，结构精简

## v0.0.1 — 2026-10-06

首个版本。
- 按 ↓ 把一行候选展开成 4×8 网格，方向键移动，空格/回车/1–8 上屏，PgUp/PgDn/-/= 翻页，Esc 或在第一行按 ↑ 收起
- 网格下方显示页码
- 收起时恢复输入法原来的候选列表（通过代理对象）
- 提供用户目录安装/卸载脚本
