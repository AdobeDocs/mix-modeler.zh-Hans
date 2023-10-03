---
title: 架构
description: 了解如何管理将数据摄取到Mix Modeler所需的架构。
feature: Schemas
exl-id: 08289581-5af9-4422-b049-8c24105e2a8e
source-git-commit: 33883626d8e7aca2eecc3571593be53ef41ac458
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 6%

---

# 架构

要管理架构，请支持要在Experience Platform摄取并在Mix Modeler中使用的数据：

1. 转到Mix Modeler界面。

1. 选择 ![架构](../assets/icons/Schemas.svg) **[!UICONTROL Schemas]**，下 **[!UICONTROL DATA MANAGEMENT]**.

请参阅 [架构UI概述](https://experienceleague.adobe.com/docs/experience-platform/xdm/ui/overview.html?lang=en) 以了解更多信息。

## 汇总或汇总数据

强烈建议使用XDM摘要量度类作为任何要摄取到Experience Platform并在Mix Modeler中使用的聚合或摘要数据的架构基础。

将XDM摘要量度类用于：

- 围墙花园数据，例如来自Facebook或YouTube的数据。

- 外部因素数据，如SPX（S&amp;P 500股价指数）、天气数据、

- 内部因素数据，例如价格变化、假日日历。

>[!IMPORTANT]
>
>架构定义必须至少包含一个数字字段（使用Integer、Double、Boolean或其他数字类型），才能支持摄取数据所需的量度。

使用 **[!DNL XDM Summary Metrics]** 基类可以很简单，如 **[!DNL ExternalFactorSummarySchema]** 下。

![外部因素架构](../assets/external-factors-schema.png)

此简单架构可用于摄取包含数据的数据集，例如：

- 竞争者索引数据

  | 时间戳 | date_type | 因子 | 值 |
  |---|---|---|--:|
  | 2020-11-28T00:00:00.000赫 | 周 | competier_index | 289.8 |
  | 2020-12-05T00:00:00.000赫 | 周 | competier_index | 291.2 |
  | 2020-12-12T00:00:00.000赫 | 周 | competier_index | 280.07 |
  | ... | ... | ... | ... |

- 公共假日数据

  | 时间戳 | date_type | 因子 | 值 |
  |---|---|---|--:|
  | 2020-11-28T00:00:00.000赫 | 周 | all_holidays_flag | 0.0 |
  | 2020-12-05T00:00:00.000赫 | 周 | all_holidays_flag | 0.0 |
  | 2020-12-12T00:00:00.000赫 | 周 | all_holidays_flag | 0.0 |
  | 2020-12-19T00:00:00.000赫 | 周 | all_holidays_flag | 0.0 |
  | 2020-12-26T00:00:00.000赫 | 周 | all_holidays_flag | 1.0 |
  | ... | ... | ... | ... |


有关更全面的示例，请参见下文 **[!DNL LumaPaidMarketingSchema]** 使用 **[!DNL XDM Summary Metrics]** 作为基类。 架构使用专用字段组（带颜色注释）进行量度(**[!DNL AMMMetrics]**)，尺寸(**[!DNL AMMDimensions]**)，以及其他特定于客户的信息(**[!DNL CustomerSpecific]**)。

![概要架构](../assets/summary-schema.png)

鉴于配置文件提取的异步性质，在从外部源收集聚合或摘要数据时，建议使用外部源系统审核详细信息字段组作为架构的一部分。 此字段组为外部源定义一组审核属性。
