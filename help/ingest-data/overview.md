---
title: 引入数据
description: 了解如何将数据摄取到Mix Modeler。
feature: Datasets, Event Datasets, Summary Datasets, Aggregate Datasets
exl-id: dc16a601-bbd9-467b-8a7e-c32654d4069a
source-git-commit: 86732fe30637aa72ced232d9f331a3cc64baa39b
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 8%

---

# 引入数据

Mix Modeler可与事件级数据、来自不同封闭花园的oe汇总营销成果数据以及来自任何其他来源（如离线广告、内部因素或外部因素）的汇总或汇总数据配合使用。

客户可以将摄取到Experience Platform中的任何类型的数据用作数据集，此类数据基于将XDM ExperienceEvent或XDM摘要量度用作基类的架构。

例如：

* 使用Adobe Analytics源连接器收集并转换为符合Adobe Analytics架构的默认或自定义版本的数据集，或者，
* 使用Experience PlatformWeb SDK、Mobile SDK或边缘网络服务器API收集的数据，用于收集Web、移动设备或任何其他类型设备上的客户交互。
* 聚集或摘要来自封闭式花园(如Facebook、YouTube)、流量源或离线广告数据的数据，
* 包含对模型构建有用的内部或外部因素的非营销聚合或摘要数据。

您可以使用Experience Platform支持的任何类型的机制来从其他来源摄取体验事件级的数据、汇总营销工作数据和数据。 例如Experience PlatformSDK、API、源连接器以及流式摄取和批量摄取。


## 准则

要将数据摄取到Experience Platform中以用于Mix Modeler，请遵循以下准则：

* 添加到数据集的增量数据不应有任何重叠。
* 来自单个源的所有数据都应具有相同的粒度。
* 对于摄取为数据集的所有聚合数据，日期和粒度是基础架构中的必填字段
* 对于作为数据集引入的所有营销工作/支出数据，渠道是基础架构中的必填字段。


## 示例

在下面查找一些通常用于Mix Modeler的数据示例，这些示例超出了更标准的体验事件数据。

+++ 汇总营销工作数据

| 地域 | 日期 | 日期类型 | 渠道 | Campaign | 单击 | 已获取 | 参与度 | 印象 | Open | 已拥有 | 已发送 |
|---|:--|---|:---:|---|--:|---|--:|---|---|---|--:|
| AMER | 2021-10-31 | 天 | 电子邮件 | | 12752 | | | | | | 1132945 |
| AMER | 2021-10-31 | 天 | FB | | 148844 | | | | | | |
| AMER | 2021-10-31 | 天 | YT | | | | 2314452 | | | | |
| 日本 | 2021-10-21 | 天 | 电子邮件 | | 21089 | | | | | | 3283626 |
| 日本 | 2021-10-21 | 天 | SOCIAL | | | | 621 | | | | |

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

要在Mix Modeler中处理数据，您需要在数据集中收集数据，并在Experience Platform中根据架构建模。 通过Mix Modeler界面可轻松访问Experience Platform架构和数据集UI。


>[!MORELIKETHIS]
>
>有关如何管理架构和数据集的更多详细信息，请参阅：
>
>* [架构](schemas.md)
>* [数据集](datasets.md)
