# 发布指南 / Release Guide

每次发布新版本时，按这个清单执行。

Use this checklist whenever you publish a new version.

## 1. 修改样式 / Edit the Style

- 更新 `shanxi-medical-university-thesis-numeric.csl`
- 用几条真实文献在 Zotero 中做测试

- Update `shanxi-medical-university-thesis-numeric.csl`
- Test the result in Zotero with a few real items

## 2. 更新版本文件 / Update Version Files

- 修改 `VERSION`
- 在 `CHANGELOG.md` 顶部新增一个版本条目

- Change `VERSION`
- Add a new section at the top of `CHANGELOG.md`

建议版本号 / Suggested versioning:

- `0.1.1`: 小修，如标点、空格或单一类型修正 / small fixes such as punctuation, spacing, or one item type
- `0.2.0`: 新增类型支持或明显格式调整 / new supported item types or a visible formatting rule change
- `1.0.0`: 稳定版，可供他人长期使用 / stable release you want others to depend on

## 3. 提交并打标签 / Commit and Tag

```powershell
git add .
git commit -m "Describe the change"
git tag v0.1.1
git push
git push origin v0.1.1
```

## 4. 创建 GitHub Release / Create a GitHub Release

在 GitHub 上：

1. 打开仓库
2. 进入 `Releases`
3. 点击 `Draft a new release`
4. 选择标签，比如 `v0.1.1`
5. 标题使用同一版本号
6. 从 `CHANGELOG.md` 复制本次更新要点
7. 上传 `shanxi-medical-university-thesis-numeric.csl` 作为附件

On GitHub:

1. Open the repository
2. Open `Releases`
3. Click `Draft a new release`
4. Select the tag, such as `v0.1.1`
5. Use the same version title
6. Copy the main points from `CHANGELOG.md`
7. Upload `shanxi-medical-university-thesis-numeric.csl` as an asset

## 5. 告诉用户改了什么 / Tell Users What Changed

Release 说明里建议保留这些部分：

- 本次更新 / What changed
- 哪些用户需要更新 / Who should update
- 新的 Zotero 录入约定 / Any new Zotero field-entry rules
- 已知限制 / Known limitations

## 推荐 Release 标题 / Suggested Release Title

- 中文: `v0.1.0 山西医科大学 Zotero 论文参考文献样式`
- English: `v0.1.0 Shanxi Medical University Zotero Thesis Style`

## 推荐 Release 文案模板 / Suggested Release Note Template

```md
## 中文

### 本次更新
- 修正学位论文输出
- 修正专利国别输出

### 建议更新对象
- 文献中包含学位论文或专利的用户

### 说明
- 学位论文导师仍建议填写在 `Editor`

## English

### What changed
- Fixed thesis output
- Fixed patent country output

### Who should update
- Users with thesis or patent references

### Notes
- Thesis advisor should still be stored in `Editor`
```
