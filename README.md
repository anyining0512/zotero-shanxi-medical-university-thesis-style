# 山西医科大学 Zotero 论文参考文献样式 / Shanxi Medical University Zotero Thesis Style

本仓库提供一个适用于山西医科大学论文参考文献格式的 Zotero CSL 样式，采用顺序编码制，参考文献表形如 `[1]`。

This repository provides a Zotero CSL style for the Shanxi Medical University thesis bibliography format. It uses a numeric bibliography style with entries such as `[1]`.

## 仓库与样式命名 / Repository and Style Names

- 中文显示名: `山西医科大学 Zotero 论文参考文献样式`
- English display name: `Shanxi Medical University Zotero Thesis Style`
- 推荐 GitHub 仓库名 / Recommended GitHub repository name: `zotero-shanxi-medical-university-thesis-style`
- 样式文件 / Style file: `shanxi-medical-university-thesis-numeric.csl`

## 文件说明 / Included Files

- `shanxi-medical-university-thesis-numeric.csl`: 可安装的 Zotero 样式 / installable Zotero style
- `VERSION`: 当前版本号 / current release version
- `CHANGELOG.md`: 更新记录 / version history
- `RELEASE.md`: 发布与更新流程 / release and GitHub update steps

## 安装方法 / Install in Zotero

1. 下载 `shanxi-medical-university-thesis-numeric.csl`。
2. 打开 Zotero。
3. 进入 `Edit -> Preferences -> Cite -> Styles`。
4. 点击 `+`。
5. 选择 `shanxi-medical-university-thesis-numeric.csl`。
6. 在 Word 或 LibreOffice 中打开 `Document Preferences`，切换到这个样式。

1. Download `shanxi-medical-university-thesis-numeric.csl`.
2. Open Zotero.
3. Go to `Edit -> Preferences -> Cite -> Styles`.
4. Click `+`.
5. Select `shanxi-medical-university-thesis-numeric.csl`.
6. In Word or LibreOffice, open `Document Preferences` and switch to this style.

## 支持的文献类型 / Supported Reference Types

- 著作 / Book `[M]`
- 期刊论文 / Journal article `[J]`
- 电子文献 / Web page or electronic resource `[EB/OL]`
- 报纸文章 / Newspaper article `[N]`
- 学位论文 / Thesis `[硕士学位论文]` or `[博士学位论文]`
- 专利 / Patent `[P]`
- 技术标准 / Standard
- 会议论文 / Conference paper `[A] ... [C]`

## 录入约定 / Important Data-Entry Rules

这些约定很重要，因为 Zotero 默认字段与学校格式并不完全一一对应。

These conventions matter because Zotero fields do not fully match the school rules.

- 学位论文导师 / Thesis advisor: 填在 `Editor` / store in `Editor`
- 学位论文类型 / Thesis type: 在 `Type` 中填写 `硕士学位论文` 或 `博士学位论文` / put `硕士学位论文` or `博士学位论文` in `Type`
- 图书或学位论文页码 / Book or thesis page range: 优先使用 `Page`，必要时在 `Extra` 中写 `Page: 56-60` / use `Page`, or `Extra` with `Page: 56-60`
- 专利国别 / Patent country: 使用 `Jurisdiction`，必要时在 `Extra` 中写 `Jurisdiction: 中国` / use `Jurisdiction`, or `Extra` with `Jurisdiction: 中国`
- 技术标准代号 / Standard number: 填在 `Number` / use `Number`

## 当前格式行为 / Current Formatting Behavior

- 参考文献表采用 `[1]` 这类数字编号 / bibliography uses numeric labels like `[1]`
- 参考文献表输出全部作者，不使用 `et al.` / bibliography prints all authors instead of `et al.`
- 正文引用当前为普通方括号编号，不是上标 / in-text citations currently render as normal bracketed numbers, not superscript
- 字体、行距、悬挂缩进和段落间距仍需在 Word 中设置 / Word font, line spacing, hanging indent, and paragraph spacing are still controlled in Word

## 上传到 GitHub / Publish to GitHub

建议把这个目录作为单独仓库发布，不要把整个 `Playground` 目录一起上传。

Recommended workflow: publish this folder as a separate repository instead of uploading the whole `Playground` directory.

```powershell
cd C:\Users\anyin\Documents\Playground\zotero-shanxi-medical-university-thesis-style
git init
git add .
git commit -m "Initial release"
git branch -M main
git remote add origin https://github.com/<your-user>/zotero-shanxi-medical-university-thesis-style.git
git push -u origin main
```

## 更新新版本 / Update to a New Version

1. 修改 `.csl` 文件 / edit the `.csl` file.
2. 更新 `VERSION` / update `VERSION`.
3. 在 `CHANGELOG.md` 顶部添加新条目 / add a new entry at the top of `CHANGELOG.md`.
4. 提交修改 / commit the changes.
5. 创建并推送标签 / create and push a tag.
6. 在 GitHub 上发布 Release / draft a GitHub Release.

示例 / Example:

```powershell
git add .
git commit -m "Fix thesis and patent formatting"
git tag v0.1.1
git push
git push origin v0.1.1
```

详细步骤见 / More detail: `RELEASE.md`.

## 许可证 / License

本样式按 `CC BY-SA 3.0` 分发，详见 `LICENSE`。

This style is distributed under `CC BY-SA 3.0`. See `LICENSE`.
