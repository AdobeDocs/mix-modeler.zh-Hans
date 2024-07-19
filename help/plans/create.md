---
title: 创建计划
description: 了解如何在Mix Modeler中创建计划。
feature: Plans
exl-id: 6d61d0b2-5871-4d00-9a35-73fff0a1c3e5
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---


# 创建计划

在Mix Modeler中，您可以使用计划画布创建计划。 在计划画布中，您可以设置计划的详细信息和预算，以及要用于计划的基础模型。 指定详细信息、预算和模型后，您可以继续使用人工智能推荐的计划或编辑按渠道划分的支出。

要创建计划，请在Mix Modeler的![PLan](/help/assets//icons/FileChart.svg) **[!UICONTROL Plans]**&#x200B;界面中选择&#x200B;**[!UICONTROL Open plan canvas]**。

1. 在“计划创建”屏幕中：

   1. 在&#x200B;**[!UICONTROL Setup]**&#x200B;部分中

      1. 输入&#x200B;**[!UICONTROL Plan name]**，例如`Demo plan`。 输入&#x200B;**[!UICONTROL Description]**，例如`Demo plan for Luma company`。
      1. 从&#x200B;**[!UICONTROL _中选择&#x200B;**[!UICONTROL Model]**选择一个选项……_.]**。
      1. 您可以选择![LinkOut](/help/assets//icons/LinkOut.svg) **[!UICONTROL Create model]**&#x200B;直接从计划创建中创建模型。 这将在您的浏览器中打开一个新选项卡，并显示[模型](../models/overview.md)界面。

         ![计划设置](/help/assets//plan-setup.png)

   1. 在&#x200B;**[!UICONTROL Budget]**&#x200B;部分中：

      1. 通过键入日期或使用![日历](/help/assets//icons/Calendar.svg)选择日期范围来指定日期范围。
      1. 输入预算。

      若要添加其他日期范围（每个日期范围都有预算），请选择![日历添加](/help/assets//icons/CalendarAdd.svg) **[!UICONTROL Add row]**。

      要删除日期范围和相关预算，请选择![关闭](/help/assets//icons/Close.svg)。

      要定义指定的最大预算，请执行以下操作：

      1. 打开&#x200B;**[!UICONTROL Maximize budget]**。
      1. 指定最大预算金额。 金额应等于或高于为日期范围指定的预算总额。

         ![计划预算](/help/assets//plan-budget.png)

   1. 选择 **[!UICONTROL Next]**。

1. 在&#x200B;**[!UICONTROL Done with all required fields]**&#x200B;对话框中：

   ![计划完成](/help/assets//plan-done-required-fields.png)

   * 选择 <img src="/help/assets//icons/NewPlan.svg" width="25" /> **[!UICONTROL Create plan now]**（如果要生成具有预测的ROI的AI推荐计划）。

     选择&#x200B;**[!UICONTROL OK]**。 您的计划已创建。


   * 如果您要在创建具有预测的ROI的计划之前编辑渠道预算，请选择![TableEdit](/help/assets//icons/TableEdit.svg) **[!UICONTROL Edit channel budgets first]**。

     选择&#x200B;**[!UICONTROL OK]**，这样您就可以在下一步的&#x200B;**[!UICONTROL Spend selection]**&#x200B;中定义渠道支出。



1. 在&#x200B;**[!UICONTROL Spend selection]**&#x200B;部分中，对于每个预算日期范围，使用![V形](/help/assets//icons/ChevronRight.svg)顶部打开该数据范围的渠道分发视图。

   1. 要定义每个渠道的预算，请为&#x200B;**[!UICONTROL Min]**&#x200B;和&#x200B;**[!UICONTROL Max]**&#x200B;输入值或使用滑块。

   1. 要在货币或百分比输入之间切换，请为&#x200B;**[!UICONTROL View spend by]**&#x200B;选择&#x200B;**[!UICONTROL $]**&#x200B;或&#x200B;**[!UICONTROL %]**。

      ![花费选择](/help/assets//plan-spend-selection.png)

   1. 完成后，选择&#x200B;**[!UICONTROL Create]**。

   1. 在&#x200B;**[!UICONTROL Create plan]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL Create plan]**&#x200B;以创建您的计划。 选择&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消计划的创建。 将显示&#x200B;**[!UICONTROL No work is saved]**&#x200B;对话框以确认。
