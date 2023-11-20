---
title: 模型
description: 了解如何在Mix Modeler中配置和使用模型。
feature: Models
exl-id: c43d9bc9-4429-45c2-9247-bd24510a24be
source-git-commit: 73534d1aecb6d1513f6f3b5f1801b497ad73278f
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 0%

---

# 模型

Mix Modeler中的模型功能允许您配置、训练特定于您的业务目标并受AI驱动的多触点归因和营销组合建模之间的传输学习支持的AI/ML模型，并对其评分。

这些模型基于您在Mix Modeler应用工作流程中创建的统一数据。

Mix Modeler模型是一种机器学习模型，用于根据营销人员的投资来测量和/或预测指定的结果。 营销接触点和摘要级别的数据可用作输入。 Mix Modeler允许您根据不同的变量集、维度和结果（如收入、销量、商机）创建模型的变体。

模型需要：

* 一次转换，
* 一个或多个营销接触点（渠道），包括摘要级别的数据、营销接触点数据（事件数据）或两者，
* 可配置的回看窗口用于
* 可配置的培训窗口。

模型可以选择包括：

* 外部因素，
* 内部因素，
* 所谓的“先验分布”（概率分布表示数据在先或在观测该数据之前所具有的知识或不确定性），其按渠道对先前转化进行索引，
* 支出份额，在营销数据稀疏时使用相对支出份额作为代理。


## 创建模型

要创建模型，请使用选择时提供的Mix Modeler逐步引导模型配置流程 **[!UICONTROL Guide me]**. 请参阅 [创建模型](create.md) 以了解更多详细信息。

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
   | 运行频率 | 训练模型的运行频率。 |
   | 上次运行 | 模型上次训练的日期和时间。 |
   | 状态 | 模型上次运行的状态。 <br/><span style="color:green">●</span> 成功<br/><span style="color:orange">●</span> 培训问题<br/> <span style="color:orange">●</span> 正在等待训练 <br/><span style="color:red">●</span> 失败 |

   {style="table-layout:auto"}

1. 要更改为列表显示的列，请选择 ![列设置](../assets/icons/ColumnSetting.svg) 并打开列 ![Check](../assets/icons/Checkmark.svg) 或关闭。

### 删除模型

要删除模型，请执行以下操作：

1. 选择要删除的模型的名称。

1. 从上下文菜单中，选择 **[!UICONTROL Delete]** 以删除模型。

### 查看模型的详细信息

要查看模型的更多详细信息，请执行以下操作：

1. 选择 ![信息](../assets/icons/Info.svg) ，以便模型显示包含详细信息的弹出窗口。



### 模型洞察

>[!NOTE]
>
>此选择仅适用于已成功训练的模型。
>

要查看模型的分析，请在Mix Modeler界面中：

1. 选择 ![](../assets/icons/FileData.svg) **[!UICONTROL Models]** 从左边栏开始。

1. 选择模型名称 **[!UICONTROL Last run status]** 之 <span style="color:green">●</span> **[!UICONTROL Success]** 从 **[!UICONTROL Models]** 表格。

1. 从上下文菜单中，选择 **[!UICONTROL Model Insights]**. 您将被重定向到 [模型分析](insights.md).


### 重新得分

>[!NOTE]
>
>此选择仅适用于已成功训练的模型。
>

要重新对模型计分，请在Mix Modeler界面中：

1. 选择 ![](../assets/icons/FileData.svg) **[!UICONTROL Models]** 从左边栏开始。

1. 选择模型名称 **[!UICONTROL Last run status]** 之 <span style="color:green">●</span> **[!UICONTROL Success]** 从 **[!UICONTROL Models]** 表格。

1. 从上下文菜单中，选择 **[!UICONTROL Re-score]**. 显示模型的更新状态可能需要几分钟的时间。

