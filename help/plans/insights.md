---
title: 计划洞察
description: 了解如何在Mix Modeler中查看计划的见解并编辑计划。
feature: Plans
exl-id: 91385595-284f-4fcb-b54b-9539905e552b
source-git-commit: fbed53a1c394d6d110db6a8a181ca815056377de
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# 计划洞察


在[!UICONTROL Plan insights]中创建您的计划分析，显示计划所基于的[!UICONTROL Model]、[!UICONTROL Data range]和[!UICONTROL Total budget]。

完成检索后，您将看到计划的概览，包括：

- [!UICONTROL Forecasted paid channel ROI]可视化图表
- [!UICONTROL Forecasted revenue]可视化图表
- [!UICONTROL Forecasted conversion]可视化图表
- [!UICONTROL Marginal channel return]可视化图表
- 计划的[!UICONTROL Data range breakdown]表，显示列

   - 渠道
   - ROI
   - CPA
   - 收入
   - 转化目标
   - 支出

要关闭该界面，请选择&#x200B;**[!UICONTROL Close]**。

若要更改查看计划ROI的方式，请在&#x200B;**[!UICONTROL View ROI]**&#x200B;中选择&#x200B;**[!UICONTROL X]**&#x200B;或&#x200B;**[!UICONTROL  %]**。

## 预测的付费渠道支出和ROI

此可视化图表根据模型、日期范围和预算，显示付费渠道上预测支出和投资回报的散点图。

![预测的付费渠道支出和ROI可视化图表](../assets/overview-plan-forecasted-paid-channel-send-roi.png)


## 预测收入

此条形图可视化图表根据模型、日期范围和预算显示渠道的预测收入。

![预测收入可视化图表](../assets/overview-plan-forecasted-revenue.png)


## 预测的转化

此条形图可视化图表根据模型、日期范围和预算显示渠道的预测转化。

![预测转化可视化图表](../assets/overview-plan-forecasted-conversions.png)


## 边际渠道回报

此折线图可视化图表显示所选渠道的边际返回曲线，其中包含&#x200B;**[!UICONTROL Marginal break-even]**&#x200B;和&#x200B;**[!UICONTROL Return point]**&#x200B;的指标。 此可视化图表可帮助您了解渠道支出如何从达到边际盈亏平衡点开始，以及您是否有空间增加渠道支出还是应该减少渠道支出以提高渠道支出效率。

![边际渠道回报可视化](../assets/overview-plan-marginal-channel-return.png)

要为可视化图表选择特定渠道，请从&#x200B;**[!UICONTROL View]**&#x200B;下拉菜单中选择一个渠道。


## 日期范围细分

[!UICONTROL Date range breakdown]表显示[!UICONTROL ROI]、[!UICONTROL Revenue]、[!UICONTROL CPA]、[!UICONTROL Conversions]和[!UICONTROL Spend]的每通道详细的粒度数据。

![日期范围划分表](../assets/overview-plan-date-range-breakdown.png)

1. 要下载包含日期范围划分数据的CSV文件，请选择![下载](/help/assets/icons/Download.svg) **[!UICONTROL Download CSV]**。 从上下文菜单中：

   - 为CSV格式的详细数据选择![下载](/help/assets/icons/Download.svg) **[!UICONTROL Detailed CSV]**。
   - 为CSV格式的摘要数据选择![下载](/help/assets/icons/Download.svg) **[!UICONTROL Summary CSV]**。

   详细数据是按周划分键的细粒度数据。 摘要数据由模型提供的日期范围作为数据键。

1. 要查看按渠道类别划分的日期范围细分，请从&#x200B;**[!UICONTROL View]**&#x200B;选项中选择&#x200B;**[!UICONTROL All channels]**、**[!UICONTROL Paid channels]**&#x200B;或&#x200B;**[!UICONTROL Non-paid channels]**。


## 编辑计划

1. 要编辑计划，请选择![编辑](/help/assets/icons/Edit.svg) **[!UICONTROL Edit plan]**：

   1. 在&#x200B;**[!UICONTROL Spend selection]**&#x200B;部分中，对于每个预算日期范围，使用![V形](/help/assets/icons/ChevronRight.svg)打开该数据范围的渠道分配视图。

   1. 要修改每个渠道的预算，请修改&#x200B;**[!UICONTROL Min]**&#x200B;和&#x200B;**[!UICONTROL Max]**&#x200B;的值或使用滑块。

   1. 要在货币或百分比输入之间切换，请为&#x200B;**[!UICONTROL View spend by]**&#x200B;选择&#x200B;**[!UICONTROL $]**&#x200B;或&#x200B;**[!UICONTROL %]**。

      ![花费选择](/help/assets/spend-selection.png)

   1. 要编辑计划的详细信息，请选择&#x200B;**[!UICONTROL Edit details]**：

      1. 在&#x200B;**[!UICONTROL Setup]**&#x200B;部分中，如果适用，修改&#x200B;**[!UICONTROL Plan name]**&#x200B;和&#x200B;**[!UICONTROL Description]**。

      1. 在&#x200B;**[!UICONTROL Budget]**&#x200B;部分中：

         1. 通过键入日期或使用![日历](/help/assets/icons/Calendar.svg)选择日期范围，修改一个或多个计划日期范围的&#x200B;**[!UICONTROL Date range]**。

         1. 为一个或多个计划的日期范围修改&#x200B;**[!UICONTROL Budget]**。

         若要添加其他日期范围（每个日期范围都有预算），请选择![日历添加](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**。

         要删除日期范围和相关预算，请选择![关闭](/help/assets/icons/Close.svg)。

         要定义最大预算，请执行以下操作：

         1. 打开&#x200B;**[!UICONTROL Maximize budget]**。
         1. 指定最大预算金额。 金额应等于或高于为日期范围指定的预算总额。

      1. 选择&#x200B;**[!UICONTROL Next]**&#x200B;以返回到&#x200B;**[!UICONTROL Spend]**&#x200B;分区。 选择&#x200B;**[!UICONTROL Cancel]**&#x200B;以返回计划概述。

         ![计划详细信息](/help/assets/plan-details.png)


1. 编辑完计划后，选择&#x200B;**[!UICONTROL Edit]**。

   在&#x200B;**[!UICONTROL All changes are final]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL OK]**&#x200B;以更新计划的当前支出分配以及ROI和收入预测。 选择&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消计划的更新。

1. 要取消计划更新，请选择&#x200B;**[!UICONTROL Cancel]**。

   在&#x200B;**[!UICONTROL No work will be saved]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL Cancel]**&#x200B;以继续处理您的计划，或者选择&#x200B;**[!UICONTROL OK]**&#x200B;以返回到“计划”界面。
