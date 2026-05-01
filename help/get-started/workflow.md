---
title: Mix Modeler工作流程
description: 了解Mix Modeler的典型工作流程。
feature: Ingest Data, Plans, Harmonized Data, Models
exl-id: 200ff846-5d78-4b25-a425-bfd558b88c88
TQID: https://experienceleague.adobe.com/PAKsHAqpIeBVCJGIPS2ZqWw-vVpS9LUpYdJRFKP0ynY
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
feature_v2:
  - id: e0abf868-dae2-4c1c-83e9-b21799232845
  - id: fbd94e4b-f9b8-42a4-8df5-3f917aabae24
  - id: a567f0f7-0057-4079-8ded-5b24cc25af15
  - id: f40f1683-8300-4054-aab8-77da06ad63ff
  - id: d822825b-9821-40d5-9b0d-42a9e3f317c5
subfeature_v2:
  - id: ad7101f7-ae92-401b-a25a-d3060d42989d
  - id: a4dc3e7d-bd07-4ac8-8e49-ff2e8fecf1e7
  - id: ee1bf083-e090-4def-936b-c111d29f42d0
  - id: d1167c89-f64a-42ca-ac95-1d91b7790df2
  - id: bc2f5225-03d4-4bc8-89ec-99d78c30e6dd
  - id: d4b8ba18-64c1-4413-be54-74405ec7f558
  - id: ba4fd72c-282e-4fb6-abc1-08e6fb87b2ad
  - id: b4655f7e-1a6e-4fa3-a7c5-3c34d4786e49
  - id: b2d4aeb9-eabe-49f6-8edb-bb2862d5980b
  - id: c89e26b6-808d-4500-8b01-450a63466999
  - id: a9505d76-24a1-4ffe-bd01-6ac32d5af453
  - id: cb40363e-1205-4921-971c-9ee6bdb18329
  - id: d7b067e6-4f39-41e9-a081-7650346a84cd
  - id: b2520ae7-8f6c-4952-935e-aacc2c10256f
  - id: e6c284e0-b6e6-4f82-bf96-e96bb5157b90
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
autotag-review: '2026-05-01T09:15:33.908Z'
source-git-commit: 5579087b9381c4d8e909ed5fe3099fd42d5c6799
workflow-type: tm+mt
source-wordcount: 238
ht-degree: 1%

---

# Mix Modeler工作流程

请观看本视频，了解Mix Modeler中的用户工作流的简介。

>[!VIDEO](https://video.tv.adobe.com/v/3424854/?learn=on)


Mix Modeler中的典型工作流包含以下活动：

![替换文本](/help/assets/ApplicationWorkflow.svg)

|  | 活动 | 描述 |
|---|---|---|
| ![数据](/help/assets/icons/Data.svg){width="100"} | [**摄取数据**](../ingest-data/overview.md) | 从Experience Platform（例如Adobe Analytics、Web SDK、其他来源）摄取事件数据、从营销渠道（例如电视、封闭花园、电子邮件、自有和经营活动）摄取聚合数据、从客户摄取外部因素数据（例如订阅服务的价格变化）和内部因素数据（例如假日计划）。 |
| ![数据检查](/help/assets/icons/DataCheck.svg){width="100"} | [**协调数据**](../harmonize-data/overview.md) | 配置映射规则和冲突解决规则，以合并Mix Modeler中衡量和规划营销活动绩效所需的各种营销数据集。 |
| ![文件配置](/help/assets/icons/FileGear.svg){width="100"} | [**生成模型**](../models/overview.md) | 包含营销接触点（例如渠道）、转化定义以及内部和外部因素的构建模型实例。 |
| ![文件数据](/help/assets/icons/FileData.svg){width="100"} | [**训练模型和评分模型**](../models/overview.md) | 使用机器学习训练和评分创建聚合分数和事件级分数。 |
| ![文件图表](/help/assets/icons/FileChart.svg){width="100"} | [**生成计划**](../plans/overview.md) | 创建和构建计划。 使用Mix Modeler模型的输出确定营销资金的最佳分配，以实现业务目标。 |
| ![仪表板](/help/assets/icons/Dashboard.svg){width="100"} | [**概述仪表板**](../dashboard/overview.md) | 使用各种可配置的可视化图表，深入了解协调的数据、模型和计划。 |

{style="table-layout:auto"}

下面概述了输入数据如何流入Mix Modeler，以及Mix Modeler如何为自己的界面以及其他解决方案（如Customer Journey Analytics）生成输出数据。

![Mix Modeler输入输出数据流](../assets/mm-input-output.png)

<!--
The detailed data-oriented flowchart below illustrates how:

* harmonized data is based on:

  * experience event data (originating from Analytics source connector, collected through Experience Platform SDKs and APIs, ingested through source connectors, or using streaming ingestion),
  * aggregate or summary data from walled gardens (like Facebook, YouTube), traffic sources, or offline advertising data, and 
  * definitions of harmonized fields and dataset rules.

* a model is based on:

  * the conversion and marketing touchpoint definitions resulting from the harmonized data and 
  * non-marketing aggregate or summary data containing internal or external factors.

* mult-touch attribution event scores can potentially be fed back into Experience Platform data lake for use in subsequent model configuration, training and scoring.

![Comprehensive workflow](/help/assets/comprehensive-workflow.svg)
-->
