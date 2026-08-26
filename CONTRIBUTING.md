# 量潮章程 — 贡献指南

## 目录结构

```
quanttide-bylaw/
├── default/company    → 法人主体章程（quanttide-bylaw-of-business-entity）
├── README.md          → 项目定位与结构
├── AGENTS.md          → Agent 工作指南
├── CHANGELOG.md       → 版本变更记录
└── CONTRIBUTING.md    → 本文件
```

## 内容规范

- 文档用中文
- 章程按法人主体组织：内容在对应子仓库（`quanttide-bylaw-of-*`）内独立维护，本仓库不直接存放内容

## 提交流程

1. 在子模块内提交推送（Conventional Commits）
2. 回到父仓库更新子模块指针，提交推送
3. 新增/移除主体时同步更新 README.md 结构树
4. 变更记录写入 CHANGELOG.md
