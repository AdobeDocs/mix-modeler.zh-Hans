---
title: 训练模型并为其评分
description: 了解如何训练和评分模型。
feature: Models
source-git-commit: 6855d19347b7f6f1477a6265310df5950b8463c9
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# 训练模型并为其评分

在您[构建](/help/models/build.md)模型后，将自动对模型进行训练和评分。 您可以手动重新训练或重新核心模型。

## 训练

当您想要包含新的增量营销和因子数据时，请考虑重新训练模型。 例如，在上一季度，市场动态发生了变化或者您的营销数据分发发生了显着变化。

要重新训练模型，请执行以下操作：

1. 从左边栏中选择![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**。

1. 为模型选择![更多](/help/assets/icons/More.svg)，然后从上下文菜单中选择&#x200B;**[!UICONTROL Train]**。 或者，从蓝色操作栏中选择![DataRefresh](/help/assets/icons/DataRefresh.svg) **[!UICONTROL Train]**。

   在&#x200B;**[!UICONTROL Train model]**&#x200B;对话框中，选择选项以：

   * **[!UICONTROL Train model with last 2 years of marketing data]**，或
   * **[!UICONTROL Train model using specific date range of data]**。
指定日期范围。 您可以使用![日历](/help/assets/icons/Calendar.svg)选择日期范围。 您必须选择至少一年的数据范围。

   ![重新训练模型](../assets/retrain-model.png)

1. 选择&#x200B;**[!UICONTROL Train]**&#x200B;以重新训练模型。


只有成功训练模型后，才能重新训练模型。


## 得分


您可以根据新的营销数据对模型递增计分，或针对特定日期范围对模型重新计分。

在执行以下操作时，请考虑重新核心模型：

* 更正不正确的营销数据。 例如，您在模型的训练和评分中包含的最近付费搜索数据漏掉了一周的数据。
* 使用新的增量营销数据，该数据可通过您配置作为协调数据一部分的数据集的更新获取。

要对模型评分或重新排序，请执行以下操作：

1. 从左边栏中选择![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**。

1. 为模型选择![更多](/help/assets/icons/More.svg)，然后从上下文菜单中选择&#x200B;**[!UICONTROL Score]**。 或者，从蓝色操作栏中选择![DataRefresh](/help/assets/icons/DataRefresh.svg) **[!UICONTROL Score]**。

   在&#x200B;**[!UICONTROL Score marketing data]**&#x200B;对话框中，选择选项以：

   * **[!UICONTROL Score new marketing data from *mm/dd/yyyy *]**，使用新的营销数据对模型进行增量评分，或
   * **[!UICONTROL Score specific date range of marketing data]**&#x200B;以重新核在特定日期范围内。
指定日期范围。 您可以使用![日历](/help/assets/icons/Calendar.svg)选择日期范围。

   ![重新核心模型](../assets/rescore-model.png)

1. 选择&#x200B;**[!UICONTROL Score]**。 使用特定数据范围对模型重新评分时，您会看到&#x200B;**[!UICONTROL Existing model is replaced]**&#x200B;对话框，提示您确认使用选定日期范围的新得分替换模型。 选择&#x200B;**[!UICONTROL Replace model]**&#x200B;以确认。

>[!IMPORTANT]
>
>重新核心模型不会更改已基于重新核心模型创建的任何“计划”。 要在计划中使用新重新整理的模型，您必须创建一个新计划。

