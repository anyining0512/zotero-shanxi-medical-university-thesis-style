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

## 更新方法

每次更新时按这个顺序处理：

1. 修改 `shanxi-medical-university-thesis-numeric.csl`
2. 更新 `VERSION`
3. 在 `CHANGELOG.md` 顶部添加新条目
4. 执行 `git add .`
5. 执行 `git commit -m "描述这次修改"`
6. 执行 `git push`

如果要发布正式版本，再额外执行：

```powershell
git tag v0.1.1
git push origin v0.1.1
```

更详细的发布步骤见 `RELEASE.md`。

## 文件说明

- `shanxi-medical-university-thesis-numeric.csl`：可安装的 Zotero 样式
- `VERSION`：当前版本号
- `CHANGELOG.md`：更新记录
- `RELEASE.md`：发布流程说明
- `LICENSE`：许可证

## English Summary

This repository contains a Zotero CSL style for the Shanxi Medical University thesis bibliography format.

- Style file: `shanxi-medical-university-thesis-numeric.csl`
- Citation style: numeric bibliography such as `[1]`
- Supported items: book, journal article, web page, newspaper article, thesis, patent, standard, and conference paper
- Thesis advisor should be stored in `Editor`
- Thesis type should be stored in `Type`
- Patent country should be stored in `Jurisdiction`
- Standard number should be stored in `Number`

See `RELEASE.md` for the release workflow and `CHANGELOG.md` for version history.

## 许可证

本样式按 `CC BY-SA 3.0` 分发，详见 `LICENSE`。
