---
title: 营销接触点
description: 了解如何在Adobe组合建模器中创建营销接触点，以将其用作协调数据的一部分。
feature: Harmonized Data, Marketing Touch Points
source-git-commit: ac17f5a9fcf036c8e689879578e4b745b789cea3
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 1%

---


# 营销接触点

营销接触点是收件人、个人和/或Cookie级别的营销事件，用于评估营销投资对数值或基于收入的转化的影响。

您可以定义营销接触点来帮助您进行归因分析。

## 管理营销接触点

要在Adobe组合建模器界面中查看可用的营销接触点表，请执行以下操作：

1. 选择 ![数据搜索](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** 从左边栏开始。

1. 选择 **[!UICONTROL Marketing touchpoint]** 从顶部栏中。 您会看到营销接触点表。

表列指定有关营销接触点的详细信息：

| 列名称 | 详细信息 |
| --- | ---|
| 名称 | 营销接触点的名称。 |
| 支出量度 | 用于计算接触点支出的协调数据指标。 |
| 数量指标 | 用于计算接触点数量的协调数据指标。 |
| 已创建 | 创建营销接触点的日期和时间。 |
| 上次修改时间 | 上次修改营销接触点的日期和时间。 |

{style="table-layout:auto"}

## 添加营销接触点

要添加营销接触点，请在 ![数据搜索](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Marketing touchpoint]** Adobe组合建模器中的接口：

1. 选择 ![添加](../assets/icons/AddCircle.svg) 添加营销接触点。

1. 在 **[!UICONTROL Marketing touchpoint]** 对话框。

   1. 输入名称 **[!UICONTROL Touchpoint Name]**&#x200B;例如 `Luma Touchpoint`.

   1. 定义 **[!UICONTROL Touchpoint rule]**.

      1. 从中选择值 **[!UICONTROL *选择协调……*]**例如&#x200B;**[!UICONTROL Brand]**.

      1. 选择运算符的值 ![V形](../assets/icons/ChevronDown.svg)例如 **[!UICONTROL is]**.

      1. 从中选择值 **[!UICONTROL *选择值&#x200B;*]**或输入值，例如&#x200B;**[!DNL Luma]**.

   1. 从中选择协调字段 **[!UICONTROL Touchpoint volume]**&#x200B;例如 **[!UICONTROL Impressions]**.

   1. 从中选择协调字段 **[!UICONTROL Touchpoint spend]**&#x200B;例如 **[!UICONTROL Cost]**.

      ![营销接触点](../assets/create-touchpoint.png)

   1. 要创建营销接触点，请选择 **[!UICONTROL Create]**. 要取消创建营销接触点，请选择 **[!UICONTROL Cancel]** .

1. 创建后，接触点将添加到营销接触点表中。

