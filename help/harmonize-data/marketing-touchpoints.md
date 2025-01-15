---
title: 营销接触点
description: 了解如何创建营销接触点，以将其用作Mix Modeler中协调数据的一部分。
feature: Harmonized Data, Marketing Touch Points
exl-id: 42851107-7568-4bc9-92ca-3cba713a522e
source-git-commit: 665b344dfa94275d71e0ecf198d9bb9b73ea584b
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# 营销接触点

营销接触点是收件人、个人和/或Cookie级别的营销事件，用于评估营销投资对数值或基于收入的转化的影响。

您可以定义营销接触点来帮助您进行归因分析。

## 管理营销接触点

要在Mix Modeler界面中查看可用的营销接触点表，请执行以下操作：

1. 从左边栏中选择![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]**。

1. 从顶部栏中选择&#x200B;**[!UICONTROL Marketing touchpoint]**。 您会看到营销接触点表。 如果有更多页面可用，请使用&#x200B;_x _]**的**[!UICONTROL Page _x_&#x200B;上的![向左箭头](/help/assets/icons/ChevronLeft.svg)或![向右箭头](/help/assets/icons/ChevronRight.svg)在表的页面之间移动。

表列指定有关营销接触点的详细信息：

| 列名称 | 详细信息 |
| --- | ---|
| 名称 | 营销接触点的名称。 |
| 支出量度 | 用于计算接触点支出的协调数据指标。 |
| 数量指标 | 用于计算接触点数量的协调数据指标。 |
| 规则 | 要使用的接触点规则。 |
| 已创建 | 创建营销接触点的日期和时间。 |
| 上次修改时间 | 上次修改营销接触点的日期和时间。 |

{style="table-layout:auto"}

## 添加营销接触点

要添加营销接触点，请在Mix Modeler的![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Marketing touchpoint]**&#x200B;界面中：

1. 选择![添加](/help/assets/icons/AddCircle.svg)添加营销接触点。

1. 在&#x200B;**[!UICONTROL Marketing touchpoint]**&#x200B;对话框中。

   1. 输入&#x200B;**[!UICONTROL Touchpoint Name]**&#x200B;的名称，例如`Luma Touchpoint`。

   1. 定义&#x200B;**[!UICONTROL Touchpoint rule]**。

      1. 从&#x200B;**[!UICONTROL *选择协调的&#x200B;*]**中选择一个值，例如&#x200B;**[!UICONTROL Brand]**。

      1. 为运算符![V形](/help/assets/icons/ChevronDown.svg)选择一个值，例如&#x200B;**[!UICONTROL is]**。

      1. 从&#x200B;**[!UICONTROL *中选择值&#x200B;*]**或输入值，例如&#x200B;**[!DNL Luma]**。

   1. 从&#x200B;**[!UICONTROL Touchpoint volume]**&#x200B;中选择协调字段，例如&#x200B;**[!UICONTROL Impressions]**。

   1. 从&#x200B;**[!UICONTROL Touchpoint spend]**&#x200B;中选择协调字段，例如&#x200B;**[!UICONTROL Cost]**。

      ![营销接触点](/help/assets/create-touchpoint.png)

   1. 要创建营销接触点，请选择&#x200B;**[!UICONTROL Create]**。 要取消创建营销接触点，请选择&#x200B;**[!UICONTROL Cancel]** 。

1. 创建后，接触点将添加到营销接触点表中。


## 查看详细信息

要查看营销接触点的详细信息，请执行以下操作：

1. 将鼠标悬停在表中的营销接触点名称上时，选择![更多](/help/assets/icons/More.svg)。

1. 选择![视图](/help/assets/icons/ViewDetail.svg) **视图**。 此时一个对话框会显示营销接触点的详细信息。 有关详细信息，请参阅[添加营销接触点](#add-a-marketing-touchpoint)。 选择&#x200B;**[!UICONTROL Cancel]**&#x200B;关闭对话框。


## 查看报告

要查看营销接触点报表，请执行以下操作：

1. 将鼠标悬停在表中的营销接触点名称上时，选择![更多](/help/assets/icons/More.svg)。

1. 选择![GraphTrend](/help/assets/icons/GraphTrend.svg) **查看报告**。 对话框会显示营销接触点的报告。

   ![营销接触点视图报告](../assets/marketingtouchpoint-view-report.png)

   * 要更改报告的粒度，请从&#x200B;**[!UICONTROL Weekly]**&#x200B;下拉菜单中选择一个值。
   * 若要更改要报告的期间，请输入开始和结束日期，或使用![日历](/help/assets/icons/Calendar.svg)在日历弹出窗口中定义期间。

1. 选择&#x200B;**[!UICONTROL Close]**&#x200B;关闭对话框。

## 删除营销接触点

要删除营销接触点，请执行以下操作：

1. 将鼠标悬停在表中的营销接触点名称上时，选择![删除](/help/assets/icons/Delete.svg) **删除**。
1. 在&#x200B;**[!UICONTROL Delete touchpoint]**&#x200B;对话框确认对话框中，选择&#x200B;**[!UICONTROL Delete]**&#x200B;以永久删除营销接触点。

