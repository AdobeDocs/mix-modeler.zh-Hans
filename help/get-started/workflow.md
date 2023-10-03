---
title: Mix Modeler工作流
description: 了解Mix Modeler的典型工作流程。
feature: Ingest Data, Plans, Harmonized Data, Models
exl-id: 200ff846-5d78-4b25-a425-bfd558b88c88
source-git-commit: 33883626d8e7aca2eecc3571593be53ef41ac458
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 2%

---

# Mix Modeler工作流

Mix Modeler中的典型工作流如下所示：

![替换文字](../assets/ApplicationWorkflow.svg)

|  | 活动 | 描述 |
|---|---|---|
| ![数据](../assets/icons/Data.svg){width="100"} | [**引入数据**](../ingest-data/overview.md) | 从Experience Platform(例如Adobe Analytics、Web SDK、其他源)摄取事件数据、从营销渠道（例如电视、封闭花园、电子邮件、自有和经营活动）摄取聚合数据、从客户摄取外部因素数据（例如订阅服务的价格变化）和内部因素数据（例如假日计划）。 |
| ![DataCheck](../assets/icons/DataCheck.svg){width="100"} | [**协调数据**](../harmonize-data/overview.md) | 配置映射规则和冲突解决规则以合并在Mix Modeler中衡量和规划营销活动绩效所需的各种营销数据集。 |
| ![FileConfig](../assets/icons/FileGear.svg){width="100"} | [**配置模型**](../models/create.md) | 使用营销接触点（例如渠道）和转化定义配置模型实例。 |
| ![文件数据](../assets/icons/FileData.svg){width="100"} | [**训练模型并为其评分**](../models/overview.md) | 使用机器学习训练和评分创建聚合分数和事件级分数。 |
| ![文件图表](../assets/icons/FileChart.svg){width="100"} | [**创建计划**](../plans/overview.md) | 利用Mix Modeler模型的输出结果确定营销资金的最佳分配，以实现业务目标。 |
| ![功能板](../assets/icons/Dashboard.svg){width="100"} | [**概述仪表板**](../dashboard/overview.md) | 使用各种可配置的构件深入了解协调的数据、模型和计划。 |

{style="table-layout:auto"}
