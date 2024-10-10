---
title: 创建模型
description: 了解如何在Mix Modeler中创建模型。
feature: Models
exl-id: e1093c09-1e23-460b-92de-cfb0061112fd
source-git-commit: 1327ef083cc681b38adc086ad4f7332fd83577b5
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---

# 创建模型

要创建模型，请在Mix Modeler的![模型](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**&#x200B;界面中选择&#x200B;**[!UICONTROL Open model canvas]**。

为了构建自定义AI支持的模型，界面提供了分步引导式模型配置流程。

1. 在&#x200B;**[!UICONTROL Setup]**&#x200B;步骤中：

   1. 输入您的模型&#x200B;**[!UICONTROL Name]**，例如`Demo model`。 输入&#x200B;**[!UICONTROL Description]**，例如`Demo model to explore AI featues of Mix Modeler`。

      ![模型名称和描述](/help/assets/model-name-description.png)

   1. 选择&#x200B;**[!UICONTROL Next]**&#x200B;以继续下一步骤。 选择&#x200B;**[!UICONTROL Cancel]**&#x200B;取消模型配置。

1. 在&#x200B;**[!UICONTROL Configure]**&#x200B;步骤中：

   1. 在&#x200B;**[!UICONTROL Conversion goal]**&#x200B;部分中：

      ![模型 — 转换步骤](/help/assets/model-conversion-step.png)

      1. 从&#x200B;**[!UICONTROL Conversion]**&#x200B;下拉菜单中选择转换。 可用转化是您在[!UICONTROL Harmonized datasets]中定义为[转化](../harmonize-data/conversions.md)一部分的转化。 例如：**[!UICONTROL Online Conversion]**。

      1. 您可以选择![LinkOutLight](/help/assets/icons/LinkOutLight.svg) **[!UICONTROL Create a conversion]**&#x200B;以直接从模型配置中创建转换。



   1. 在&#x200B;**[!UICONTROL Marketing touchpoints]**&#x200B;部分中，您可以选择一个或多个营销接触点，对应于您在[!UICONTROL Harmonized datasets]中定义为[营销接触点](../harmonize-data/marketing-touchpoints.md)一部分的营销接触点。


      ![模型 — 营销接触点步骤](/help/assets/model-marketing-touchpoint-step.png)

      1. 从&#x200B;**[!UICONTROL Touchpoint include]**&#x200B;下拉菜单中选择一个或多个营销接触点。

         * 您可以使用![CrossSize75](/help/assets/icons/CrossSize75.svg)删除接触点。
         * 您可以使用&#x200B;**[!UICONTROL Clear all]**&#x200B;删除所有接触点。

      1. 您可以选择![LinkOutLight](/help/assets/icons/LinkOutLight.svg) **[!UICONTROL Create a touchpoint]**&#x200B;以直接从模型配置中创建营销接触点。

      >[!NOTE]
      >
      >您无法使用具有重叠数据的接触点设置模型，并且必须至少有一个包含支出的接触点。

   1. 默认情况下，会对您协调视图中的所有数据生成一个分数。 要仅对群体的子集进行评分，请使用&#x200B;**[!UICONTROL Eligible data population]**&#x200B;部分中的容器定义一个或多个过滤器。

      ![模型 — 符合条件的数据填充](/help/assets/model-eligible-data-population-step.png)

      * 对于每个容器，定义一个或多个事件。

         1. 对于每个事件：

            1. 从&#x200B;**[!UICONTROL _选择协调字段_]**&#x200B;中选择量度或维度。

            1. 选择适当的运算符： **[!UICONTROL equals]**、**[!UICONTROL not equals]**、**[!UICONTROL less than]**、**[!UICONTROL greater than]**、**[!UICONTROL starts with]**、**[!UICONTROL doesn't start with]**、**[!UICONTROL ends with]**、**[!UICONTROL doesn't end with]**、**[!UICONTROL contains]**、**[!UICONTROL doesn't contain]**、**[!UICONTROL is in]**&#x200B;或&#x200B;**[!UICONTROL is not in]**。

            1. 在&#x200B;**[!UICONTROL _处输入或选择一个值输入或选择值_]**。

         1. 若要在容器中添加其他事件，请选择![添加](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add event]**。

         1. 要从容器中删除事件，请选择![关闭](/help/assets/icons/CrossSize75.svg)。

         1. 要使用容器中定义的所有或多个事件进行筛选，请选择&#x200B;**[!UICONTROL Any of]**&#x200B;或&#x200B;**[!UICONTROL All of]**。 标签相应地从&#x200B;**[!UICONTROL Include ... Or ...]**&#x200B;更改为&#x200B;**[!UICONTROL Include ... And ...]**。

      * 要添加符合条件的数据填充容器，请选择![添加](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add eligible population]**。

      * 要删除符合条件的数据填充容器，请在容器中选择![更多](/help/assets/icons/More.svg)，然后从上下文菜单中选择&#x200B;**[!UICONTROL Remove marketing touchpoint]**。



   1. 要将包含外部因素的数据集添加到模型，请在&#x200B;**[!UICONTROL External factors dataset]**&#x200B;部分中使用一个或多个容器。 外部因素的一个例子是标普指数。

      ![模型 — 外部因素数据集](/help/assets/model-external-factors-dataset-step.png)

      * 对于每个容器：

         1. 输入&#x200B;**[!UICONTROL External factor name]**，例如`External Factors`。

         1. 从&#x200B;**[!UICONTROL Dataset]**&#x200B;下拉菜单中选择一个数据集。 您可以选择![数据](/help/assets/icons/Data.svg)来管理数据集。 有关详细信息，请参阅[数据集](../ingest-data/datasets.md)。

         1. 从&#x200B;**[!UICONTROL Impact on conversion]**&#x200B;下拉菜单中选择一个选项： **[!UICONTROL Auto select]**、**[!UICONTROL Positive]**&#x200B;或&#x200B;**[!UICONTROL Negative]**。

      * 要添加额外的外部因子数据集容器，请选择![添加](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add external factor]**。

      * 要删除外部因子数据集容器，请选择![RemoveCircle](/help/assets/icons/RemoveCircle.svg)。




   1. 要将包含内部因子的数据集添加到模型，请在&#x200B;**[!UICONTROL Internal factors dataset]**&#x200B;部分中使用一个或多个容器。 电子邮件营销数据便是内部因素的示例。

      ![模型 — 内部因素数据集](/help/assets/model-internal-factors-dataset-step.png)

      * 对于每个容器：

         1. 输入&#x200B;**[!UICONTROL Internal factor name]**，例如`Email Marketing Data`。

         1. 从&#x200B;**[!UICONTROL _中选择数据集_]**。 您可以选择![数据](/help/assets/icons/Data.svg)来管理数据集。 有关详细信息，请参阅[数据集](../ingest-data/datasets.md)。

         1. 从&#x200B;**[!UICONTROL Impact on conversion]**&#x200B;下拉菜单中选择一个选项： **[!UICONTROL Auto select]**、**[!UICONTROL Positive]**&#x200B;或&#x200B;**[!UICONTROL Negative]**。

      * 要添加其他内部因子数据集容器，请选择![添加](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add internal factor]**。

      * 要删除内部因子数据集容器，请选择![RemoveCircle](/help/assets/icons/RemoveCircle.svg)。



   1. 要定义模型的回顾时间范围，请在&#x200B;**[!UICONTROL Give contribution credit to touchpoints occurring within]** ... **[!UICONTROL weeks prior to the conversion]**&#x200B;中输入一个介于`1`和`52`之间的值。

   1. 选择&#x200B;**[!UICONTROL Next]**&#x200B;以继续下一步骤。 如果需要更多配置，请使用红色轮廓和文本说明需要哪些其他配置。 <br/>选择&#x200B;**[!UICONTROL Back]**&#x200B;以返回上一步。 <br/>选择&#x200B;**[!UICONTROL Cancel]**&#x200B;取消模型配置。

1. 在&#x200B;**[!UICONTROL Advanced]**&#x200B;步骤中：

   1. 在&#x200B;**[!UICONTROL Define training window]**&#x200B;部分中，选择

      * **[!UICONTROL Have Mix Modeler select a helpful training window]**&#x200B;和

      * **[!UICONTROL Manually input a training window]**&#x200B;的问题。选中后，在&#x200B;**[!UICONTROL Include events the following years prior to a conversion]**&#x200B;中定义年数。

        ![模型 — 定义训练时段](/help/assets/model-define-training-window.png)

   1. 在&#x200B;**[!UICONTROL Spend share]**&#x200B;部分中：

      * 要在营销数据稀疏时使用历史营销投资比率通知模型，请激活&#x200B;**[!UICONTROL Allow spend share]**。

   1. 在&#x200B;**[!UICONTROL MTA enabled]**&#x200B;部分中：

      * 要为模型启用MTA功能，请激活&#x200B;**[!UICONTROL MTA enabled]**。 如果您已启用MTA，则在培训模型和为模型评分后，即可使用多点接触归因分析。 在[模型分析](insights.md)中查看[归因](insights.md#attribution)选项卡。

   1. 在&#x200B;**[!UICONTROL Prior knowledge]**&#x200B;部分中：

      ![模型 — 先验知识](/help/assets/model-prior-knowledge-step.png)

      1. 选择默认为&#x200B;**[!UICONTROL Absolute values]**&#x200B;的&#x200B;**[!UICONTROL Rule type]**。

      1. 使用&#x200B;**[!UICONTROL Contribution proportion]**&#x200B;列为&#x200B;**[!UICONTROL Name]**&#x200B;下列出的任何渠道指定贡献百分比。

      1. 在适当的情况下，您可以为每个渠道添加&#x200B;**[!UICONTROL Level of confidence]**&#x200B;百分比。

      1. 需要时，使用&#x200B;**[!UICONTROL Clear all]**&#x200B;清除&#x200B;**[!UICONTROL Contribution proportion]**&#x200B;和&#x200B;**[!UICONTROL Level of confidence]**&#x200B;列的所有输入值。



1. 选择&#x200B;**[!UICONTROL Finish]**&#x200B;以完成模型配置。

   * 在&#x200B;**[!UICONTROL Create instance?]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL Ok]**&#x200B;以立即触发第一组训练和评分运行。 您的模型已列出，状态为![StatusOrange](/help/assets/icons/StatusOrange.svg) **[!UICONTROL Awaiting training]**。

     选择要取消的&#x200B;**[!UICONTROL Cancel]**。

   * 如果需要更多配置，请使用红色轮廓和文本说明需要哪些其他配置。

   选择&#x200B;**[!UICONTROL Back]**&#x200B;以返回上一步。

   选择&#x200B;**[!UICONTROL Cancel]**&#x200B;取消模型配置。
