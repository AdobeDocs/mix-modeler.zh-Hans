---
title: 计划洞察
description: 了解如何在Mix Modeler中查看计划的见解并编辑计划。
feature: Plans
exl-id: 91385595-284f-4fcb-b54b-9539905e552b
source-git-commit: 86b58717c3c8be183c70d1ceccf6f7c757303518
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 0%

---

# 计划洞察


在[!UICONTROL Plan insights]中创建您的计划分析，显示计划所基于的[!UICONTROL Model]、[!UICONTROL Data range]和[!UICONTROL Plan target]。


创建分析后，您将看到计划的概览，包括：

- 显示计划所基于的[!UICONTROL Model]、[!UICONTROL Data range]和[!UICONTROL Plan target]的标头。
   - 如果定义了基于目标的计划，则标记会指示目标的状态。可能的选项包括：

      - [!BADGE 目标可实现]{type=Positive}
      - [!BADGE 目标无法实现]{type=Negative}

   - 选择![ChevronDown](/help/assets/icons/ChevronDown.svg) **[!UICONTROL Show more]**&#x200B;以显示更多详细信息。

- [[!UICONTROL Forecasted paid channel ROI]可视化图表](#forecasted-paid-channel-spend-and-roi)
- [[!UICONTROL Forecasted revenue]可视化图表](#forecasted-revenue)
- [[!UICONTROL Forecasted conversion]可视化图表](#forecasted-conversions)
- [[!UICONTROL Marginal channel return]可视化图表](#marginal-channel-return)
- 计划[[!UICONTROL Data range breakdown]的](#date-range-breakdown)表，显示列

   - 渠道
   - ROI
   - CPA
   - 收入
   - 转化目标
   - 支出

要关闭该界面，请选择&#x200B;**[!UICONTROL Close]**。

若要更改查看计划ROI的方式，请在&#x200B;**[!UICONTROL X]**&#x200B;中选择&#x200B;**[!UICONTROL  %]**&#x200B;或&#x200B;**[!UICONTROL View ROI]**。

## 预测的付费渠道支出和ROI

此可视化图表根据模型、日期范围和预算，显示付费渠道上预测支出和投资回报的散点图。

![预测的付费渠道支出和ROI可视化图表](../assets/overview-plan-forecasted-paid-channel-send-roi.png)


## 预测收入

此条形图可视化图表根据模型、日期范围和预算显示渠道的预测收入。

![预测收入可视化图表](../assets/overview-plan-forecasted-revenue.png)


## 预测的转化

此条形图可视化图表根据模型、日期范围和预算显示渠道的预测转化。

![预测转化可视化图表](../assets/overview-plan-forecasted-conversions.png)


## 边际渠道回报

此折线图可视化图表显示所选渠道的边际返回曲线，其中包含&#x200B;**[!UICONTROL Marginal break-even]**&#x200B;和&#x200B;**[!UICONTROL Return point]**&#x200B;的指标。 此可视化图表可帮助您了解渠道支出如何达到边际盈亏平衡点。 您是否有空间增加渠道支出，还是应该减少渠道支出，以提高渠道支出效率。

![边际渠道回报可视化](../assets/overview-plan-marginal-channel-return.png)

要为可视化图表选择特定渠道，请从&#x200B;**[!UICONTROL View]**&#x200B;下拉菜单中选择一个渠道。

## 渠道协同效应

渠道协同增效矩阵可帮助您识别营销渠道如何相互作用，从而在各自贡献之外产生乘数效应。

![计划渠道协同效应](/help/assets/plan-channel-synergies.png)

要下载表示矩阵的CSV文件，请选择![下载](/help/assets/icons/Download.svg) **[!UICONTROL Download]**。

## 日期范围细分

[!UICONTROL Date range breakdown]表显示[!UICONTROL ROI]、[!UICONTROL Revenue]、[!UICONTROL CPA]、[!UICONTROL Conversions]和[!UICONTROL Spend]的每通道详细的粒度数据。

![日期范围划分表](../assets/overview-plan-date-range-breakdown.png)

1. 要下载包含日期范围划分数据的CSV文件，请选择![下载](/help/assets/icons/Download.svg) **[!UICONTROL Download CSV]**。 从上下文菜单中：

   - 为CSV格式的详细数据选择![下载](/help/assets/icons/Download.svg) **[!UICONTROL Detailed CSV]**。
   - 为CSV格式的摘要数据选择![下载](/help/assets/icons/Download.svg) **[!UICONTROL Summary CSV]**。

   详细数据是按周划分键的细粒度数据。 摘要数据由模型提供的日期范围作为数据键。

1. 要查看按渠道类别划分的日期范围细分，请从&#x200B;**[!UICONTROL All channels]**&#x200B;选项中选择&#x200B;**[!UICONTROL Paid channels]**、**[!UICONTROL Non-paid channels]**&#x200B;或&#x200B;**[!UICONTROL View]**。


## 编辑计划

要编辑计划，请选择![编辑](/help/assets/icons/Edit.svg) **[!UICONTROL Edit plan]**。

1. 在&#x200B;**[!UICONTROL Spend selection]**&#x200B;部分中，对于每个预算日期范围，使用![V形](/help/assets/icons/ChevronRight.svg)打开该数据范围的渠道分配视图。

   如果您想要使用过去的营销支出数据和见解，则可以使用历史引用数据。 将历史引用数据考虑在内：

   - 通过突出显示高性能渠道和性能不佳的渠道来改进预算分配。
   - 支持趋势分析。
   - 在配置计划时，确定有效策略并避免错误。

   如果选择历史参考期，则需调整以前的支出模式首选项，Mix Modeler的计划功能可生成符合您期望的计划。 这些计划最终应增强利益相关者的信心，确保营销计划是战略性的、高效的，并且这些计划以经验证的绩效数据和业务需求为基础。

   ![花费选择](/help/assets/plan-spend-selection.png)

   1. 选择 **[!UICONTROL Spend pattern]**。

      - 默认选项为&#x200B;**[!UICONTROL Automatic]**。
      - 选择&#x200B;**[!UICONTROL Historical reference]**&#x200B;并输入&#x200B;**[!UICONTROL Start date]**&#x200B;以引用Mix Modeler已可用的以往营销支出数据。 **[!UICONTROL End date]**&#x200B;是根据所选的数据范围自动确定的。 建议的开始日期是第一个可用的过去营销支出数据。 为了表示您选择了不存在的历史参考期，您会看到![AlertRed](/help/assets/icons/AlertRed.svg)。


   1. 要修改每个渠道的预算，请修改&#x200B;**[!UICONTROL Min]**&#x200B;和&#x200B;**[!UICONTROL Max]**&#x200B;的值或使用滑块。

   1. 要在货币或百分比输入之间切换，请为&#x200B;**[!UICONTROL $]**&#x200B;选择&#x200B;**[!UICONTROL %]**&#x200B;或&#x200B;**[!UICONTROL View spend by]**。

   1. 要编辑计划的详细信息，请选择&#x200B;**[!UICONTROL Edit details]**：

      1. 在&#x200B;**[!UICONTROL Setup]**&#x200B;部分中：

         1. 输入&#x200B;**[!UICONTROL Plan name]**，例如`Demo plan`。 输入&#x200B;**[!UICONTROL Description]**，例如`Demo plan for Luma company`。
         1. 从&#x200B;**[!UICONTROL Model]**&#x200B;中选择&#x200B;**[!UICONTROL _选择一个选项……_.]**

            ![计划设置](/help/assets/plan-setup.png)

      1. 在&#x200B;**[!UICONTROL Goal]**&#x200B;部分中，选择要优化计划的目标。 您可以选择
         - **[!UICONTROL I have a budget to spend]**

           ![计划预算](../assets/plan-budget.png)

           此选项允许您为一个或多个日期范围输入预算。

            1. 在&#x200B;**[!UICONTROL Optimize]**&#x200B;容器中：
               1. 从&#x200B;**[!UICONTROL Select conversion]**&#x200B;下拉菜单中选择转换。
               1. 从&#x200B;**[!UICONTROL Select model]**&#x200B;下拉菜单中选择模型。
            1. 通过键入日期或使用&#x200B;**[!UICONTROL Date range]**&#x200B;日历![选择日期范围来指定](/help/assets/icons/Calendar.svg)。
            1. 输入&#x200B;**[!UICONTROL Budget]**。
若要添加其他日期范围（每个日期范围都有预算），请选择![日历添加](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**。
要删除日期范围和相关预算，请选择![关闭](/help/assets/icons/Close.svg)。
            1. 要定义要限制计划的可选最大预算，请执行以下操作：
               1. 打开&#x200B;**[!UICONTROL Maximize budget]**。
               1. 指定最大预算的金额。 金额应等于或高于为日期范围指定的预算总额。


         - **[!UICONTROL I have a target to achieve]** [!BADGE Beta]

           ![计划目标](../assets/plan-target.png)

            1. 在&#x200B;**[!UICONTROL Optimize]**&#x200B;容器中
               1. 从&#x200B;**[!UICONTROL Select conversion]**&#x200B;下拉菜单中选择转换。
               1. 从&#x200B;**[!UICONTROL Select target metric]**&#x200B;下拉菜单中选择一个目标量度。 您可以选择介于&#x200B;**[!UICONTROL Conversion]**、**[!UICONTROL CPA]**、**[!UICONTROL Revenue]**&#x200B;或&#x200B;**[!UICONTROL ROI]**&#x200B;之间。
               1. 从&#x200B;**[!UICONTROL Select model]**&#x200B;下拉菜单中选择模型。
            1. 通过键入日期或使用![日历](/help/assets/icons/Calendar.svg)选择日期范围来指定日期范围。
            1. 输入所选目标度量的值。 例如，**[!UICONTROL Conversion]**&#x200B;的数字、**[!UICONTROL ROI]**&#x200B;的百分比或&#x200B;**[!UICONTROL CPA]**&#x200B;和&#x200B;**[!UICONTROL Revenue]**的货币值。
要添加其他日期范围（每个日期范围都有其目标指标），请选择![CalendarAdd](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**。
要删除日期范围和关联的目标量度，请选择![关闭](/help/assets/icons/Close.svg)。
            1. 要定义要限制计划的可选最大预算，请执行以下操作：
               1. 打开&#x200B;**[!UICONTROL Maximize budget]**。
               1. 指定最大预算的金额。

         1. 选择&#x200B;**[!UICONTROL Next]**&#x200B;以返回到&#x200B;**[!UICONTROL Spend selection]**&#x200B;分区。

1. 在&#x200B;**[!UICONTROL Advanced configuration]**&#x200B;部分中：

   ![编辑高级配置](../assets/edit-plan-advanced-configuration.png)

   - 汇总您的计划名称、模型、日期范围和总预算。

   - 默认情况下，Mix Modeler会使用最新的历史季节性数据自动计算每次转换的平均收入。 在&#x200B;**[!UICONTROL Average Revenue per conversion]**&#x200B;中，您可以定义每次转换的特定平均收入。

   1. 对于预算中的每个日期范围：
      1. 从&#x200B;**[!UICONTROL Date range]**&#x200B;下拉菜单中选择一个日期范围。
      1. 输入&#x200B;**[!UICONTROL Average revenue]**&#x200B;值。
   1. 选择![AddCircle](/help/assets/icons/AddCircle.svg)添加每个转化单位的自定义平均收入以添加日期范围。
   1. 选择![RemoveCircle](/help/assets/icons/RemoveCircle.svg)以删除日期范围。

   >[!NOTE]
   >
   >如果您的模型不包括历史收入数据，则必须为为预算指定的每个日期范围定义每次转换的平均收入。
   >

   - 默认情况下，Mix Modeler会使用最新的历史季节性数据自动计算渠道成本。 在&#x200B;**[!UICONTROL Channel costs]**&#x200B;中，您可以定义自定义渠道成本。

   1. 对于模型中的每个渠道，定义自定义渠道成本。
      1. 从&#x200B;**[!UICONTROL Channel]**&#x200B;下拉菜单中选择一个渠道。
      1. 对于预算中的每个日期范围：
         1. 从&#x200B;**[!UICONTROL Date range]**&#x200B;下拉菜单中选择一个日期范围。
         1. 输入&#x200B;**[!UICONTROL Average revenue]**&#x200B;值。
      1. 选择![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom average revenue per conversion unit]**&#x200B;以添加日期范围。
      1. 选择![RemoveCircle](/help/assets/icons/RemoveCircle.svg)以删除日期范围。

   1. 选择![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom channel cost]**&#x200B;以添加频道。
   1. 选择![CrossSize400](/help/assets/icons/CrossSize400.svg)以删除自定义渠道。


1. 完成计划编辑后，选择&#x200B;**[!UICONTROL Edit]**。

   在&#x200B;**[!UICONTROL All changes are final]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL OK]**&#x200B;以更新计划的当前支出分配以及ROI和收入预测。 选择&#x200B;**[!UICONTROL Cancel]**&#x200B;以取消计划的更新。


- 要随时取消计划更新，请选择&#x200B;**[!UICONTROL Cancel]**。 在&#x200B;**[!UICONTROL No work will be saved]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL Cancel]**&#x200B;以继续处理您的计划，或者选择&#x200B;**[!UICONTROL OK]**&#x200B;以返回到“计划”界面。
- 要返回向导，请选择&#x200B;**[!UICONTROL Back]**。
