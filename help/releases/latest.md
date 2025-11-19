---
title: 查看当前的Mix Modeler发行说明
description: 最新 Mix Modeler 发行说明
feature-set: Experience Cloud
feature: Release Notes
exl-id: 38a47672-2af2-437c-b769-4d5febb941f5
source-git-commit: 6fc734793102533003c731e22dfe0d8c422a1cde
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 5%

---

# 当前的Mix Modeler发行说明

**上次更新**：2025年11月12日。

以下发行说明涵盖最新版本的Mix Modeler。 Mix Modeler版本在持续交付模型上运行，该模型允许大约每月一次的发布。 因此，这些发行说明将会相应更新，因此请定期检查。



## 2025 年 11 月

| 功能 | 描述 | [转出开始](#release-strategy) | [正式发布](#release-strategy) |
|---|---|---|---|
| **[!UICONTROL Plans tracking]** | 允许用户了解营销计划的执行如何跟踪计划的内容。 这样您就可以对营销效果充满信心。 或者尽早发现机会和风险，以纠正错误并实现业务目标。 已更新[计划可视化图表的性能](/help/dashboard/plans.md#performance-to-plan)，并允许配置量度和粒度。 | 2025年11月12日 | 2025年11月12日 |
| **[!UICONTROL Channel synergy insights]** | 展示营销渠道如何协作以产生更大的影响。 通过这些见解，您可以满怀信心地解释过去的营销绩效并相应地调整营销支出，以最大限度地提高营销投资组合的整体回报。 [模型分析](/help/models/insights.md#channel-synergy)和[计划分析](/help/plans/insights.md#channel-synergies)中提供了渠道协同矩阵。 | 2025年11月12日 | 2025年11月12日 |
| **修复** | 修复了以下票证： <ul><li>AMM-2920：计划创建流程和迁移。</li><li>AMM-3282：大网格中小数字变化的科学记数法。</li></ul> | 2025年11月12日 | 2025年11月12日 |


## 2025 年 9 月

| 功能 | 描述 | [转出开始](#release-strategy) | [正式发布](#release-strategy) |
|---|---|---|---|
| **[!UICONTROL Dataset mapping validations]** | 向Experience Platform数据集映射中添加了针对协调字段的验证。 | 2025年9月9日 | 2025年9月9日 |
| **[!UICONTROL Context menu on links to model and plans]** | 启用指向模型和计划的链接的浏览器上下文菜单。 您现在可以使用该浏览器上下文菜单在新标签或窗口中打开特定计划或模型。 | 2025年9月9日 | 2025年9月9日 |
| **修复** | 修复了以下票证： <ul><li>AMM-3101：修复了为规则创建不正确的映射： `event_date`作为字段名称而非`timestamp`传递。</li><li>AMM-3092：修复了无法更改基于重复预算的计划的渠道最大限制值。</li><li>AM3130：修复了模型的详细信息弹出窗口中错误的&#x200B;**[!UICONTROL Run frequency]**&#x200B;信息。</li><li>AMM3158：在&#x200B;**[!UICONTROL Select target metric]**&#x200B;计划创建&#x200B;**[!UICONTROL Optimize]**&#x200B;接口的[窗格中更新了](/help/plans/build.md)选项的标签。</li><li>AMM 3176：修复了无法在[的](/help/models/insights.md#breakdown)选项卡中查看&#x200B;**[!UICONTROL Attribution]**&#x200B;按渠道&#x200B;**[!UICONTROL Model Insights]**&#x200B;划分可视化图表的问题。</li></ul> | 2025年9月9日 | 2025年9月9日 |
| **修复** | 修复了以下票证： <ul><li>AMM-3174：在没有现有计划可用时改进了体验。</li><li>AMM-3216：增强了对自定义日期范围的验证。</li><li>AMM-3240：固定运行模型频率显示。</ul> | 2025 年 9 月 23 日 | 2025 年 9 月 23 日 |

## 2025 年 7 月 - 8 月

| 功能 | 描述 | [转出开始](#release-strategy) | [正式发布](#release-strategy) |
|---|---|---|---|
| **[!UICONTROL Compare plans update]** | [比较计划](/help/plans/compare.md) UI现在可显示付费营销的其他详细信息：投资回报率(ROI)或CPA，以及收入。 | 2025年8月20日 | 2025年8月20日 |
| **协调更新** | 现在，所有数据集规则都使用类似的[通用映射到协调字段体验](/help/harmonize-data/dataset-rules.md)，无论数据集类型如何。 当您从摘要数据集中映射标准协调字段时，Mix Modeler会尝试自动推导相应的Experience Platform数据集字段。 | 2025年7月29日 | 2025年7月29日 |


## 2025年5月至6月

| 功能 | 描述 | [转出开始](#release-strategy) | [正式发布](#release-strategy) |
|---|---|---|---|
| **基于目标的计划** | 在预算旁边，您可以在[创建](/help/plans/build.md)或[编辑](/help/plans/insights.md#edit-plan)计划时定义目标（目标）。 目标指标的示例包括收入、转化、CPA或ROI。 | 2025年6月18日 | 2025年7月8日 |
| **支出模式配置** | 现在，当您构建计划时，在定义每个预算日期范围的支出模式时，可以选择使用[历史引用](/help/plans/build.md)数据（如过去的营销支出数据和见解）。 | 2025年5月14日 | 2025年5月14日 |
| **高级计划配置** | 您可以为计划定义[高级配置](/help/plans/build.md)，例如每次转换的平均收入和渠道成本。 | 2025年5月14日 | 2025年5月14日 |

## 2025年3月至4月

| 功能 | 描述 | [转出开始](#release-strategy) | [正式发布](#release-strategy) |
|---|---|---|---|
| **模型漂移检测** | 在打开模型时，当检测到模型漂移时，系统会[提示您重新训练模型](/help/models/insights.md#model-drift)。 | 2025年4月3日 | 2025 年 5 月 7 日 |
| **计划分析中的边际渠道回报** | 将[边际渠道回报](/help/plans/insights.md#marginal-channel-return)可视化图表添加到计划分析中，该可视化图表显示所有或选定渠道的边际盈亏平衡图和计划回报。 | 2025年4月3日 | 2025年4月24日 |


## 2025年1月至2月

| 功能 | 描述 | [转出开始](#release-strategy) | [正式发布](#release-strategy) |
|---|---|---|---|
| **嵌套条件** | 在模型[的](/help/models/build.md#configure)配置中定义符合条件的数据群体时，可以使用AND和OR创建嵌套条件。 | 2025年1月15日 | 2025年2月18日 |
| **查看报告** | 您可以查看有关您定义为协调数据一部分的[转化](/help/harmonize-data/conversions.md#view-report)或[营销接触点](/help/harmonize-data/marketing-touchpoints.md#view-report)的报告。 | 2025年1月15日 | 2025年2月18日 |
| **删除确认** | 系统会提示您确认删除[计划](/help/plans/overview.md#delete-plans)或[模型](/help/models/overview.md#delete-models)。 | 2025年1月15日 | 2025年2月18日 |
| **因素UI改进** | 您可以选择要在模型分析中显示的[因子](/help/models/insights.md#factors-beta)。 | 2025年1月15日 | 2025年2月18日 |
| **错误处理** | 便于用户使用的错误消息以及改进的用户体验，在数据协调和计划中出现错误情景。 | 2025年2月18日 | 2025年2月18日 |
| **模型状态** | 在整个模型生命周期中重新定义[模型状态](/help/models/overview.md#manage-models)。 | 2025年2月18日 | 2025年2月18日 |


## 发布策略

[!UICONTROL Mix Modeler]使用功能标志（也称为“切换”）控制新功能的可见性，从而允许在完全发布之前进行受控规模测试。 此发布策略包括以下阶段：

* **有限测试**：从Adobe内部用户的测试开始的分阶段发布。 然后，它提供给一小部分客户使用，以确保该功能满足客户的需求和期望。

* **开始推出**：分阶段发布的推出从有限测试阶段开始。 然后，此发布在两个月内从0%到100%提供给客户。 由于分阶段推出在Experience Cloud组织级别进行，因此组织中所有授权用户都将获得相同的体验。
