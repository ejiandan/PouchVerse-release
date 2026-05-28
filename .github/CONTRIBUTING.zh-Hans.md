# 贡献指南 · PouchVerse

感谢您有兴趣改进 PouchVerse 的文档和翻译！

> For the English contributing guide, see [CONTRIBUTING.md](CONTRIBUTING.md).

---

## 可以贡献什么

这是 PouchVerse 的**公开发布仓库**，包含文档、翻译、法律文件、用户手册和应用截图。欢迎以下类型的贡献：

- **文档修正** — 错别字、失效链接、格式问题
- **翻译改进** — 纠错或使译文更加地道自然
- **新增翻译** — 如果您希望添加尚未支持的语言
- **截图更新** — 如果您有更新或更高质量的素材

> **应用源代码**不在此仓库中。如需提交功能建议或应用 Bug，请[提交 Issue](https://github.com/ejiandan/PouchVerse-release/issues/new/choose)。

---

## 开始贡献

1. **Fork** 本仓库
2. **Clone** 您的 Fork 到本地
3. 为您的更改创建新**分支**：
   ```
   git checkout -b fix/readme-zh-Hans-typo
   ```
4. 进行修改
5. 使用清晰的消息**提交**（见下方规范）
6. **推送**到您的 Fork 并创建 **Pull Request**

---

## 提交信息规范

使用轻量级规范：

```
<类型>(<范围>): <简短描述>
```

| 类型     | 适用场景                           |
|----------|------------------------------------|
| `fix`    | 修复错别字、失效链接或错误信息     |
| `feat`   | 添加新内容（如新翻译文件）         |
| `chore`  | 资源更新、元数据变更               |
| `docs`   | 改善文档结构或清晰度               |

**示例：**
```
fix(zh-Hans): 修正 Quick-Start 中的误译段落
feat(fr): 添加法语版 README 翻译
chore: 更新 iPhone 截图（iOS 18 版本）
```

---

## 翻译规范

- 翻译**含义**，而非逐字直译
- 使用目标语言自然地道的表达方式
- 保留**技术术语**（如 SHA-256、LAN、Face ID），除非目标语言有广泛接受的等效词汇
- 保留所有 **Markdown 格式**（加粗、链接、标题、表格）
- 与英文原版（`README.md`）保持**相同的标题结构**

### 支持的语言

| 语言         | 文件后缀       |
|--------------|----------------|
| 英语         | （无后缀）     |
| 简体中文     | `.zh-Hans`     |
| 繁体中文     | `.zh-Hant`     |
| 日语         | `.ja`          |
| 韩语         | `.ko`          |
| 西班牙语     | `.es`          |

---

## Pull Request 检查清单

提交 PR 前，请确认：

- [ ] 更改仅限于所描述的范围
- [ ] 已检查拼写和语法
- [ ] 更改文件中的所有链接均有效
- [ ] Markdown 可正常渲染（使用 GitHub 预览）
- [ ] 若为翻译：含义与英文原文一致

---

## 有问题？

一般问题请在[讨论区](https://github.com/ejiandan/PouchVerse-release/discussions)提出，具体问题请[提交 Issue](https://github.com/ejiandan/PouchVerse-release/issues)。
