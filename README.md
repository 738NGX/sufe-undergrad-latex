# 上海财经大学本科毕业论文模板

自编自用。

## 文件说明

- `main.tex` - 主文件
- `cover.tex` - 封面
- `abstract-cn.tex` / `abstract-en.tex` - 中英文摘要
- `content.tex` - 正文文件
- `draft.md` - 正文草稿
- `sample.bib` - 参考文献
- `figures/` - 图片文件夹

## 如何将草稿转换为正文？

作者喜欢使用 Markdown 编写论文草稿。写完后直接在模板路径下执行以下命令：

```sh
pandoc draft.md --template=template.tex -o content.tex --biblatex -f markdown-auto_identifiers
```

即可自动将正文草稿编译成正文文本。从而免去了手写 latex 的麻烦。