# Vault Structure

本 Skill 不要求固定目录树。一个可工作的 Vault 只需要能区分几种语义：临时收录、输入、产出、项目状态、综合理解、AI 导航。

可以参考：

```text
00 Inbox/
10 Projects/
20 Knowledge/
30 Sources/
40 Outputs/
AI-NAV.md
AGENTS.md
```

这只是示例，不是标准答案。

## Inbox

用于尚未正式整理的新材料。用户只需要低成本投递文件、链接或备注，AI 再完成正式分类和 metadata。

## Sources / Inputs

保存用户接触过的外部信息及其原始记录。这里首先是 evidence，不自动等于用户观点或稳定知识。

## Outputs

保存用户实际做过的东西。文本优先保存全文；大型项目可以保存 record 和原始位置。AI 实质参与生产时，应保留 provenance 边界。

## Projects

保存当前正在推进的事情、规则、阶段目标和状态。项目最近很活跃，不代表它就是长期身份。

## Knowledge / Corpus Synthesis

这是 AI 长期备忘录的核心层。它保存对一批材料的综合理解，而不是复制原文。优先按 corpus 形成综合，不急着做一份包罗万象的用户画像。

## AI Navigation

给未来 AI / Agent 使用的机器侧入口，说明不同问题应该先读什么、什么时候再下钻 Sources / Outputs、哪些边界不能越过。

如果用户已有成熟 Vault，先映射现有目录到这些职责，只补真正缺失的层，不要为了安装 Skill 强迫重构。
