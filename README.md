# 量潮章程

## 仓库定位

量潮章程（quanttide-bylaw）是量潮知识管理体系中的**章程聚合容器**——按主体与领域聚合各章程子仓库（git submodule）。每个子仓库独立维护，本仓库只追踪引用。

在量潮"正交分解"中，本仓库横跨**主体轴（Who it is）与领域轴（What it expresses）**：`default/` 聚合各法人主体章程，`domains/` 聚合各领域章程，回答"我们依据什么规则运行"。

## 仓库结构

```
quanttide-bylaw/
├── default/company      → 法人主体章程（quanttide-bylaw-of-business-entity）
├── domains/             → 领域章程子仓库（git submodule）
│   ├── asset            → 资产管理章程（quanttide-bylaw-of-asset-management）
│   ├── data             → 数据工程章程（quanttide-bylaw-of-data-engineering）
│   ├── delib            → 议事管理章程（quanttide-bylaw-of-deliberation-management）
│   ├── docs             → 文档工程章程（quanttide-bylaw-of-document-engineering）
│   ├── devops           → DevOps 工程章程（quanttide-bylaw-of-devops）
│   ├── human            → 人力资源章程（quanttide-bylaw-of-human-resources）
│   ├── meta             → 元工程章程（quanttide-bylaw-of-philosophy）
│   └── product          → 产品研发章程（quanttide-bylaw-of-product-development）
├── README.md            → 本文件
├── AGENTS.md            → Agent 工作指南
├── CHANGELOG.md         → 版本变更记录
├── CONTRIBUTING.md      → 贡献指南
├── ROADMAP.md           → 路线图
└── LICENSE              → 许可证
```

## 子模块管理

- 子模块独立提交推送，本仓库只更新引用指针
- 新增章程仓库：`git submodule add <url> default/<path>`（主体章程）或 `domains/<path>`（领域章程）
- 同步全部子模块：`git submodule update --init --recursive`

## 关联

- 章程与档案、日志同源：`assets/quanttide-profile`（工作档案聚合）、`assets/quanttide-journal`（工作日志聚合）
- 主仓库：`quanttide` 根仓库 `default/quanttide-tech` 文档站链接各法人主体章程
