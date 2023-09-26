---
title: 转化
description: 了解如何在Adobe组合建模器中创建要用作协调数据一部分的转化。
feature: Harmonized Data, Conversions
source-git-commit: ac17f5a9fcf036c8e689879578e4b745b789cea3
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 3%

---


# 转化

转化事件是确定营销活动影响的业务目标。 示例：电子商务订单、店内购买、网站访问等。

您可以定义归因分析的营销转化。

## 管理转化

要查看可用转化表，请在Adobe组合建模器界面中：

1. 选择 ![数据搜索](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** 从左边栏开始。

1. 选择 **[!UICONTROL Conversions]** 从顶部栏中。 您会看到转化率表。

表列指定有关转换的详细信息：

| 列名称 | 详细信息 |
| --- | ---|
| 名称 | 转换的名称。 |
| 收入 | 用于计算转化收入的统一数据指标。 |
| 转化量度 | 用作分析转化指标的协调数据指标。 |
| 已创建 | 创建转化的日期和时间。 |
| 上次修改时间 | 上次修改转换的日期和时间。 |

{style="table-layout:auto"}

## 添加转化

要添加转化，请在 ![数据搜索](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Conversion]** Adobe组合建模器中的接口：

1. 选择 ![添加](../assets/icons/AddCircle.svg) **[!UICONTROL Add a conversion]**.

1. 在 **[!UICONTROL Create Conversion]** 对话框：

   1. 输入名称 **[!UICONTROL Conversion]**&#x200B;例如 `Store Conversions`.

   1. 定义 **[!UICONTROL Conversion category]**.

      1. 从中选择值 **[!UICONTROL *选择协调……*]**例如 `Conversion Type`.

      1. 选择运算符的值 ![V形](../assets/icons/ChevronDown.svg)例如 **[!UICONTROL is]**.

      1. 从中选择值 **[!UICONTROL *选择值&#x200B;*]**或输入值，例如&#x200B;**[!UICONTROL Store]**.

   1. 从中选择协调字段 **[!UICONTROL Conversion metric for analysis]**&#x200B;例如 **[!UICONTROL Orders]**.

   1. 从中选择协调字段 **[!UICONTROL Revenue field]**&#x200B;例如 **[!UICONTROL Gross Demand]**.

   1. 要创建转换，请选择 **[!UICONTROL Create]**. 要取消转换的创建，请选择 **[!UICONTROL Cancel]**.

      ![替换文字](../assets/create-conversion.png)

1. 创建后，转化会被添加到转化表中。
