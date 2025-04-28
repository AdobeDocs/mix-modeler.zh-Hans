---
title: 协调数据集概述
description: 了解如何在Mix Modeler中协调数据。
feature: Harmonized Data
exl-id: 6cb70762-e3b2-46a0-b028-1d6daf3edae5
source-git-commit: 857641f6c1db749f79056ce2a2ea35fc4d3e3a3c
workflow-type: tm+mt
source-wordcount: '1013'
ht-degree: 6%

---

# 协调数据集概述

Mix Modeler中的数据性质因数据源而异。 数据可以是：

* 聚合或摘要数据，例如从围墙花园数据源收集的数据，或通过运行广告牌营销活动、事件或物理广告营销活动收集的离线广告数据（如支出），
* 事件数据，例如来自第一方数据源的事件数据。 此事件数据可以是通过Adobe Analytics源连接器从Adobe Analytics收集的数据，也可以是通过Experience Platform Web或Mobile SDK或Edge Network API收集的数据，或使用源连接器引入的数据。

Mix Modeler的协调服务将聚合和事件数据吸收到一致的数据视图中。 此数据视图与[内部和外部因素数据](#factors)相结合，是Mix Modeler中模型的源。 该服务在不同数据集上使用最高的粒度。 例如，如果一个数据集的粒度为每月，而其余数据集的粒度为每周和每日，则协调服务使用每月粒度创建一个数据视图。

## 因素

因素对于模型构建至关重要，您想要了解哪些因素会对业务产生整体影响。 因素可能与营销数据无关。

* 内部因素特定于您的组织，可能会影响您的转化。 例如，您的销售季节、促销活动等。

* 外部因素是组织无法控制的因素，但仍会影响您实现的转化。 例如CPI、标普500等。



## 统一数据的示例

假设您有以下数据集可用于Mix Modeler。

**数据集1**

包含YouTube中的营销工作数据集，并将聚合数据集的粒度设置为每天。

| 日期 | 日期类型 | 渠道 | Campaign | 品牌 | 地域 | 点击次数 | 支出 |
|---|:--:|---|---|---|---|---:|---:|
| 12-31-2021 | 天 | YouTube | Y_Fall_02 | BrandX | US | 10000 | 100 |
| 01-01-2022 | 天 | YouTube | Y_Fall_02 | BrandX | US | 1000 | 10 |
| 01-03-2022 | 天 | YouTube | Y_Fall_01 | BrandY | CA | 10000 | 100 |
| 01-04-2022 | 天 | YouTube | Y_Summer_01 | 空 | CA | 9000 | 80 |

{style="table-layout:auto"}


**数据集2**

包含来自Facebook的营销工作数据集，其聚合数据的粒度设置为每周。

| 日期 | 日期类型 | 渠道 | Campaign | 地域 | 点击次数 | 支出 |
|--- |:---:|--- |---|---|---:|---:|
| 01-01-2022 | 周 | Facebook | FB_Fall_01 | US | 8000 | 100 |
| 01-08-2022 | 周 | Facebook | FB_Fall_02 | US | 1000 | 10 |
| 01-08-2022 | 周 | Facebook | FB_Fall_01 | US | 7000 | 100 |
| 01-16-2022 | 周 | Facebook | FB_Summer_01 | CA | 10000 | 80 |

{style="table-layout:auto"}


**数据集3**

转化数据集，其聚合数据集的粒度设置为每天。

| 日期 | 日期类型 | 地域 | 目标 | 收入 |
|--- |:---: |---|---|---:|
| 01-01-2022 | 天 | US | 时尚 | 200 |
| 01-08-2022 | 天 | US | 时尚 | 10 |
| 01-08-2022 | 天 | US | 珠宝 | 1100 |
| 01-16-2022 | 天 | CA | 珠宝 | 80 |

{style="table-layout:auto"}


**数据集4**

客户提供的示例体验事件数据集(Web SDK事件)。

| 时间戳 | 身份标识命名空间 | 身份ID | 渠道 | 点击次数 |
|--- |--- |--- |--- |---:|
| 01-01-2022 00:01:01.000 | ECID | 64fd46ff-8c63-43b4-85a7-92b953113ba0 | CSE | 1 |
| 01-01-2022 00:01:01.000 | ECID | 64fd46ff-8c63-43b4-85a7-92b953113ba0 | CSE | 1 |
| 01-08-2022 00:01:01.000 | ECID | 2ca2a16e-caf0-4fa9-9a8b-9774b39547c4 | CSE | 1 |
| 01-08-2022 00:01:01.000 | ECID | 5ce99bfb-e44a-40d9-b8cd-c5408bda7cdc | CSE | 1 |

{style="table-layout:auto"}


您要构建协调的数据集，并将粒度设置为每周。 将事件数据聚合到周粒度，并将其添加到协调的数据集。 结果是：

**协调的数据集**

| 日期 | 日期类型 | 渠道 | Campaign | 品牌 | 地域 | 目标 | 点击次数 | 支出 | 收入 |
|--- |:---:|--- |--- |--- |---|---|---:|---:|---:|
| 12-27-2021 | 周 | YouTube | Y_Fall_02 | BrandX | US | 空 | 11000 | 110 | 空 |
| 01-03-2022 | 周 | YouTube | Y_Fall_01 | BrandY | CA | 空 | 10000 | 100 | 空 |
| 01-03-2022 | 周 | YouTube | Y_Summer_01 | 空 | CA | 空 | 9000 | 80 | 空 |
| 01-01-2022 | 周 | Facebook | FB_Fall_01 | 空 | US | 空 | 8000 | 100 | 空 |
| 01-08-2022 | 周 | Facebook | FB_Fall_02 | 空 | US | 空 | 1000 | 10 | 空 |
| 01-08-2022 | 周 | Facebook | FB_Fall_01 | 空 | US | 空 | 7000 | 100 | 空 |
| 01-16-2022 | 周 | Facebook | FB_Summer_01 | 空 | CA | 空 | 10000 | 80 | 空 |
| 12-27-2021 | 周 | 空 | 空 | 空 | US | 时尚 | 空 | 空 | 200 |
| 01-03-2022 | 周 | 空 | 空 | 空 | US | 时尚 | 空 | 空 | 10 |
| 01-03-2022 | 周 | 空 | 空 | 空 | US | 珠宝 | 空 | 空 | 1100 |
| 01-10-2022 | 周 | 空 | 空 | 空 | CA | 珠宝 | 空 | 空 | 80 |
| 01-01-2022 | 周 | CSE | 空 | 空 | 空 | 空 | 2 | 空 | 空 |
| 01-08-2022 | 周 | CSE | 空 | 空 | 空 | 空 | 2 | 空 | 空 |

{style="table-layout:auto"}


## 设置统一数据

要像在简化的[示例](#an-example-of-harmonized-data)中一样构建协调的数据集，您必须执行以下步骤：

1. 定义要在现有的全球统一字段之外使用的其他[统一字段](fields.md)。
1. 设置[数据集规则](dataset-rules.md)以将聚合或体验事件数据集的字段映射到协调的字段。
1. 使用您定义的标准和附加协调字段定义[营销接触点](marketing-touchpoints.md)。
1. 使用您定义的标准和附加协调字段定义[转化](conversions.md)。


## 查看协调的数据

要查看您的协调数据，请在Mix Modeler界面中执行以下操作：

1. 从左边栏中选择![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized datasets]**。

1. 从顶部栏中选择&#x200B;**[!UICONTROL Harmonized data]**。 系统将根据您定义的字段、数据集规则、营销接触点和转化显示协调数据的简述。

   1. 要重新定义重新提取协调数据所依据的期间，请输入&#x200B;**[!UICONTROL Date range]**&#x200B;的日期范围或使用![日历](/help/assets/icons/Calendar.svg)选择数据范围。

   1. 要修改“协调”数据表中显示的协调字段列，请使用![设置](/help/assets/icons/Setting.svg)打开&#x200B;**[!UICONTROL Column settings]**&#x200B;对话框。

      1. 从&#x200B;**[!UICONTROL AVAILABLE COLUMNS]**&#x200B;中选择![SelectBox](/help/assets/icons/SelectBox.svg)一个或多个列，并使用![右V形](/help/assets/icons/ChevronRight.svg)将这些列添加到&#x200B;**[!UICONTROL SELECTED COLUMNS]**。

      1. 从&#x200B;**[!UICONTROL SELECTED COLUMNS]**&#x200B;中选择![SelectBox](/help/assets/icons/SelectBox.svg)一个或多个列，并使用![左V形](/help/assets/icons/ChevronLeft.svg)删除所选列并将这些列返回给&#x200B;**[!UICONTROL AVAILABLE COLUMNS]**。

      1. 从&#x200B;**[!UICONTROL DEFAULT SORT]**&#x200B;中选择一列并在&#x200B;**[!UICONTROL Ascending]**&#x200B;或&#x200B;**[!UICONTROL Descending]**&#x200B;之间切换。

      1. 要更改列的显示顺序，您可以通过拖放来上下移动&#x200B;**[!UICONTROL SELECTED COLUMNS]**&#x200B;中的列。

   1. 选择&#x200B;**[!UICONTROL Submit]**&#x200B;以提交列设置更改。 选择&#x200B;**[!UICONTROL Close]**&#x200B;以取消所做的任何更改。

1. 如果有更多页面可用，请使用&#x200B;_x _]**的**[!UICONTROL Page _x_&#x200B;上的![向左箭头](/help/assets/icons/ChevronLeft.svg)或![向右箭头](/help/assets/icons/ChevronRight.svg)在页面之间移动。

1. 您可以选择下载协调的数据。

   1. 选择![下载](/help/assets/icons/Download.svg) [!BADGE 测试版]。
   1. 在弹出窗口中，选择![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Create]**。
   1. 输入&#x200B;**[!UICONTROL Report name]**，例如`Test Report`。
   1. 选择![FileCSV](/help/assets/icons/FileCSV.svg) **[!UICONTROL Report]**。

   标题基于您提供的报表名称以及当前日期和时间（例如`Test Report_2025_04_23_9-5-18.csv`）的CSV报表将下载到您的默认下载文件夹。

