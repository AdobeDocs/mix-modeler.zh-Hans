---
title: 转化
description: 了解如何创建转化，以便在Mix Modeler中协调数据时使用。
feature: Harmonized Data, Conversions
exl-id: a8559426-452a-43e8-9a60-0c0bc97d863c
source-git-commit: 935b179e31d1b677a8c83b1566c02b7aaa617e8d
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 1%

---

# 转化

转化事件是确定营销活动影响的业务目标。 示例：电子商务订单、店内购买、网站访问等。

您可以定义归因分析的营销转化。

## 管理转化

要在Mix Modeler界面中查看可用转化的表格，请执行以下操作：

1. 从左边栏中选择![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]**。

1. 从顶部栏中选择&#x200B;**[!UICONTROL Conversions]**。 您会看到转化率表。

表列指定有关转换的详细信息：

| 列名称 | 详细信息 |
| --- | ---|
| 名称 | 转换的名称。 |
| 收入 | 用于计算转化收入的统一数据指标。 |
| 转化量度 | 用作分析转化指标的协调数据指标。 |
| 类别 | 转化的转化类别。 |
| 已创建 | 创建转化的日期和时间。 |
| 上次修改时间 | 上次修改转换的日期和时间。 |


## 添加转化

要添加转换，请在Mix Modeler的![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Conversion]**&#x200B;界面中：

1. 选择![添加](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a conversion]**。

1. 在&#x200B;**[!UICONTROL Create conversion]**&#x200B;对话框中：

   1. 输入&#x200B;**[!UICONTROL Conversion]**&#x200B;的名称，例如`Store Conversions`。

   1. 定义&#x200B;**[!UICONTROL Conversion category]**。

      1. 从&#x200B;**[!UICONTROL *选择协调……*]**&#x200B;中选择一个值，例如`Conversion types`。

      1. 选择运算符![V形](/help/assets/icons/ChevronDown.svg)的值，例如&#x200B;**[!UICONTROL is]**。

      1. 从&#x200B;**[!UICONTROL *中选择值&#x200B;*]**&#x200B;或输入值，例如&#x200B;**[!UICONTROL Store]**。

   1. 从&#x200B;**[!UICONTROL Conversion metric for analysis]**&#x200B;中选择协调字段，例如&#x200B;**[!UICONTROL Orders]**。

   1. 从&#x200B;**[!UICONTROL Revenue field]**&#x200B;中选择协调字段，例如&#x200B;**[!UICONTROL Gross Demand]**。

   1. 要创建转换，请选择&#x200B;**[!UICONTROL Create]**。 要取消转换的创建，请选择&#x200B;**[!UICONTROL Cancel]**。

      ![替换文本](/help/assets/create-conversion.png)

1. 创建后，转化会被添加到转化表中。


## 查看详细信息

要查看转换的详细信息，请执行以下操作：

1. 将鼠标悬停在表中的转化名称上时，选择![更多](/help/assets/icons/More.svg)。

1. 选择![查看](/help/assets/icons/ViewDetail.svg) **查看详细信息**。 此时将显示一个对话框，其中显示了转换的详细信息。 有关详细信息，请参阅[添加转换](#add-a-conversion)。 选择&#x200B;**[!UICONTROL Cancel]**&#x200B;关闭对话框。

## 查看报告

要查看转化报表，请执行以下操作：

1. 将鼠标悬停在表中的转化名称上时，选择![更多](/help/assets/icons/More.svg)。

1. 选择![GraphTrend](/help/assets/icons/GraphTrend.svg) **查看报告**。 此时将显示一个对话框，其中显示了转换的报告。

   ![转化视图报告](../assets/conversion-view-report.png)

   * 要更改报告的粒度，请从&#x200B;**[!UICONTROL Weekly]**&#x200B;下拉菜单中选择一个值。
   * 若要更改要报告的期间，请输入开始和结束日期，或使用![日历](/help/assets/icons/Calendar.svg)在日历弹出窗口中定义期间。

1. 选择&#x200B;**[!UICONTROL Close]**&#x200B;关闭对话框。

## 删除转换

要删除转换，请执行以下操作：

1. 将鼠标悬停在表中的转换名称上时，选择![删除](/help/assets/icons/Delete.svg) **删除**。
1. 在&#x200B;**[!UICONTROL Delete conversion]**&#x200B;对话框确认对话框中，选择&#x200B;**[!UICONTROL Delete]**&#x200B;以永久删除转换。
