---
title: 评分数据
description: 了解如何保留Mix Modeler中的模型评分数据。
feature: Models
exl-id: 2f2c3d20-7b14-41cc-a11a-03e8ad9e5d7a
source-git-commit: 86732fe30637aa72ced232d9f331a3cc64baa39b
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 5%

---

# 评分数据

在对模型评分的过程中，评分数据会保留在Experience Platform的数据集内。 此数据集符合为Mix Modeler实例中的每个模型创建的架构。

评分数据的架构的命名如下 `AMM AI Schema - <name of model> <id>`. 例如： `AMM AI Schema - Model for Online Conversion 10120`.

持久保留模型的评分数据的数据集的名称如下 `AMM AI Aggregrate Scores - <id>`例如 `AMM AI Aggregrate Scores - 10120`.


## 架构

该架构包括一个字段组，该字段组具有一个包含有关分数的详细信息的对象。 该对象包含以下字段。

| 字段名称 | 类型 | 定义 |
|---|---|---|
| **campaignGroup** | 字符串 | 营销活动组的名称。 |
| **campaignName** | 字符串 | 营销活动的名称。 |
| **贡献** | 多次 | 给定接触点中归属于此转化的贡献。 |
| **conversionEndDate** | 日期 | 转换窗口的结束日期。 |
| **conversionName** | 字符串 | 在转换定义设置步骤中创建的转换的名称。 |
| **conversionStartDate** | 日期 | 转换窗口的开始日期。 |
| **地域** | 字符串 | 发生转化的地理位置。 |
| **mediaChannel** | 字符串 | 在接触点设置步骤中使用的渠道名称。 |
| **mediaSubChannel** | 字符串 | 子渠道的名称。 |
| **收入** | 多次 | 归因于给定接触点的此转化的收入。 |
| **scorecreatedtime** | 日期时间 | 此得分记录的创建时间。 |
| **接触点结束日期** | 日期 | 接触点窗口的结束日期。 |
| **接触点名称** | 字符串 | 在接触点定义设置步骤中创建的接触点的名称。 目前，接触点是在媒体频道上定义的。 |
| **接触点开始日期** | 日期 | 接触点窗口的开始日期。 |

请参阅 [架构](../ingest-data/schemas.md) 以了解更多信息。
