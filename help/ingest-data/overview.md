---
title: 摄取数据概述
description: 了解如何将数据摄取到Mix Modeler。
feature: Datasets, Event Datasets, Summary Datasets, Aggregate Datasets
exl-id: dc16a601-bbd9-467b-8a7e-c32654d4069a
source-git-commit: 1a9df9f9819d9e0031e58443ec6a9e755a151ba0
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 7%

---

# 摄取数据概述

Mix Modeler可处理来自不同封闭花园的事件级数据、汇总或汇总营销工作数据。 以及来自任何其他来源（如离线广告、内部因素或外部因素）的汇总或汇总数据。

客户可以将摄取到Experience Platform中的任何类型的数据用作数据集，此类数据基于将XDM ExperienceEvent或XDM摘要量度用作基类的架构。

例如：

* 使用Adobe Analytics源连接器收集的数据。 并转换为符合Adobe Analytics架构的默认或自定义版本的数据集。
* 使用Experience Platform Web SDK、Mobile SDK或Edge Network Server API收集的数据，用于收集Web、移动设备或任何其他类型设备上的客户交互。
* 汇总或摘要来自封闭花园的数据(如Facebook、YouTube)、流量源或离线广告数据。
* 包含对模型构建有用的内部或外部因素的非营销聚合或摘要数据。

您可以使用Experience Platform支持的任何类型的机制，从其他来源摄取体验事件级别的汇总营销工作数据和数据。 例如Experience Platform SDK、API、源连接器以及流式摄取和批量摄取。 要了解有关在Experience Platform中引入数据以用于Adobe Mix Modeler的更多信息，请参阅[数据引入概述](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/ingestion/home)。

## 准则

要将数据摄取到Experience Platform以与Mix Modeler一起使用，请遵循以下准则：

* 添加到数据集的增量数据不应有任何重叠。
* 来自单个源的所有数据都应具有相同的粒度。
* 对于摄取为数据集的所有聚合数据，日期和粒度是基础架构中的必填字段
* 对于作为数据集引入的所有营销工作/支出数据，渠道是基础架构中的必填字段。


## 示例

在下面查找除了更标准的体验事件数据之外通常在Mix Modeler中使用的一些数据示例。

+++ 汇总营销工作数据

| 地域 | 日期 | 日期类型 | 渠道 | Campaign | 单击 | 已获取 | 参与度 | 印象 | Open | 已拥有 | 已发送 | 支出 |
|---|:--|---|:---:|---|--:|---|--:|---|---|---|--:|--:|
| AMER | 2021-10-31 | 天 | 电子邮件 | | 12752 | | | | | | 1132945 | |
| AMER | 2021-10-31 | 天 | FB | | 148844 | | | | | | | 42111 |
| AMER | 2021-10-31 | 天 | YT | | | | 2314452 | | | | | 10540 |
| 日本 | 2021-10-21 | 天 | 电子邮件 | | 21089 | | | | | | 3283626 | |
| 日本 | 2021-10-21 | 天 | SOCIAL | | | | 621 | | | | | 74512 |

{style="table-layout:auto"}

+++

+++ 汇总转化数据

| 地域 | 日期 | 日期类型 | 产品 | 销售量 | 收入 |
|---|:---|:---:|---|--:|--:|
| EMEA | 2021-09-13 | 天 | 创新型经济 | 603 | 36537.68 |
| EMEA | 2021-09-13 | 天 | 元宇宙 | 55 | 21704.37 |
| 日本 | 2022-05-30 | 天 | Pro Imaging | 487 | 64469.60 |
| 日本 | 2022-05-30 | 天 | Document Cloud | 642 | 100509.07 |

{style="table-layout:auto"}

+++

+++ 外部因素数据

| 数据 | 日期类型 | 因素 | 值 |
|---|:---:|:---:|:---|
| 2020-08-02 | 周 | SPX | 3325.866 |
| 2020-08-09 | 周 | SPX | 3364.158 |
| 2020-08-16 | 周 | SPX | 3385.858 |
| 2020-08-23 | 周 | SPX | 3497.965 |

{style="table-layout:auto"}

+++

要在Mix Modeler中处理数据，您需要在数据集中收集数据，并按照Experience Platform中的架构建模。 通过Mix Modeler界面，可以轻松访问Experience Platform架构和数据集UI。


## 验证

要验证您的数据在Mix Modeler中是否正确可用，您可以执行以下操作：

* 在[概述](/help/overview.md)中使用可视化。
* 下载并检查来自协调数据集中的[协调数据](/help/harmonize-data/overview.md)的数据。

若要验证您的数据是否在Experience Platform中正确摄取，您可以[使用Experience Platform查询服务](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/query/home)编写和执行SQL查询。


>[!MORELIKETHIS]
>
>有关如何管理架构和数据集的更多详细信息，请参阅：
>
>* [架构](schemas.md)
>* [数据集](datasets.md)
