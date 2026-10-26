# AoA

维护适用于不同类型项目的个人偏好和通用工作原则，用于初始化项目的 `AGENTS.md`。

原则按 Open Knowledge Format（OKF）组织，以带 YAML frontmatter 的 Markdown 保存。项目中的具体目标、架构约束、操作边界、执行命令和验收方式由各项目补充。

## 目录

- [原则库索引](knowledge/index.md)：OKF bundle 的入口。
- [通用工作原则](knowledge/principles.md)：目的与交付、来源与证据、推进与成本三方面的要求。
- [项目 AGENTS.md 模板](templates/AGENTS.md)：接入原则并填写项目规则。

## 初始化项目

1. 将 `templates/AGENTS.md` 复制为目标项目的 `AGENTS.md`，保留并整合目标项目已有的有效规则。
2. 将 `knowledge/principles.md` 复制到目标项目的 `.agents/principles.md`。
3. 根据项目情况填写模板中的目标、约束、命令和验收方式，移除未填写的占位项。
4. 在目标 Agent 中确认它已实际读取原则文件和项目规则。

复制后的原则是项目内快照。更新本库后，应检查差异并同步到需要更新的项目。若使用共享路径，可修改模板中的读取路径，并确保目标环境可以访问。

OKF 负责内容组织，Agent 的指令入口负责加载。文件链接本身不保证目标 Agent 自动读取或执行规则。

## 维护

通用原则应适用于不同类型项目。仅在特定项目、工具或主机上成立的要求，放在对应项目或环境的规则中。

目前三条原则集中维护；只有在需要独立引用、选择或更新时再拆分。修改时保留必要条件和行为要求，避免加入对当前任务没有帮助的流程。

本库采用 [OKF v0.2 官方规范](https://github.com/GoogleCloudPlatform/open-knowledge-format/blob/main/SPEC.md)。`knowledge/` 是 bundle 根目录，模板和项目说明位于 bundle 之外。

## 许可证

本项目采用 [MIT License](LICENSE)。使用、修改或分发本项目内容时，请保留版权及许可声明。
