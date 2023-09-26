---
title: Adobe组合建模器工作流程
description: 了解Adobe组合建模器的典型工作流程。
feature: Datasets, Event Datasets, Plans, Harmonized Data, Models
source-git-commit: ac17f5a9fcf036c8e689879578e4b745b789cea3
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 2%

---


# Adobe组合建模器工作流程

Adobe混合建模器中的典型工作流如下所示：

![替换文字](../assets/ApplicationWorkflow.svg)

|  | 活动 | 描述 |
|---|---|---|
| ![数据](../assets/icons/Data.svg){width="100"} | [**引入数据**](../ingest-data/overview.md) | 从Adobe Experience Platform(例如Adobe Analytics、Web SDK、其他源)摄取事件数据、从营销渠道（例如电视、封闭式花园、电子邮件、自有和运营的活动）摄取聚合数据，以及从客户摄取外部因素数据（例如订阅服务的价格变化）。 |
| ![DataCheck](../assets/icons/DataCheck.svg){width="100"} | [**协调数据**](../harmonize-data/overview.md) | 配置映射规则和冲突解决规则，以合并在Adobe组合建模器中衡量和规划营销活动绩效所需的各种营销数据集。 |
| ![FileConfig](../assets/icons/FileGear.svg){width="100"} | [**配置模型**](../models/create.md) | 使用营销接触点（例如渠道）和转化定义配置模型实例。 |
| ![文件数据](../assets/icons/FileData.svg){width="100"} | [**训练模型并为其评分**](../models/overview.md) | 使用机器学习训练和评分创建聚合分数和事件级分数。 |
| ![文件图表](../assets/icons/FileChart.svg){width="100"} | [**创建计划**](../plans/overview.md) | 利用Adobe组合建模器模型的输出结果确定营销资金的最佳分配以实现业务目标。 |
| ![功能板](../assets/icons/Dashboard.svg){width="100"} | [**概述仪表板**](../dashboard/overview.md) | 使用各种可配置的构件深入了解协调的数据、模型和计划。 |

{style="table-layout:auto"}

