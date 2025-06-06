---
title: Mix Modeler工作流程
description: 了解Mix Modeler的典型工作流程。
feature: Ingest Data, Plans, Harmonized Data, Models
exl-id: 200ff846-5d78-4b25-a425-bfd558b88c88
source-git-commit: bdb5992ba1e6a4e5aa546b6ffb8e9673ed69be22
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Mix Modeler工作流程

请观看本视频，了解Mix Modeler中的用户工作流的简介。

>[!VIDEO](https://video.tv.adobe.com/v/3440216/?learn=on&captions=chi_hans)


Mix Modeler中的典型工作流包含以下活动：

![替换文本](/help/assets/ApplicationWorkflow.svg)

|  | 活动 | 描述 |
|---|---|---|
| ![数据](/help/assets/icons/Data.svg){width="100"} | [**摄取数据**](../ingest-data/overview.md) | 从Experience Platform(例如Adobe Analytics、Web SDK、其他来源)摄取事件数据、从营销渠道（例如电视、封闭花园、电子邮件、自有和经营活动）摄取聚合数据、从客户摄取外部因素数据（例如订阅服务的价格变化）和内部因素数据（例如假日计划）。 |
| ![数据检查](/help/assets/icons/DataCheck.svg){width="100"} | [**协调数据**](../harmonize-data/overview.md) | 配置映射规则和冲突解决规则，以合并Mix Modeler中衡量和规划营销活动绩效所需的各种营销数据集。 |
| ![文件配置](/help/assets/icons/FileGear.svg){width="100"} | [**生成模型**](../models/overview.md) | 包含营销接触点（例如渠道）、转化定义以及内部和外部因素的构建模型实例。 |
| ![文件数据](/help/assets/icons/FileData.svg){width="100"} | [**训练模型和评分模型**](../models/overview.md) | 使用机器学习训练和评分创建聚合分数和事件级分数。 |
| ![文件图表](/help/assets/icons/FileChart.svg){width="100"} | [**生成计划**](../plans/overview.md) | 创建和构建计划。 使用Mix Modeler模型的输出确定营销资金的最佳分配，以实现业务目标。 |
| ![仪表板](/help/assets/icons/Dashboard.svg){width="100"} | [**概述仪表板**](../dashboard/overview.md) | 使用各种可配置的可视化图表，深入了解协调的数据、模型和计划。 |

{style="table-layout:auto"}

下面概述了输入数据如何流入Mix Modeler，以及Mix Modeler如何为自己的界面以及其他解决方案(如Customer Journey Analytics)生成输出数据。

![Mix Modeler输入输出数据流](../assets/mm-input-output.png)
<!---
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
