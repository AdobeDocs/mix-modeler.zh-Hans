---
title: 模型
description: 了解如何在Mix Modeler中配置和使用模型。
feature: Models
source-git-commit: 08cfd4239f6bcaf885565f3ae04cbd51869e8c00
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# 模型

Mix Modeler中的模型功能允许您配置、训练特定于您的业务目标并受AI驱动的多触点归因和营销组合建模之间的传输学习支持的AI/ML模型，并对其评分。

这些模型基于您在Mix Modeler应用工作流程中创建的统一数据。

要创建模型，请使用“混合建模器”步骤引导式模型配置流程，此流程可在选择时提供 **[!UICONTROL Guide me]**. 请参阅 [创建模型](create.md) 以了解更多详细信息。

## 管理模型

要查看当前模型的表，请在Mix Modeler界面中：

1. 选择 ![](../assets/icons/FileData.svg) **[!UICONTROL Models]** 从左边栏开始。

1. 您会看到当前模型的表。

   表列指定有关模型的详细信息。

   | 列名称 | 详细信息 |
   |---|---|
   | 名称 | 模型的名称 |
   | 描述 | 模型的描述 |
   | 转化事件 | 您为模型选择的转换。 |
   | 数据集 | 模型用于训练和评分的数据集。 默认情况下，这是协调的数据集。 |
   | 运行频率 | 训练模型的运行频率。 |
   | 上次运行 | 模型上次训练的日期和时间。 |
   | 上次运行状态 | 模型上次运行的状态。 <br/><span style="color:green">●</span> 成功<br/><span style="color:orange">●</span> 培训问题<br/> <span style="color:orange">●</span> 正在等待训练 <br/><span style="color:red">●</span> 失败 |

   {style="table-layout:auto"}

1. 要更改为列表显示的列，请选择 ![列设置](../assets/icons/ColumnSetting.svg) 并打开列 ![Check](../assets/icons/Checkmark.svg) 或关闭。

### 删除模型

要删除模型，请执行以下操作：

1. 选择要删除的模型的名称。

1. 从上下文菜单中，选择 **[!UICONTROL Delete]** 以删除模型。

### 查看模型的详细信息

要查看模型的更多详细信息，请执行以下操作：

1. 选择要查看其更多详细信息的模型名称。

1. 从上下文菜单中，选择 **[!UICONTROL More]**. 您会在右窗格中看到所选模型的详细信息。



### 模型洞察

>[!NOTE]
>
>此选择仅适用于训练成功的模型。
>

要查看模型的分析，请在Mix Modeler界面中：

1. 选择 ![](../assets/icons/FileData.svg) **[!UICONTROL Models]** 从左边栏开始。

1. 选择模型名称 **[!UICONTROL Last run status]** 之 <span style="color:green">●</span> **[!UICONTROL Success]** 从 **[!UICONTROL Models]** 表格。

1. 从上下文菜单中，选择 **[!UICONTROL Model Insights]**. 您将被重定向到 [模型分析](insights.md).


