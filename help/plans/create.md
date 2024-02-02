---
title: 创建计划
description: 了解如何在Mix Modeler中创建计划。
feature: Plans
exl-id: 6d61d0b2-5871-4d00-9a35-73fff0a1c3e5
source-git-commit: 86732fe30637aa72ced232d9f331a3cc64baa39b
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---


# 创建计划

在Mix Modeler中，您可以使用计划画布创建计划。 在计划画布中，您可以设置计划的详细信息和预算，以及要用于计划的基础模型。 指定详细信息、预算和模型后，您可以继续使用人工智能推荐的计划或编辑按渠道划分的支出。

要创建计划，请在 ![PLan](../assets/icons/FileChart.svg) **[!UICONTROL Plans]** 界面中，选择Mix Modeler **[!UICONTROL Open plan canvas]**.

1. 在“计划创建”屏幕中：

   1. 在 **[!UICONTROL Setup]** 部分

      1. 输入 **[!UICONTROL Plan name]**&#x200B;例如 `Demo plan`. 输入 **[!UICONTROL Description]**&#x200B;例如 `Demo plan for Luma company`.
      1. 选择 **[!UICONTROL Model]** 从 **[!UICONTROL _选择一个选项……_.]**.
      1. 您可以选择 ![链接输出](../assets/icons/LinkOut.svg) **[!UICONTROL Create model]** 在计划创建中直接创建模型。 这将在您的浏览器中打开一个新选项卡，并显示 [模型](../models/overview.md) 界面。

         ![计划设置](../assets/plan-setup.png)

   1. 在 **[!UICONTROL Budget]** 部分：

      1. 通过键入日期或使用以下方式选择日期范围来指定日期范围 ![日历](../assets/icons/Calendar.svg).
      1. 输入预算。

      要添加额外的日期范围（每个日期范围都有预算），请选择 ![CalendarAdd](../assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**.

      要删除日期范围和关联的预算，请选择 ![关闭](../assets/icons/Close.svg).

      要定义指定的最大预算，请执行以下操作：

      1. 切换 **[!UICONTROL Maximize budget]** 打开。
      1. 指定最大预算金额。 金额应等于或高于为日期范围指定的预算总额。

         ![计划预算](../assets/plan-budget.png)

   1. 选择 **[!UICONTROL Next]**。

1. 在 **[!UICONTROL Done with all required fields]** 对话框：

   ![已完成计划](../assets/plan-done-required-fields.png)

   * 选择 <img src="../assets/icons/NewPlan.svg" width="25" /> **[!UICONTROL Create plan now]** 如果要生成具有预测的ROI的AI推荐计划，请执行以下操作。

     选择 **[!UICONTROL OK]**. 您的计划已创建。


   * 选择 ![表编辑](../assets/icons/TableEdit.svg) **[!UICONTROL Edit channel budgets first]** 如果您要在创建具有预测ROI的计划之前编辑渠道预算。

     选择 **[!UICONTROL OK]**，以便您能够在以下位置定义渠道支出： **[!UICONTROL Spend selection]** 在下一步中。



1. 在 **[!UICONTROL Spend selection]** 部分，对于每个预算日期范围，使用 ![V形](../assets/icons/ChevronRight.svg) 顶部打开该数据范围的渠道分布视图。

   1. 要定义每个渠道的预算，请输入值 **[!UICONTROL Min]** 和 **[!UICONTROL Max]** 或者用滑块。

   1. 要在货币或百分比输入之间切换，请选择 **[!UICONTROL $]** 或 **[!UICONTROL %]** 对象 **[!UICONTROL View spend by]**.

      ![支出选择](../assets/plan-spend-selection.png)

   1. 完成后，选择 **[!UICONTROL Create]**.

   1. 在 **[!UICONTROL Create plan]** 对话框，选择 **[!UICONTROL Create plan]** 以创建您的计划。 选择 **[!UICONTROL Cancel]** 以取消计划的创建。 A **[!UICONTROL No work is saved]** 将显示对话框以确认。
