---
title: 模型分析
description: 了解如何获取有关模型的详细信息，如Mix Modeler中的历史概述、模型见解和模型质量。
feature: Models
exl-id: d99852f9-ba0d-4a2e-b5f3-ca0efe6002fd
source-git-commit: 72f122f1cdf7252dae9e93e5ea133e8cc76564dc
workflow-type: tm+mt
source-wordcount: '1422'
ht-degree: 0%

---

# 模型分析

要查看模型分析，请在Mix Modeler的![模型](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**&#x200B;界面中：

1. 从&#x200B;**[!UICONTROL Models]**&#x200B;表中，选择&#x200B;**[!UICONTROL Last run status]**&#x200B;为<span style="color:green">●</span>的模型的名称 **[!UICONTROL Success]**。

1. 从上下文菜单中选择&#x200B;**[!UICONTROL Model Insights]**。

![模型分析选项卡栏](/help/assets/model-insights-tabbar.png)

您会看到指定模型上次刷新的时间，并使用四个选项卡显示可视化图表：[模型分析](#model-insights)、[归因](#attribution)、[因素](#factors)、[诊断](#diagnostics)和[历史概述](#historical-overview)。

您可以更改每个选项卡上的可视化图表所基于的日期段。 输入日期期间或选择![日历](/help/assets/icons/Calendar.svg)以选择日期期间。

## [!UICONTROL Model insights]

“模型分析”选项卡显示[按日期和基本媒体列出的贡献](#contribution-by-date-and-base-media)、[按渠道列出的贡献](#contribution-by-channel)、[营销绩效摘要](#marketing-performance-summary)和[边际响应曲线](#marginal-response-curves)的可视化图表。 该选项卡还提供[接触点细分](#touchppint-breakdown)表。

![模型 — 模型分析](/help/assets/model-insights-insights.png)

* 您可以将鼠标悬停在每个可视化图表中的单个图表元素上，以显示包含更多详细信息的弹出框。

* 要下载包含可视化图表数据的CSV文件，请选择![下载](/help/assets/icons/Download.svg)。

* 要以Microsoft® Excel格式下载完整的模型分析数据，请选择![下载](/help/assets/icons/Download.svg) **[!UICONTROL Download data]**。


### 按日期和基本媒体列出的贡献

栈叠的图表按顺序排列：底部为基数，中间为非支出渠道，顶部为支出渠道。

### 按渠道显示的贡献

圆环图可视化图表显示按渠道划分的贡献分布。

### 营销绩效摘要

按渠道显示ROI绩效的水平条形图。

### 边际响应曲线

折线图可可视化并比较营销渠道投资产生的边际回报。  并找出盈亏平衡点，即递增回报低于递增支出。 因此，此可视化图表可帮助您了解营销投资何时开始变得不那么有影响力。

曲线、收支平衡点和相应的值是根据所选的数据范围和所选渠道计算的。

要更改渠道，请执行以下操作：

* 从&#x200B;**[!UICONTROL Channel]**&#x200B;下拉菜单中选择一个渠道以更新特定渠道的可视化图表。


### 接触点细分

接触点细分表每周显示所有渠道或选定渠道的接触点细分。

![接触点细分](../assets/touchpoint-breakdown.png)

以下列可用：

| 列 | 描述 |
|---|---|
| **[!UICONTROL Date range]** | 要报告的周。 |
| **[!UICONTROL Touchpoint]** | 特定的接触点渠道。 |
| **[!UICONTROL ROI]** | (**[!UICONTROL Revenue]** - **[!UICONTROL Spend]**) / **[!UICONTROL Spend]**&#x200B;的百分比。 |
| **[!UICONTROL Revenue]** | 日期范围的收入。 |
| **[!UICONTROL CPA]** | **[!UICONTROL Spend]** / **[!UICONTROL Conversions]**。 |
| **[!UICONTROL Conversions]** | 日期范围的转化。 |
| **[!UICONTROL Spend]** | 数据范围的支出。 |

要选择特定渠道或所有渠道，请从&#x200B;**[!UICONTROL View]**&#x200B;下拉菜单中选择。

要下载接触点划分表的内容，请选择![下载](/help/assets/icons/Download.svg) **[!UICONTROL Download CSV]**。

## [!UICONTROL Attribution]

使用[!UICONTROL Attribution]选项卡，您可以了解具有事件级别数据的接触点和营销活动的有效性。 支持以下归因模型：

* 根据Mix Modeler中选定的模型：
   * 算法 — 影响输出
   * 算法 — 增量
* 基于规则：
   * 衰减单位
   * 首次接触
   * 最后接触
   * 线性
   * Ushape

有关Mix Modeler中的多点触控归因功能的介绍，请参阅[多点触控归因](../get-started/about.md#multi-touch-attribution)。

从&#x200B;**[!UICONTROL Attribution Model]**&#x200B;下拉菜单中选择一个或多个归因模型。 选定的归因模型适用于归因选项卡中的所有可视化图表。

![归因](/help/assets/model-insights-attribution.png)

Mix Modeler多点接触归因粒度事件分数与总体Mix Modeler分数和ROI相匹配。 这些得分也可作为Experience Platform中的数据集使用。

归因选项卡包含以下可视化图表：

### [!UICONTROL Overview]

[!UICONTROL Overview]可视化图表显示选定归因模型的转化合计和百分比。 选择更多模型会为可视化图表添加其他圆，每个圆都有自己的颜色与图例相对应。

要查看包含归因模型详细信息的弹出窗口，请将光标悬停在可视化图表中的任何圆圈上。

### [!UICONTROL Trends]

[!UICONTROL Daily trends]、[!UICONTROL Weekly trends]或[!UICONTROL Monthly trends]可视化图表显示选定归因模型的每日、每周或每月转化趋势。

要选择句点，请从![更多](/help/assets/icons/More.svg)中选择&#x200B;**[!UICONTROL Daily trends]**、**[!UICONTROL Weekly trends]**&#x200B;或&#x200B;**[!UICONTROL Monthly trends]**。

要查看详细信息，请将鼠标悬停在特定归因模型的数据行上以显示一个弹出窗口，其中显示该数据的转化总数。

### [!UICONTROL Breakdown]

[!UICONTROL Breakdown]可视化图表按渠道或接触点划分每个所选归因模型的转化。 此可视化图表有助于确定每个渠道或接触点的有效性。

要选择划分类型，请从![更多](/help/assets/icons/More.svg)中选择&#x200B;**[!UICONTROL Breakdown by channel]**&#x200B;或&#x200B;**[!UICONTROL Breakdown by touchpoint]**。

要查看详细信息，请将鼠标悬停在任何图表元素上。

### [!UICONTROL Top campaigns]

热门促销活动可视化图表显示排名最前的促销活动列表，其中包含“促销活动名称”、“渠道”、“媒体类型”和“增量转化”列。 此可视化图表有助于让您的团队了解特定渠道的特定营销活动的有效性，并深入了解您应该进一步投资哪些营销活动。

要按“渠道”、“媒体类型”或“增量转化”的升↑或降序↓序对表进行排序，请选择列标题并切换排序。

要在单独的对话框中展开表，请从![更多](/help/assets/icons/More.svg)中选择&#x200B;**[!UICONTROL Expand]**。

展开的“热门促销活动”对话框显示的表格及其添加列

* 增量转化
* 受影响的转化
* 首次触点转化
* 最近联系转化

  您可以选择每个附加的列标题，以按升序或降序对表进行排序。

要关闭展开的“热门促销活动”对话框，请选择&#x200B;**[!UICONTROL Close]**。


### [!UICONTROL Breakdown by touchpoint position]

[!UICONTROL Breakdown by touchpoint position]可视化图表是按接触点位置及所有转化路径上的接触点划分的已归因转化。 此图表可帮助您比较某个接触点在某个位置的贡献是否优于其他位置以及在任何位置的其他接触点。

>[!NOTE]
>
>归因模型在所有接触点和位置的贡献百分比之和应等于100。


职位[!UICONTROL Starter]、[!UICONTROL Player]和[!UICONTROL Closer]的定义如下：

| 位置 | 描述 |
|---|---|
| [!UICONTROL Starter] | 此位置指示接触点是否为转化路径中的首次触点。 |
| [!UICONTROL Player] | 此位置指示接触点不是导致转化的首次接触还是最后接触。 |
| [!UICONTROL Closer] | 此位置指示接触点是否为转化前的最后一次触点。 |


### [!UICONTROL Top conversion paths]

[!UICONTROL Top conversion paths]可视化图表根据选定的归因模型显示前5个转化路径。

对于每个转换路径，您会看到：

* 有影响的渠道的数量，
* 已归因路径总数，
* 此转化路径的已归因路径与已归因路径总数的百分比，
* 对于每个渠道，归因模型贡献百分比和
* 这些渠道归因模型贡献百分比的总和。

## **[!UICONTROL Factors]**

“因子”选项卡显示外部因子相关的见解。

![因素](/help/assets/factors.png)

此可视化图表可帮助您了解各种内部和外部因素对转化基线的增量影响。 例如，经济条件或促销活动。


要下载包含该表数据的CSV文件，请选择![下载](/help/assets/icons/Download.svg)。

如果没有可用数据，您会看到一条消息![TableAndChart](/help/assets/icons/TableAndChart.svg) **[!UICONTROL No data is available, you may need to retrain your model, or change the date range to view insights]**。

## [!UICONTROL Diagnostics]

“诊断”选项卡显示以下各项的可视化图表：

* [!UICONTROL Model Assessment]可视化图表，可按实际转化与预测转化或残差转化进行划分。

  要划分可视化图表，请从&#x200B;**[!UICONTROL Breakdown]**&#x200B;列表中选择&#x200B;**[!UICONTROL Actual vs. Predicted]**&#x200B;或&#x200B;**[!UICONTROL Residuals]**。

* [!UICONTROL Model fitting metrics]表，显示每个转化量度的以下列：

   * 实际转化

   * 模型化转化

   * 剩余转化（实际转化与模型转化之间的差异）

   * 模型质量得分值：

      * R2（R平方），它表明数据拟合回归模型（拟合优度）的程度。

      * MAPE（平均绝对误差百分比），最常用于测量预测准确度的KPI之一，它以实际值的百分比表示预测误差。

      * RMSE（均方根误差）：显示平均误差，根据误差的平方进行加权。

  要下载包含该表数据的CSV文件，请选择![下载](/help/assets/icons/Download.svg)。

* [!UICONTROL Touchpoint effectiveness]表，表示Attribution AI算法模型的结果。 此表的数据仅为特定时间段生成。 选择&#x200B;**[!UICONTROL As of *xx/xx/xx， xx：xx TZ *]**![信息](/help/assets/icons/InfoOutline.svg)以了解更多详细信息。

  该可视化图表按降序显示每个接触点的[!UICONTROL Efficiency measure] ![降序](/help/assets/icons/SortOrderDown.svg)：

   * [!UICONTROL Paths touched]：可视化实现转化的路径百分比和未实现转化的路径百分比。 对于接触点，当归因转化率较高时，您会看到更多归因转化。 此比率将导致转化的路径百分比与&#x200B;*不会*&#x200B;导致转化的路径百分比进行比较。
   * [!UICONTROL Efficiency measure]：由算法归因模型生成，效率度量指示接触点对转化的相对重要性，与接触点数量无关。 效率在1到5的刻度上测量。 请注意，接触点数量越大并不能保证效率测量值越高。
   * [!UICONTROL Total volume]：用户接触接触点的总次数。 该数字包括出现在实现转化的路径上的接触点以及导致转化的路径&#x200B;*而非*。

![诊断](/help/assets/model-insights-diagnostics.png)


## [!UICONTROL Historical overview]

“历史概述”选项卡显示以下各项的可视化图表：

* 按财政季度和产品划分的转化和支出。

* 按渠道支出。

* 接触点支出。

  您可以为此可视化图表选择要显示的替代基于支出的渠道。 从&#x200B;**[!UICONTROL Channels]**&#x200B;中选择一个渠道。

* 接触点数量。

  您可以为此可视化图表选择要显示的替代基于卷的渠道。 从&#x200B;**[!UICONTROL Channels]**&#x200B;中选择一个渠道。

![模型 — 历史概述](/help/assets/model-insights-historical-overview.png)
