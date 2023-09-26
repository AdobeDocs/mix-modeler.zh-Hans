---
title: 引入数据
description: 了解如何将数据摄取到Adobe组合建模器。
feature: Datasets, Event Datasets, Summary Datasets, Aggregate Datasets
source-git-commit: ae1c74ed2edf1e69e7ab77d16aba797921c14ad9
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 14%

---


# 引入数据

Adobe Mix Modeler可同时处理来自各个封闭花园的事件级别数据和汇总营销工作数据。 客户可以将摄取到Adobe Experience Platform中的各种数据用作数据集，并且这些数据基于基于XDM体验事件的架构。

例如：

* 使用Adobe Analytics源连接器收集并转换为符合Adobe Analytics架构的默认或自定义版本的数据集，或者，
* 使用Adobe Experience Platform Web SDK、Mobile SDK或边缘网络服务器API收集的数据，用于收集Web、移动设备或任何其他类型设备上的客户交互。
* 来自不同围墙花园/流量源的摘要数据，基于包含XDM摘要量度类以及流量和转化摘要字段组的架构，
* 有助于建立模型的非市场数据（例如宏观经济指标），

您可以使用Adobe Experience Platform支持的任何类型的机制来摄取体验事件级别和汇总营销工作数据。 例如Adobe Experience Platform SDK、API、源连接器以及流式摄取和批量摄取。


## 准则

要将数据摄取到Adobe Experience Platform以与Adobe组合建模器一起使用，请遵循以下准则：

* 添加到数据集的增量数据不应有任何重叠。
* 来自单个源的所有数据都应具有相同的粒度。
* 对于摄取为数据集的所有聚合数据，日期和粒度是基础架构中的必填字段
* 对于作为数据集引入的所有营销工作/支出数据，渠道是基础架构中的必填字段。


## 示例

在下面查找一些通常用于Adobe组合建模器的数据示例，这些示例超出了更标准的体验事件数据。

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

要在Adobe组合建模器中处理数据，您需要在数据集中收集数据，并按照Adobe Experience Platform中的架构进行建模。 通过Adobe组合建模器界面，可以轻松访问架构和数据集UI。

>[!MORELIKETHIS]
>
>有关如何管理架构和数据集的更多详细信息，请参阅：
>
>* [架构](schemas.md)
>* [数据集](datasets.md)
