# 发布指南 / Release Guide

## 日常更新

1. 修改 `shanxi-medical-university-thesis-numeric.csl`
2. 更新 `VERSION`
3. 在 `CHANGELOG.md` 顶部添加新条目
4. 执行 `git add .`
5. 执行 `git commit -m "描述这次修改"`
6. 执行 `git push`

## 发布正式版本

```powershell
git tag v0.1.1
git push origin v0.1.1
```

然后在 GitHub 的 `Releases` 页面：

1. 点击 `Draft a new release`
2. 选择刚推送的标签
3. 标题使用同一版本号
4. 粘贴 release 文案
5. 上传 `shanxi-medical-university-thesis-numeric.csl` 作为附件

## 版本号建议

- `0.1.1`：小修，如标点、空格或单一类型修正
- `0.2.0`：新增类型支持或明显格式调整
- `1.0.0`：稳定版
