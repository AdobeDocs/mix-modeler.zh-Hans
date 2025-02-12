---
title: 使用评分数据
description: 了解如何保留Mix Modeler中的模型评分数据。
feature: Models
exl-id: 2f2c3d20-7b14-41cc-a11a-03e8ad9e5d7a
source-git-commit: 5f6c35816a8850bf170cb73d9710e65809e5f372
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 6%

---

# 使用评分数据

在对模型评分的过程中，评分数据会保留在Experience Platform的数据集内。 如果您在模型创建期间启用了多接触点归因，则Experience Platform中的某个数据集中会保留额外的事件得分数据。

其中每个数据集都符合架构。 本文记录了这些架构。


## 汇总评分数据架构

评分数据的架构的名称类似于`AMM AI Schema - <name of model> <id>`。 例如： `AMM AI Schema - Model for Online Conversion 10120`。

保留模型评分数据的数据集的名称类似于`AMM AI Aggregrate Scores - <id>`，例如`AMM AI Aggregrate Scores - 10120`。

该架构包括一个字段组，该字段组具有一个包含有关分数的详细信息的对象。 该对象包含以下字段。

| 字段名称 | 类型 | 定义 |
|---|---|---|
| `campaignGroup` | 字符串 | 营销活动组的名称。 |
| `campaignName` | 字符串 | 营销活动的名称。 |
| `contribution` | 多次 | 给定接触点中归属于此转化的贡献。 |
| `conversionEndDate` | 日期 | 转换窗口的结束日期。 |
| `conversionName` | 字符串 | 在转换定义设置步骤中创建的转换的名称。 |
| `conversionStartDate` | 日期 | 转换窗口的开始日期。 |
| `geo` | 字符串 | 发生转化的地理位置。 |
| `mediaChannel` | 字符串 | 在接触点设置步骤中使用的渠道名称。 |
| `mediaSubChannel` | 字符串 | 子渠道的名称。 |
| `revenue` | 多次 | 归因于给定接触点的此转化的收入。 |
| `scoreCreatedTime` | 日期时间 | 创建此得分记录时的时间戳。 |
| `touchpointEndDate` | 日期 | 接触点窗口的结束日期。 |
| `touchpointName` | 字符串 | 在接触点定义设置步骤中创建的接触点的名称。 目前，接触点是在媒体频道上定义的。 |
| `touchpointStartDate` | 日期 | 接触点窗口的开始日期。 |


## 事件评分数据架构

评分数据的架构的名称类似于`Attribution AI Scores - <name of model> <id> - Schema`。 例如： `Attribution AI Scores - Model for Online Conversion 10120 - Schema`。

保留模型评分数据的数据集的名称类似于`Attribution AI Scores - <name of model> <id>`，例如`Attribution AI Scores - Model for Online Conversion 10120 `。

该架构包含一个字段组，该字段组包含包含有关内核的详细信息的对象。 对象的名称类似于`attibution_AI_scores__<name of model> id`。

该字段组包含以下字段。

| 字段名称 | 类型 | 描述 |
|---|---|---|
| `conversion` | 对象 | 转换元数据列。 |
|     `passThrough` | 对象 |  |
|         `eventType` | 字符串 | |
|         `channel_typeAtSource` | 字符串 | |
|      `dataSource` | 字符串 | 数据源的全局唯一标识。<br> **示例：** `Adobe Analytics` |
|      `eventSource` | 字符串 | 实际事件发生时的源。<br> **示例：** `Adobe.com` |
|      `eventType` | 字符串 | 此时间序列记录的主要事件类型。<br> **示例：** `Order` |
|      `geo` | 字符串 | 转换传递的地理位置`placeContext.geo.countryCode`。<br> **示例：** `US` |
|      `path` | 字符串 | |
|      `priceTotal` | 多次 | 通过转换<br>获得的收入 **示例：** `99.9` |
|      `product` | 字符串 | 产品本身的XDM标识符。<br> **示例：** `RX 1080 ti` |
|      `productType` | 字符串 | 在此产品视图中向用户显示的产品显示名称。<br> **示例：** `Gpus` |
|      `quantity` | 整数 | 转换期间购买的数量。<br> **示例：** `1` |
|      `receivedTimeStamp` | 日期时间 | 已收到转换的时间戳。<br> **示例：** `2020-06-09T00:01:51.000Z` |
|      `skuId` | 字符串 | 库存单位(SKU)，供应商定义的产品的唯一标识符。<br> **示例：** `MJ-03-XS-Black` |
|      `timestamp` | 日期时间 | 转换的时间戳。<br> **示例：** `2020-06-09T00:01:51.000Z` |
|      `totalDaysToConversion` | 整数 |  |
|      `totalTouchpointCount` | 整数 | |
| `customerProfile` | 对象 | 用于构建模型的用户的身份详细信息。 |
|      `identity` | 对象 | |
|           `id` | 字符串 | |
|           `namespace` | 字符串 | 包含用于构建模型的用户的详细信息，如`id`和`namespace`。 |
| `touchpointsDetail` | 对象[] | 导致转化的接触点详细信息列表，按接触点出现次数或时间戳排序。 |
|      `scores` | 对象 | 作为得分的接触点对此转化的贡献。 |
|           `algorithmicInfluenced` | 多次 | 影响分数是每个营销接触点负责的转化率部分。 |
|           `algorithmicSourced` | 多次 | 增量分数是营销接触点直接造成的边际影响量。 |
|           `decayUnits` | 多次 | 基于规则的归因得分，其中距离转化较近的接触点比距离转化较远的接触点获得更多的点数。 |
|           `firstTouch` | 多次 | 基于规则的归因得分，将所有信用分配给转化路径上的初始接触点。 |
|           `lastTouch` | 多次 | 基于规则的归因得分，可将所有信用分配给最接近转化的接触点。 |
|           `linear` | 多次 | 基于规则的归因得分，它将信用平等分配给转化路径上的每个接触点。 |
|           `uShape` | 多次 | 基于规则的归因得分，将40%的信用分配给第一个接触点，将40%的信用分配给最后一个接触点。 其他接触点平分剩余的20%。 |
|      `touchPoint` | 对象 | 接触点元数据。 |
|           `passThrough` | 对象 | |
|                `eventType` | 字符串 | |
|           `campaignGroup` | 字符串 |  |
|           `campaignName` | 字符串 | |
|           `campaignTag` | 字符串 | |
|           `eventId` | 字符串 | |
|           `geo` | 字符串 | |
|           `mediaAction` | 字符串 | |
|           `mediaChannel` | 字符串 | |
|           `receivedTimeStamp` | 日期时间 | |
|           `timestamp` | 日期时间 | |
|      `isFirstInThePosition` | 整数 | |
|      `lag` | 整数 | |
|      `position` | 字符串 | |
|      `touchpointCountToConversion` | 整数 | |
|      `touchpointName` | 字符串 | 在安装期间配置的接触点的名称。<br> **示例：** `PAID_SEARCH_CLICK` |
| `conversionName` | 字符串 | 在安装期间配置的转换的名称。<br> **示例：** `Order`，`Lead`，`Visit` |
| `scoreCreatedTime` | 日期时间 | |
| `segmentation` | 字符串 | 转化区段，例如构建模型所针对的地域划分。 当区段不存在时，`segmentation`与`conversionName`相同。<br> **示例：** `ORDER_US` |





有关详细信息，请参阅[架构](../ingest-data/schemas.md)。
