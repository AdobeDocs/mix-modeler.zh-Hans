---
title: Mix Modeler工作流
description: 了解Mix Modeler的典型工作流程。
feature: Ingest Data, Plans, Harmonized Data, Models
exl-id: 200ff846-5d78-4b25-a425-bfd558b88c88
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Mix Modeler工作流

请观看本视频，了解Mix Modeler中的用户工作流简介。

>[!VIDEO](https://video.tv.adobe.com/v/3424854/?learn=on)


Mix Modeler中的典型工作流包含以下活动：

![替换文本](/help/assets//ApplicationWorkflow.svg)

|  | 活动 | 描述 |
|---|---|---|
| ![数据](/help/assets//icons/Data.svg){width="100"} | [**引入数据**](../ingest-data/overview.md) | 从Experience Platform(例如Adobe Analytics、Web SDK、其他源)摄取事件数据、从营销渠道（例如电视、封闭花园、电子邮件、自有和经营活动）摄取聚合数据、从客户摄取外部因素数据（例如订阅服务的价格变化）和内部因素数据（例如假日计划）。 |
| ![DataCheck](/help/assets//icons/DataCheck.svg){width="100"} | [**协调数据**](../harmonize-data/overview.md) | 配置映射规则和冲突解决规则以合并在Mix Modeler中衡量和规划营销活动绩效所需的各种营销数据集。 |
| ![FileConfig](/help/assets//icons/FileGear.svg){width="100"} | [**配置模型**](../models/create.md) | 使用营销接触点（例如渠道）、转化定义以及内部和外部因素配置模型实例。 |
| ![文件数据](/help/assets//icons/FileData.svg){width="100"} | [**训练模型并为其评分**](../models/overview.md) | 使用机器学习训练和评分创建聚合分数和事件级分数。 |
| ![文件图表](/help/assets//icons/FileChart.svg){width="100"} | [**创建计划**](../plans/overview.md) | 利用Mix Modeler模型的输出结果确定营销资金的最佳分配，以实现业务目标。 |
| ![仪表板](/help/assets//icons/Dashboard.svg){width="100"} | [**概述仪表板**](../dashboard/overview.md) | 使用各种可配置的构件深入了解协调的数据、模型和计划。 |

{style="table-layout:auto"}

以下面向数据的详细流程图说明了以下步骤：

* 统一数据基于：

   * 体验事件数据(源自Analytics源连接器，通过Experience PlatformSDK和API收集，通过源连接器摄取，或使用流式摄取)，
   * 聚合或摘要来自封闭式花园(如Facebook、YouTube)、流量源或离线广告数据，以及
   * 协调字段和数据集规则的定义。

* 模型基于：

   * 由协调的数据和市场推广数据产生的转换和营销接触点定义
   * 包含内部或外部因素的非营销汇总或汇总数据。

* 多接触点归因事件得分可以潜在地反馈到Experience Platform数据湖中，用于后续模型配置、训练和评分。

![全面的工作流程](/help/assets//comprehensive-workflow.svg)
