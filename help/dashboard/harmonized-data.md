---
title: 协调的数据概述仪表板
description: 了解如何在Adobe组合建模器中使用协调的数据概述仪表板。
feature: Dashboard, Harmonized Data
source-git-commit: abbfc78e9fa774a240d000131f35d3dc257c15ea
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---


# 统一的数据概述

Adobe组合Modeler概述中的“协调数据”标签提供了对协调数据的洞察，您已配置该数据作为所摄取数据和协调数据设置的一部分使用。

此概述显示了四个KPI状态卡小组件（顶行）和六个其他可配置小组件。

要更改小部件中显示数据的日期期间，请手动输入开始日期和结束日期，或使用以下方式选择期间 ![日历](../assets/icons/Calendar.svg).

## 数据过滤器

您可以使用以下工具筛选为所有小部件显示的数据： ![筛选](../assets/icons/Filter.svg) **[!UICONTROL Data Filters]** 窗格。

为每个类别选择一个或多个筛选器(**[!UICONTROL Channel]**， **[!UICONTROL Brand]**， **[!UICONTROL Source Type]**、和 **[!UICONTROL Traffic Source]**)。

所选过滤器显示在小组件的顶部 **[!UICONTROL FILTERING BY:]**.

1. 要删除单个过滤器，请选择 ![关闭](../assets/icons/Close.svg) 在筛选器上，列在 **[!UICONTROL FILTERING BY:]**.

1. 您可以使用以下方式快速清除所有过滤器 **[!UICONTROL Clear All]**.

![统一的数据概述](../assets/harmonized-data-overview.png)


## 配置构件

您可以配置每个构件。

* 在KPI状态卡小部件上：

   1. 选择 ![编辑](../assets/icons/Edit.svg) 和 ![编辑](../assets/icons/Edit.svg) **[!UICONTROL Edit Data]** 从上下文菜单中。

   1. 在 **[!UICONTROL KPI status card]** 对话框：

      1. 选择 **[!UICONTROL KPI]** 从名单上。

      1. 选择 **[!UICONTROL Apply]** 将更改应用到卡片。 选择 **[!UICONTROL Cancel]** 以取消更改。

* 在其他可配置的构件上：

   1. 选择 ![编辑](../assets/icons/Edit.svg) 和 ![编辑](../assets/icons/Edit.svg) **[!UICONTROL Edit Data]** 从上下文菜单中。

   1. 在 **[!UICONTROL Edit Data]** 对话框：

      1. 从中选择量度 **[!UICONTROL Select a metric]**&#x200B;例如 **[!UICONTROL Impressions]**.
      1. 从中选择类别 **[!UICONTROL Select category]**&#x200B;例如 **[!UICONTROL Media Type]**.
      1. （可选）从中选择第二个类别 **[!UICONTROL Select second category (optional)]**&#x200B;例如 **[!UICONTROL Traffic Source]**.
      1. 选择 ![时钟](../assets/icons/Clock.svg) **[!UICONTROL Time]** 或 ![计算器](../assets/icons/Calculator.svg) **[!UICONTROL Total]** 作为分析类型 **[!UICONTROL Select analysis type]**.

         如果您选择 ![时钟](../assets/icons/Clock.svg) **[!UICONTROL Time]**，您可以指定时间频率。 选择 **[!UICONTROL Daily]**， **[!UICONTROL Weekly]**， **[!UICONTROL Monthly]** 或 **[!UICONTROL Quarterly]** 从 **[!UICONTROL Select time frequency]**.

         您将在以下位置看到当前选择的更新预览： [!UICONTROL Preview Area] 以及您当前使用的构件 [!UICONTROL Current].

         ![编辑协调的数据构件](../assets/edit-harmonized-data-widget.png)

         如果由于数据不可用而无法呈现预览，您会看到 ![数据错误](../assets/icons/DataUnavailable.svg) [!UICONTROL Insights Not Available] - [!UICONTROL Harmonized fields are not available].

      1. 选择 **[!UICONTROL Apply]** 将更改应用到构件。 选择 **[!UICONTROL Cancel]** 以取消对当前构件所做的任何更改。

