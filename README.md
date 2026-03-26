# 山西医科大学 Zotero 论文参考文献样式

English name: `Shanxi Medical University Zotero Thesis Style`

这是一个适用于山西医科大学学位论文参考文献格式的 Zotero CSL 样式，采用顺序编码制，参考文献表形如 `[1]`。

## 仓库信息

- GitHub 仓库名：`zotero-shanxi-medical-university-thesis-style`
- 样式文件：`shanxi-medical-university-thesis-numeric.csl`
- Zotero 样式显示名：`Shanxi Medical University Thesis Numeric / 山西医科大学学位论文参考文献样式`

## 安装方法

1. 下载 `shanxi-medical-university-thesis-numeric.csl`。
2. 打开 Zotero。
3. 进入 `Edit -> Preferences -> Cite -> Styles`。
4. 点击 `+`。
5. 选择 `shanxi-medical-university-thesis-numeric.csl`。
6. 在 Word 或 LibreOffice 中打开 `Document Preferences`，切换到这个样式。

## 支持的文献类型

- 著作 `[M]`
- 期刊论文 `[J]`
- 电子文献 `[EB/OL]`
- 报纸文章 `[N]`
- 学位论文 `[硕士学位论文]`、`[博士学位论文]`
- 专利 `[P]`
- 技术标准
- 会议论文 `[A] ... [C]`

## Zotero 录入约定

- 学位论文导师：填在 `Editor`
- 学位论文类型：在 `Type` 中填写 `硕士学位论文` 或 `博士学位论文`
- 图书或学位论文页码：优先使用 `Page`，必要时在 `Extra` 中写 `Page: 56-60`
- 专利国别：使用 `Jurisdiction`，必要时在 `Extra` 中写 `Jurisdiction: 中国`
- 技术标准代号：填在 `Number`

## 当前格式行为

- 参考文献表采用 `[1]` 这类数字编号
- 参考文献表输出全部作者，不使用 `et al.`
- 正文引用当前为普通方括号编号，不是上标
- 字体、行距、悬挂缩进和段落间距仍需在 Word 中设置

## English Summary

This repository contains a Zotero CSL style for the Shanxi Medical University thesis bibliography format. It uses a numeric bibliography style such as `[1]` and supports books, journal articles, web pages, newspaper articles, theses, patents, standards, and conference papers.

## 维护说明

版本记录见 `CHANGELOG.md`，发布流程见 `RELEASE.md`。

## 许可证

本样式按 `CC BY-SA 3.0` 分发，详见 `LICENSE`。
