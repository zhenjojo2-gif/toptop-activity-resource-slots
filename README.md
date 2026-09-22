# TOPTOP 活动资源位制作 Skill

用于 Codex，在 Figma 中制作与验收 TOPTOP 运营活动资源位。

支持两种模式：

- **模板适配**：复制现成模板，按需求与翻译 key 完成多国家、多语言适配。
- **主视觉延展＋自主排版**：通过 Chrome「Kivi 画布快生成」插件延展活动主视觉，再在 Figma 中独立排版文字、标题和奖励。

## 在 Codex 中安装

将下面这段话复制到 Codex：

```text
请使用 skill-installer 安装这个 Skill：
https://github.com/zhenjojo2-gif/toptop-activity-resource-slots/tree/main/skills/toptop-activity-resource-slots
```

安装后在下一轮对话中使用 `$toptop-activity-resource-slots`。

## 使用示例

```text
使用 $toptop-activity-resource-slots，按模板适配制作。
设计稿：[本次 Figma 链接]
需求文档：[本次需求链接]
翻译文档：[本次翻译链接]
保留原模板，在独立输出页面制作各国家资源位。
```

```text
使用 $toptop-activity-resource-slots，按主视觉延展＋自主排版制作。
主视觉设计稿：[本次 Figma 链接]
需求文档：[本次需求链接]
翻译文档：[本次翻译链接]
通过 Chrome 的 Kivi 画布快生成插件，为本活动新建无限画布制作素材。
```

## 使用条件

- Codex 可读取本次需求和翻译资料，并通过 Figma 能力读取、编辑目标文件。
- 需要访问 Skill 引用的固定视觉规范。公开仓库不会改变 Figma 或业务资料的访问权限。
- 主视觉延展模式需要可用的 Chrome「Kivi 画布快生成」插件与 Kivi 登录。默认模型为 GPT image2.5，每批生成4张候选；执行时核对平台实际能力。
- 本仓库包含通用技能，不含具体活动的设计素材、翻译表、制作记录或成品。

## 已沉淀规则

普通可缩文案最低16px，特殊字段执行各自规范；居中信息组共用中心线，分栏布局各自对齐；奖励遮挡信息时整体避让；双奖励采用紧凑居中布局。行距和元素间距由每个活动统一确定，不固定跨活动数值。

保留原模板、可编辑文案和独立素材层。按翻译 key 与语言严格匹配，并同时进行结构检查和截图验收。最终交付 Figma。

首页弹窗背景仅需头图、750×825弹窗框及一句合成提示词；增高只延长中段，保持上下装饰比例。以用户修订稿的实际属性更新版式基线。活动时间直接使用需求表“活动时间（本地）”原文，保留年份与各国格式，不自行简写或换算。

同一活动续做复用已核对的数据、素材与版式，只更新变化字段；按模式加载参考文档，批量读取/写入并采用增量验收。Kivi 复用现有参考，按任务状态退避轮询，避免重复上传、重复生成和重复截图。

技能入口：[SKILL.md](skills/toptop-activity-resource-slots/SKILL.md)
