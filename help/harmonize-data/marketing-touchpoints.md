---
title: 营销接触点
description: 了解如何创建营销接触点，以将其用作Mix Modeler中协调数据的一部分。
feature: Harmonized Data, Marketing Touch Points
exl-id: 42851107-7568-4bc9-92ca-3cba713a522e
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# 营销接触点

营销接触点是收件人、个人和/或Cookie级别的营销事件，用于评估营销投资对数值或基于收入的转化的影响。

您可以定义营销接触点来帮助您进行归因分析。

## 管理营销接触点

要在Mix Modeler界面中查看可用的营销接触点表，请执行以下操作：

1. 选择 ![数据搜索](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** 从左边栏开始。

1. 选择 **[!UICONTROL Marketing touchpoint]** 从顶部栏中。 您会看到营销接触点表。 如果有更多页面可用，请使用 ![向左箭头](/help/assets//icons/ChevronLeft.svg) 或 ![向右箭头](/help/assets//icons/ChevronRight.svg) 在 **[!UICONTROL Page _x _之_x_]** 在表的页面之间移动。

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

要添加营销接触点，请在 ![数据搜索](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Marketing touchpoint]** 界面Mix Modeler：

1. 选择 ![添加](/help/assets//icons/AddCircle.svg) 添加营销接触点。

1. 在 **[!UICONTROL Marketing touchpoint]** 对话框。

   1. 输入名称 **[!UICONTROL Touchpoint Name]**&#x200B;例如 `Luma Touchpoint`.

   1. 定义 **[!UICONTROL Touchpoint rule]**.

      1. 从中选择值 **[!UICONTROL *选择已协调&#x200B;*]**例如&#x200B;**[!UICONTROL Brand]**.

      1. 选择运算符的值 ![V形](/help/assets//icons/ChevronDown.svg)例如 **[!UICONTROL is]**.

      1. 从中选择值 **[!UICONTROL *选择值&#x200B;*]**或输入值，例如&#x200B;**[!DNL Luma]**.

   1. 从中选择协调字段 **[!UICONTROL Touchpoint volume]**&#x200B;例如 **[!UICONTROL Impressions]**.

   1. 从中选择协调字段 **[!UICONTROL Touchpoint spend]**&#x200B;例如 **[!UICONTROL Cost]**.

      ![营销接触点](/help/assets//create-touchpoint.png)

   1. 要创建营销接触点，请选择 **[!UICONTROL Create]**. 要取消创建营销接触点，请选择 **[!UICONTROL Cancel]** .

1. 创建后，接触点将添加到营销接触点表中。


## 查看营销接触点

要查看营销接触点，请执行以下操作：

1. 选择 ![更多](/help/assets//icons/More.svg) 将鼠标悬停在表格中的营销接触点名称上时，会出现这种情况。

1. 选择 ![视图](/help/assets//icons/ViewDetail.svg) **视图**. 此时一个对话框会显示营销接触点的详细信息。 请参阅 [添加营销接触点](#add-a-marketing-touchpoint) 以了解更多信息。 选择 **[!UICONTROL Cancel]** 以关闭对话框。


## 删除营销接触点

要删除营销接触点，请执行以下操作：

1. 选择 ![删除](/help/assets//icons/Delete.svg) **删除** 将鼠标悬停在表格中的营销接触点名称上时，会出现这种情况。
1. 在 **[!UICONTROL Delete touchpoint]** 对话框确认对话框选择 **[!UICONTROL Delete]** 以永久删除营销接触点。

