---
title: 计划概述
description: 了解如何在Mix Modeler中查看、选择和操作计划。
feature: Plans
exl-id: 45a8dc30-3259-493d-8ea5-1899903733a6
source-git-commit: 0d11168b71319e6c854482f89dbb1bb68962a880
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# 计划概述

Mix Modeler中的计划允许您按业务部门和渠道分配预算。 计划功能与根据您的统一数据经过培训的模型的结果相集成。

计划概述一家企业计划在给定时间范围内在营销相关项目上可自由支配的投资（例如预算）。 这些投资服务于常见的KPI（例如订单、收入）。 计划可包括来自付费广告、赞助网络内容和活动等渠道的费用。

计划要求：

- 模型，
- 一个数据范围，
- 预算。

计划可以选择包括：

- 设定的识别窗口，
- 多个航班日期，每个航班都有目标预算，
- 按渠道和投放日期列出的最小和最大预算限制。

如果您用于计划的模型依据新数据进行了评分，则需要创建新计划以考虑重新评分的数据。


## 构建计划

要构建计划，请使用Mix Modeler计划创建向导。 有关更多详细信息，请参阅[生成计划](build.md)。


## 管理计划

要查看当前计划的表格，请在Mix Modeler界面中执行以下操作：

1. 从左边栏中选择![](/help/assets/icons2/FileChart.svg) **[!UICONTROL Plans]**。

1. 您会看到当前计划及其状态的表。

   表列指定有关计划的详细信息。

   | 列名称 | 详细信息 |
   |---|---|
   | 名称 | 计划的名称 |
   | 模型 | 用作计划基础的模型。 |
   | Date range | 计划的完整日期范围。 |
   | 预算 | 计划的总预算。 |
   | 计划目标 | 为基于目标的计划定义的目标量度。 |
   | 预测退货 | 计划的[预测返回](/help/main-guide/glossary.md) |
   | 预测的ROI | 计划的[预测ROI](/help/main-guide/glossary.md)。 |
   | 预测的转化 | 计划的[预测转化](/help/main-guide/glossary.md) |
   | 预测的CPA | 计划的[预测CPA](/help/main-guide/glossary.md) |
   | 状态 | 计划的状态： <p><span style="color:red">●</span>失败， <p><span style="color:blue">●</span>正在处理，或 <p><span style="color:green">●</span>完成。 |

   {style="table-layout:auto"}

   您可以使用![ColumnSetting](/help/assets/icons/ColumnSetting.svg)来选择要显示在表格中的![复选标记](/help/assets/icons/Checkmark.svg)列。

   要按升序![ArrowMoveUp](/help/assets/icons2/ArrowMoveUp.svg)或降序![ArrowMoveDown](/help/assets/icons2/ArrowMoveDown.svg)顺序对任意列的表进行排序，请选择列的标题。

   要对&#x200B;**[!UICONTROL Name]**、**[!UICONTROL Model]**&#x200B;或&#x200B;**[!UICONTROL Date range]**&#x200B;列进行排序或调整其大小，请选择&#x200B;**[!UICONTROL Name]** ![V形](/help/assets/icons/ChevronDown.svg)、**[!UICONTROL Model]** ![V形](/help/assets/icons/ChevronDown.svg)或&#x200B;**[!UICONTROL Date range]** ![V形](/help/assets/icons/ChevronDown.svg)。 从上下文菜单中选择&#x200B;**[!UICONTROL Sort ascending]**、**[!UICONTROL Sort descending]**&#x200B;或&#x200B;**[!UICONTROL Resize column]**。 或者，可以将鼠标悬停在这些列的列分隔符上以调整列的大小。

1. 使用![搜索](/help/assets/icons/Search.svg)在表中搜索并筛选一个或多个特定计划。

### 计划洞察

要查看计划的分析并编辑计划，请执行以下操作：

1. 从左边栏中选择![PLan](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]**。

1. 选择计划名称。

您被重定向到[计划分析](insights.md)。


### 复制计划

要复制计划，请执行以下操作：

- 为计划选择![更多](/help/assets/icons/More.svg)。 从上下文菜单中选择&#x200B;**[!UICONTROL Duplicate]**。
- 或者，在表![SelectBox](/help/assets/icons/SelectBox.svg)中选择一个计划，然后从蓝色操作栏中选择![复制](/help/assets/icons/Copy.svg) **[!UICONTROL Duplicate]**。

已创建一个新计划，其名称由原始计划的名称附加上&#x200B;**[!UICONTROL (Copy)] (_n_)**&#x200B;组成。 系统会自动将您重定向到[计划创建](build.md)，以便为复制的计划提供更新的详细信息。

- 原始计划中的详细信息（如描述、预算等）将复制过来。
- 原始计划中的预算约束将复制到新创建的计划中。
- 您可以选择另一个模型作为复制计划的基础。
   - 对于已复制计划中存在，但在新选择的模型中不存在的接触点或渠道，将从计划中移除这些接触点或渠道的任何约束。
   - 对于复制计划中不存在但在新选择的模型中存在的接触点或渠道，约束将设置为：
      - 最小值为`0`，
      - 与计划外部测试版范围预算一致的最大值。



### 比较计划

要比较计划，请执行以下操作：

1. 从表中选择两个计划。
1. 从蓝色操作栏中选择![比较](/help/assets/icons/Compare.svg) **[!UICONTROL Compare]**。 您看到&#x200B;**[!UICONTROL Compare plans]** UI。


### 删除计划

要删除计划，请执行以下操作：

1. 为计划选择![更多](/help/assets/icons/More.svg)。 从上下文菜单中选择&#x200B;**[!UICONTROL Delete]**。 <br/>或者，在表![SelectBox](/help/assets/icons/SelectBox.svg)中选择计划，然后从蓝色操作栏中选择![删除](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**。
1. 在&#x200B;**[!UICONTROL Delete]**&#x200B;确认对话框中选择&#x200B;**[!UICONTROL Delete plan]**&#x200B;以删除计划。 选择要取消的&#x200B;**[!UICONTROL Cancel]**。

要删除多个计划，请执行以下操作：

1. 选择多个计划。
1. 从蓝色操作栏中，选择![删除](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;以删除计划。
1. 在&#x200B;**[!UICONTROL Delete]** x **[!UICONTROL Delete *计划&#x200B;*确认对话框中选择]**&#x200B;以删除计划。 选择要取消的&#x200B;**[!UICONTROL Cancel]**。


