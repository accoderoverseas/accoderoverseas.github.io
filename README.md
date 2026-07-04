# accoderoverseas.github.io

OAVO 每日一题 · 北美 / 澳洲 OA·VO 真题讲解站点。基于 [GitHub Pages](https://pages.github.com/) + [just-the-docs](https://just-the-docs.com/) 主题，云端自动构建。

网站地址：https://accoderoverseas.github.io

## 目录结构

```
_config.yml            站点配置（主题、搜索、辅助链接）
index.md               首页
companies.md           “按公司刷题”栏目页
companies/<公司>/       每个公司一个目录，index.md 为公司页，其余为题解
knowledge-points.md    知识点索引
contact.md             联系方式
```

## 新增一篇题解

1. 在 `companies/<公司>/` 下新建 `xxx.md`；
2. 顶部加 front matter（`title` / `parent` / `grand_parent: 按公司刷题` / `nav_order`）；
3. `git add . && git commit && git push`，GitHub 自动重建，约 1–2 分钟生效。

## 本地预览（可选）

```bash
bundle install
bundle exec jekyll serve   # 打开 http://localhost:4000
```
