---
title: 模型分析
description: 了解如何在Adobe组合建模器中获取有关模型的详细信息，如历史概述、模型见解和模型质量。
feature: Models
source-git-commit: ac17f5a9fcf036c8e689879578e4b745b789cea3
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# 模型分析

要查看模型洞察，请在 ![模型](../assets/icons/FileData.svg) **[!UICONTROL Models]** Adobe组合建模器中的接口：

1. 选择模型名称 **[!UICONTROL Last run status]** 之 <span style="color:green">●</span> **[!UICONTROL Success]** 从 **[!UICONTROL Models]** 表格。

1. 从上下文菜单中，选择 **[!UICONTROL Model Insights]**.

您会看到指定模型的上次刷新时间，并且小组件使用三个选项卡显示：历史概述、模型洞察和模型质量。

您可以更改每个选项卡上的小组件所基于的日期段。 输入日期期间或选择 ![日历](../assets/icons/Calendar.svg) 以选择日期期间。


## 历史概述

“历史概述”选项卡显示以下各项的小部件：

* 按财政季度和产品划分的转化和支出

* 按渠道支出

* 接触点支出

  您可以为此小组件选择一个要显示的基于支出的替代渠道。 从中选择渠道 **[!UICONTROL Channels]**.

* 接触点数量

  您可以选择为此小组件显示的替代的基于卷的渠道。 从中选择渠道 **[!UICONTROL Channels]**.



![模型 — 历史概述](../assets/model-historical-overview.png)


## 模型洞察

模型分析选项卡显示以下构件：

* 按日期和基本媒体列出的贡献

* 按渠道列出的贡献

* 营销绩效摘要

您可以将鼠标悬停在每个小组件中的单个图表元素上，以查看包含更多详细信息的弹出框。

![模型 — 模型洞察](../assets/model-model-insights.png)


## 模型质量

“模型质量”选项卡显示用于测量的构件：

* R2（R平方），它表明数据拟合回归模型（拟合优度）的程度。

* MAPE（平均绝对误差百分比），最常用于测量预测准确度的KPI之一，它以实际值的百分比表示预测误差。

* RMSE（均方根误差）：显示平均“误差”，根据误差的平方进行加权。


