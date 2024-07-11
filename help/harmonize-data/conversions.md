---
title: 转化
description: 了解如何创建转化，以便在Mix Modeler中协调数据时使用。
feature: Harmonized Data, Conversions
exl-id: a8559426-452a-43e8-9a60-0c0bc97d863c
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 1%

---

# 转化

转化事件是确定营销活动影响的业务目标。 示例：电子商务订单、店内购买、网站访问等。

您可以定义归因分析的营销转化。

## 管理转化

要在Mix Modeler界面中查看可用转化的表格，请执行以下操作：

1. 选择 ![数据搜索](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** 从左边栏开始。

1. 选择 **[!UICONTROL Conversions]** 从顶部栏中。 您会看到转化率表。

表列指定有关转换的详细信息：

| 列名称 | 详细信息 |
| --- | ---|
| 名称 | 转换的名称。 |
| 收入 | 用于计算转化收入的统一数据指标。 |
| 转化量度 | 用作分析转化指标的协调数据指标。 |
| 类别 | 转化的转化类别。 |
| 已创建 | 创建转化的日期和时间。 |
| 上次修改时间 | 上次修改转换的日期和时间。 |

{style="table-layout:auto"}

## 添加转化

要添加转化，请在 ![数据搜索](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Conversion]** 界面Mix Modeler：

1. 选择 ![添加](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add a conversion]**.

1. 在 **[!UICONTROL Create conversion]** 对话框：

   1. 输入名称 **[!UICONTROL Conversion]**&#x200B;例如 `Store Conversions`.

   1. 定义 **[!UICONTROL Conversion category]**.

      1. 从中选择值 **[!UICONTROL *选择协调……*]**例如 `Conversion types`.

      1. 选择运算符的值 ![V形](/help/assets//icons/ChevronDown.svg)例如 **[!UICONTROL is]**.

      1. 从中选择值 **[!UICONTROL *选择值&#x200B;*]**或输入值，例如&#x200B;**[!UICONTROL Store]**.

   1. 从中选择协调字段 **[!UICONTROL Conversion metric for analysis]**&#x200B;例如 **[!UICONTROL Orders]**.

   1. 从中选择协调字段 **[!UICONTROL Revenue field]**&#x200B;例如 **[!UICONTROL Gross Demand]**.

   1. 要创建转换，请选择 **[!UICONTROL Create]**. 要取消转换的创建，请选择 **[!UICONTROL Cancel]**.

      ![替换文本](/help/assets//create-conversion.png)

1. 创建后，转化会被添加到转化表中。


## 查看转化

要查看转换，请执行以下操作：

1. 选择 ![更多](/help/assets//icons/More.svg) 将鼠标悬停在表中的转化名称上时，出现此错误。

1. 选择 ![视图](/help/assets//icons/ViewDetail.svg) **视图**. 此时将显示一个对话框，其中显示了转换的详细信息。 请参阅 [添加转化](#add-a-conversion) 以了解更多信息。 选择 **[!UICONTROL Cancel]** 以关闭对话框。


## 删除转换

要删除转换，请执行以下操作：

1. 选择 ![删除](/help/assets//icons/Delete.svg) **删除** 将鼠标悬停在表中的转化名称上时，出现此错误。
1. 在 **[!UICONTROL Delete conversion]** 对话框确认对话框选择 **[!UICONTROL Delete]** 以永久删除转换。
