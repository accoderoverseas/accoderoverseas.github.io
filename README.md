# accoderoverseas.github.io

码上出海 Coding Overseas · 求职 OA/VO 真题讲解 × 留学生 CS 课程辅导站点。基于 [GitHub Pages](https://pages.github.com/) + [just-the-docs](https://just-the-docs.com/) 主题，云端自动构建。

网站地址：https://accoderoverseas.github.io

## 目录结构

```
_config.yml            站点配置（主题、搜索、辅助链接）
index.md               首页
daily.md               “算法每日一题”栏目页（左侧可展开）
daily/<日期-题名>.md    每篇每日一题（front matter 里 parent: 算法每日一题）
companies.md           “求职找工OA/VO真题拆解”栏目页（permalink 仍为 /companies/）
companies/<公司>/       每个公司一个目录，index.md 为公司页，其余为题解
knowledge-points.md    “算法数据结构知识点速查”（parent: 求职找工OA/VO真题拆解，permalink /knowledge-points/）
cs-courses.md          “留学生CS课程”栏目页
cs-courses/            子目录：cheatsheet.md（CS课程速查）、course-map.md（学校课程图谱）
contact.md             联系方式
```

## 新增一篇题解（按公司）

1. 在 `companies/<公司>/` 下新建 `xxx.md`；
2. 顶部加 front matter（`title` / `parent` / `grand_parent: 求职找工OA/VO真题拆解` / `nav_order`）；
3. `git add . && git commit && git push`，GitHub 自动重建，约 1–2 分钟生效。

## 新增一篇每日一题

1. 在 `daily/` 下新建 `YYYY-MM-DD-题名.md`；
2. 顶部加 front matter：
   ```yaml
   ---
   title: 2026-07-05 · 题名
   parent: 算法每日一题
   nav_order: 20260705   # 用日期 YYYYMMDD，父页设了 child_nav_order: reversed，最新日期自动排最前
   ---
   ```
3. `git add . && git commit && git push`，左侧「算法每日一题」展开即可看到新题。

## 本地预览（可选）

```bash
bundle install
bundle exec jekyll serve   # 打开 http://localhost:4000
```
