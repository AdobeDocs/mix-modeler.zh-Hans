---
title: 架构
description: 了解如何管理将数据摄取到Adobe组合建模器所需的架构。
feature: Datasets
source-git-commit: abbfc78e9fa774a240d000131f35d3dc257c15ea
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 1%

---


# 架构

要管理架构，请支持您要在Adobe Experience Platform中摄取并在Adobe组合建模器中使用的数据：

1. 转到Adobe混合建模器界面。

1. 选择 ![架构](../assets/icons/Schemas.svg) **[!UICONTROL Schemas]**，下 **[!UICONTROL DATA MANAGEMENT]**.

请参阅 [架构UI概述](https://experienceleague.adobe.com/docs/experience-platform/xdm/ui/overview.html?lang=en) 以了解更多信息。

## 汇总或汇总数据

强烈建议使用XDM摘要量度类作为架构的基础，该架构支持您要在Experience Platform中摄取并在Adobe组合建模器中使用的任何聚合或摘要数据。

有关示例，请参见下文 **[!DNL LumaPaidMarketingSchema]** 将XDM摘要量度用作量度的基类和专用字段组（带颜色注释）(**[!DNL AMMMetrics]**)，尺寸(**[!DNL AMMDimensions]**)和其他特定于客户的信息(**[!DNL CustomerSpecific]**)。

![概要架构](../assets/summary-schema.png)

要定义一组审计属性，强烈建议使用外部源系统审计详细信息字段组，作为用于从外部源收集聚合或摘要数据的架构的一部分。
