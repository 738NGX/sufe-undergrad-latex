# 上海财经大学本科毕业论文模板

按照上财计算机与人工智能学院Word版毕业论文模板要求格式编写。自编自用。

## 文件说明

- `main.tex` - 主文件
- `cover.tex` - 封面
- `draft.md` - 摘要 / 正文草稿
- `content.tex` - 摘要 / 正文文件
- `appendix.tex` - 附录
- `sample.bib` - 参考文献
- `figures/` - 图片文件夹

## 使用说明

本模板设计上支持 Markdown 写作后一键转换为 LaTeX，保证了写作的便利性。

首先在 `cover.tex` 修改封面展示信息。

摘要与正文的具体的撰写示例参考 `draft.md` 此处不再赘述。

完成写作后直接在模板路径下运行以下指令，即可将草稿自动转换为需要的 tex 文件。

```sh
pandoc draft.md --template=template.tex -o content.tex --biblatex -f markdown-auto_identifiers
```

如有附录编写需求，请在 `appendix.tex` 中编写。如无附录，可以在 `main.tex` 中注释或删除相关部分。