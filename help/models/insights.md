---
title: 模型洞察
description: 了解如何获取有关模型的详细信息，如Mix Modeler中的历史概述、模型见解和模型质量。
feature: Models
exl-id: d99852f9-ba0d-4a2e-b5f3-ca0efe6002fd
source-git-commit: bc48dc564042890856072a07c3a9715ba9dcdb87
workflow-type: tm+mt
source-wordcount: '1914'
ht-degree: 0%

---

# 模型洞察

模型分析中的每个可视化图表都旨在帮助您：

* 可视化和量化您组织的营销活动的影响。
* 确定哪些渠道表现良好。
* 确定可能需要优化的渠道。

然后，这些见解可帮助您支持资源优先顺序和分配。

要查看模型分析，请在Mix Modeler的![模型](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**&#x200B;界面中：

1. 从&#x200B;**[!UICONTROL Models]**&#x200B;表中，选择&#x200B;**[!UICONTROL Last run status]**&#x200B;为<span style="color:green">●</span>的模型的名称 **[!UICONTROL Success]**。

1. 从上下文菜单中选择&#x200B;**[!UICONTROL Model Insights]**。

![模型分析选项卡栏](/help/assets/model-insights-tabbar.png)

您会看到指定模型上次刷新的时间，并使用四个选项卡显示可视化图表：[模型分析](#model-insights)、[归因](#attribution)、[因素](#factors)、[诊断](#diagnostics)和[历史概述](#historical-overview)。

您可以更改每个选项卡上的可视化图表所基于的日期段。 输入日期期间或选择![日历](/help/assets/icons/Calendar.svg)以选择日期期间。

## [!UICONTROL Model insights]

“模型见解”选项卡显示[按日期和基础媒体显示的贡献](#contribution-by-date-and-base-media)、[按渠道显示的贡献](#contribution-by-channel)、[营销业绩摘要](#marketing-performance-summary)和[边际响应曲线](#marginal-response-curves)的可视化。 该选项卡还提供了[接触点细分](#touchppint-breakdown)表。

![模型 — 模型见解](/help/assets/model-insights-insights.png)

* 您可以将鼠标悬停在每个可视化的个别图表元素上，以显示包含更多详细信息的弹出窗口。

* 要下载包含可视化图表数据的CSV文件，请选择![下载](/help/assets/icons/Download.svg)。

* 要以Microsoft® Excel格式下载完整的模型分析数据，请选择![下载](/help/assets/icons/Download.svg) **[!UICONTROL Download data]**。


### 按日期和基本媒体列出的贡献。

此栈叠图形可视化图表的顺序如下：

* 底部的。
* 非支出渠道居于中间。
* 将渠道置顶。

此可视化图表表示在某个日期范围内按基础、支出渠道和非支出渠道实现的贡献比例。 此可视化图表有助于展示增量功能。 基本信息表示在没有任何营销的情况下会发生什么，非支出渠道加上支出渠道（在基本信息的基础上）归因于营销影响。 简言之，非支出加支出等于营销工作的增量影响，可视化图表可让您轻松了解insight营销产生的价值。

### 按渠道显示的贡献

一个圆环图可视化图表，可显示各个渠道的贡献分布。 此可视化图表通过前三个执行渠道的镜头（不包括基本和&#x200B;*所有其他*&#x200B;类别）展示递增性。 该可视化图表有助于支持优先级和预算分配。

### 营销绩效摘要。

显示每个通道的ROI或CPA性能的水平条形图可视化。 此可视化图表突出显示您的营销投资的ROI/CPA。 通道根据ROI/CPA按降序排列。 可视化有助于识别哪些渠道最有效以及哪些渠道可能需要优化。

### 边际响应曲线。

折线图可可视化并比较营销渠道投资产生的边际回报。  并找出盈亏平衡点，即递增回报低于递增支出。 因此，此可视化图表可帮助您了解营销投资何时开始变得不那么有影响力。

曲线、平衡点和相应值将根据选定的数据范围和选定的通道进行计算。

要更改频道，请执行以下操作：

* 从&#x200B;**[!UICONTROL Channel]**&#x200B;下拉菜单中选择一个频道以更新特定频道的可视化。


### 接触点细分

接触点细分表以每周为基数显示所有或选定通道的每周接触点细分，显示与每个通道关联的关键指标。 该表便于在更精细的渠道级别进行比较、趋势识别和性能跟踪。 此表明确补充了[按日期和基本媒体列出的贡献](#contribution-by-date-and-base-media)可视化图表和[按渠道列出的贡献](#contribution-by-channel)可视化图表。

![接触点细分](../assets/touchpoint-breakdown.png)

可使用以下列：

| 列 | 描述 |
|---|---|
| **[!UICONTROL Date range]** | 要报告的周。 |
| **[!UICONTROL Touchpoint]** | 特定接触点通道。 |
| **[!UICONTROL ROI]** | (**[!UICONTROL Revenue]** - **[!UICONTROL Spend]**) / **[!UICONTROL Spend]**&#x200B;的百分比。 |
| **[!UICONTROL Revenue]** | 日期范围的收入。 |
| **[!UICONTROL CPA]** | **[!UICONTROL Spend]** / **[!UICONTROL Conversions]**。 |
| **[!UICONTROL Conversions]** | 日期范围的转化。 |
| **[!UICONTROL Spend]** | 数据范围的开销。 |

要选择特定频道或所有频道，请从&#x200B;**[!UICONTROL View]**&#x200B;下拉菜单中选择。

若要下载接触点细分表的内容，请选择![下载](/help/assets/icons/Download.svg) **[!UICONTROL Download CSV]**。

## **[!UICONTROL Factors]** [!BADGE 测试版]

因子[!BADGE 测试版]选项卡显示外部因子相关见解。

![因素](/help/assets/factors.png)

此可视化图表可帮助您了解各种内部和外部因素对转化基线的增量影响。 例如，经济条件或促销活动。

使用&#x200B;**[!UICONTROL Factors]**&#x200B;下拉菜单选择要显示的因子。

<!-- need to update the image when we do have a proper example -->

要下载包含该表数据的CSV文件，请选择![下载](/help/assets/icons/Download.svg)。

如果没有可用的数据，您将看到消息![TableAndChart](/help/assets/icons/TableAndChart.svg) **[!UICONTROL No data is available, you may need to retrain your model, or change the date range to view insights]**。

## [!UICONTROL Attribution]

>[!NOTE]
>
>“属性”选项卡仅适用于已启用MTA的模型。


使用[!UICONTROL Attribution]选项卡，您可以了解具有事件级别数据的接触点和营销活动的有效性。  请参阅[构建模型](build.md)。

支持以下归因模型：

* 基于Mix Modeler中选择的模型：
   * 算法 — 影响输出
   * 算法 — 增量
* 基于规则：
   * 衰减单位
   * 首次接触
   * 最近联系
   * 线性
   * Ushape

有关Mix Modeler中多点触控归因功能的介绍，请参阅[多点触控归因](../get-started/about.md#multi-touch-attribution)。

从&#x200B;**[!UICONTROL Attribution Model]**&#x200B;下拉菜单中选择一个或多个归因模型。 选定的归因模型适用于“归因”选项卡中的所有可视化。

![归因](/help/assets/model-insights-attribution.png)

Mix Modeler多点接触归因粒度事件得分与总体Mix Modeler得分和ROI相符。 这些得分也可作为Experience Platform中的数据集使用。

归因选项卡包含以下可视化图表：

### [!UICONTROL Overview]

[!UICONTROL Overview]可视化图表显示选定归因模型的转化合计和百分比。 选择更多模型会为可视化图表添加其他圆，每个圆都有自己的颜色与图例相对应。

要查看包含归因模型详细信息的弹出窗口，请将光标悬停在可视化图表中的任何圆圈上。

### [!UICONTROL Trends]

[!UICONTROL Daily trends]、[!UICONTROL Weekly trends]或[!UICONTROL Monthly trends]可视化图表显示选定归因模型的每日、每周或每月转化趋势。

要选择期间，请从![更多](/help/assets/icons/More.svg)中选择&#x200B;**[!UICONTROL Daily trends]**、**[!UICONTROL Weekly trends]**&#x200B;或&#x200B;**[!UICONTROL Monthly trends]**。

要查看详细信息，请将鼠标悬停在特定归因模型的数据行上以显示一个弹出窗口，其中显示该数据的转化总数。

### [!UICONTROL Breakdown]

[!UICONTROL Breakdown]可视化图表按渠道或接触点划分每个所选归因模型的转化。 此可视化图表有助于确定每个渠道或接触点的有效性。

要选择划分类型，请从![更多](/help/assets/icons/More.svg)中选择&#x200B;**[!UICONTROL Breakdown by channel]**&#x200B;或&#x200B;**[!UICONTROL Breakdown by touchpoint]**。

要查看详细信息，请将鼠标悬停在任何图表元素上。

### [!UICONTROL Top campaigns]

热门促销活动可视化图表显示排名最前的促销活动列表，其中包含“促销活动名称”、“渠道”、“媒体类型”和“增量转化”列。 此可视化可帮助让您的团队了解特定渠道的特定营销活动的有效性，并提供关于您应进一步投资哪些营销活动的深入见解。

要按“渠道”、“媒体类型”或“增量转化”的升↑或降序↓序对表进行排序，请选择列标题并切换排序。

要在单独的对话框中展开表，请从![更多](/help/assets/icons/More.svg)中选择&#x200B;**[!UICONTROL Expand]**。

展开的“热门促销活动”对话框显示的表格及其添加列

* 增量转化
* 受影响的转化
* 首次触控转换
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
| [!UICONTROL Player] | 此位置指示接触点不是导致转换的第一个接触点还是最后一个接触点。 |
| [!UICONTROL Closer] | 此位置指示接触点是否为转化前的最后一次触点。 |


### [!UICONTROL Top conversion paths]

[!UICONTROL Top conversion paths]可视化图表根据选定的归因模型显示前5个转化路径。

对于每个转换路径，您会看到：

* 有影响的渠道的数量，
* 已归因路径总数，
* 此转换路径的属性化路径与总属性化路径的百分比，
* 对于每个渠道，归因模型贡献百分比，以及
* 这些通道归因模式贡献百分比的总和。


## [!UICONTROL Diagnostics]

“诊断”选项卡显示以下各项的可视化：

* [!UICONTROL Model Assessment]可视化，您可以按实际与预测或残差转换细分。

  要划分可视化图表，请从&#x200B;**[!UICONTROL Breakdown]**&#x200B;列表中选择&#x200B;**[!UICONTROL Actual vs. Predicted]**&#x200B;或&#x200B;**[!UICONTROL Residuals]**。

* [!UICONTROL Model fitting metrics]表，显示每个转化量度的以下列：

   * 实际转化

   * 模型化转化

   * 剩余折换（实际折换与模型折换之间的差异）

   * 模型质量分数值：

      * R2（R平方），它表明数据拟合回归模型（拟合优度）的程度。

      * MAPE（平均绝对误差百分比），最常用于测量预测准确度的KPI之一，它以实际值的百分比表示预测误差。

      * RMSE（均方根误差）：显示平均误差，根据误差的平方进行加权。

  要下载包含该表数据的CSV文件，请选择![下载](/help/assets/icons/Download.svg)。

* [!UICONTROL Touchpoint effectiveness]表，表示归因人工智能算法模型的结果。 此表的数据仅为特定时间段生成。 选择&#x200B;**[!UICONTROL As of *xx/xx/xx， xx：xx TZ *]**![信息](/help/assets/icons/InfoOutline.svg)以了解更多详细信息。

  该可视化图表按降序显示每个接触点的[!UICONTROL Efficiency measure] ![降序](/help/assets/icons/SortOrderDown.svg)：

   * [!UICONTROL Paths touched]：可视化实现转化的路径百分比和未实现转化的路径百分比。 对于接触点，当归因转化率较高时，您会看到更多归因转化。 此比率将导致转化的路径百分比与&#x200B;*不会*&#x200B;导致转化的路径百分比进行比较。
   * [!UICONTROL Efficiency measure]：由算法归因模型生成，效率度量指示接触点对于转换的相对重要性，与接触点体积无关。 效率在1到5的范围内测量。 请注意，较高的接触点体积并不能保证较高的效率测量。
   * [!UICONTROL Total volume]：用户接触接触点的聚合次数。 该数字包括出现在实现转换的路径上的接触点以及导致转换的路径&#x200B;*不是*。

![诊断](/help/assets/model-insights-diagnostics.png)


## [!UICONTROL Historical overview]

“历史概述”选项卡显示以下各项的可视化图表：

![模型 — 历史概述](/help/assets/model-insights-historical-overview.png)


### 按财政季度和产品划分的转化和支出

此可视化图表表示给定日期范围内各个季度的转化和支出分布。 该可视化图表有助于识别支出推动转化的高性能季度。


### 按渠道支出

此可视化图表表示给定日期范围内各个渠道的支出分布。 该可视化图表支持快速识别哪些渠道的支出最多。


### Touchpoint支出

此可视化图表表示给定日期范围内每个季度的付费接触点之间的支出分布。 通过可视化，可了解在特定渠道和季度中哪些接触点被优先处理。 可视化有助于识别渠道支出模式和趋势，特别是在一段时间内支出较少且不频繁的渠道。

要为此可视化图表选择要显示的替代基于支出的渠道，请执行以下操作：

* 从&#x200B;**[!UICONTROL Channels]**&#x200B;中选择一个渠道。


### 接触点数量

此可视化图表表示给定日期范围内每个季度所有接触点的数量分布。

要为此可视化图表选择要显示的替代基于卷的渠道，请执行以下操作：

* 从&#x200B;**[!UICONTROL Channels]**&#x200B;中选择一个频道。


## **[!UICONTROL Edit]**

您可以编辑模型的名称、说明以及训练和评分的安排。

1. 选择![编辑](/help/assets/icons/Edit.svg)编辑

1. 在&#x200B;**[!UICONTROL Edit model]**&#x200B;对话框中：

   * 输入新的&#x200B;**[!UICONTROL Name]**&#x200B;和&#x200B;**[!UICONTROL Description]**。

   * 要启用计划，请启用&#x200B;**[!UICONTROL Status]**。 您只能为经过训练和评分的模型启用计划。

      1. 选择&#x200B;**[!UICONTROL Scoring frequency]**：

         * **[!UICONTROL Daily]**：输入有效时间（例如`05:22 pm`）或使用![时钟](/help/assets/icons/Clock.svg)。
         * **[!UICONTROL Weekly]**：选择一周中的某一天并输入有效时间（例如`05:22 pm`）或使用![时钟](/help/assets/icons/Clock.svg)。
         * **[!UICONTROL Monthly]**：从“在每次运行时运行”下拉菜单中选择一个月中的某一天，并输入有效时间（例如`05:22 pm`）或使用![时钟](/help/assets/icons/Clock.svg)。

      1. 从下拉菜单中选择&#x200B;**[!UICONTROL Training frequency]**： **[!UICONTROL Monthly]**、**[!UICONTROL Quarterly]**、**[!UICONTROL Yearly]**&#x200B;或&#x200B;**[!UICONTROL None]**。

     ![编辑模型](../assets/model-edit.png)

1. 选择 **[!UICONTROL Save]**。
