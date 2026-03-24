---
title: 数据集规则
description: 了解如何定义Mix Modeler规则，以将其用作在Dataset中协调数据的一部分。
feature: Harmonized Data, Dataset Rules
exl-id: 57d7940a-2900-4814-a30d-bb02bff7615d
source-git-commit: 9987c845414fa5a3abda201d55f7b1ed6e211780
workflow-type: tm+mt
source-wordcount: '2106'
ht-degree: 3%

---

# 数据集规则

数据集规则可帮助您使用在Mix Modeler中获取的数据中的字段来映射协调的字段。

* 对于在Adobe Experience Platform中摄取的聚合数据，可将一个或多个可用数据集字段映射到相应的协调字段。
* 对于事件数据，您可以直接或使用条件将一个或多个协调的字段单独映射到数据集中的字段。


## 管理数据集规则

要查看可用数据集规则的表，请在Mix Modeler界面中执行以下操作：

1. 从左边栏中选择![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]**。

1. 从顶栏中选择&#x200B;**[!UICONTROL Dataset rules]**。 您会看到数据集规则的表。

您可以使用![搜索](/help/assets/icons/Search.svg) **[!UICONTROL _输入数据集名称_]**&#x200B;快速搜索数据集。

表列指定有关数据集规则的详细信息：

| 列名 | 详细信息 |
| ---------------------- | ----------|
| **[!UICONTROL Dataset]** | 数据集的名称。  使用![更多](/help/assets/icons/More.svg)为数据集选择操作。 您可以：<ul><li>![预览](/help/assets/icons/Preview.svg) **[!UICONTROL View]**&#x200B;以查看数据集规则配置。 所有字段都被禁用。</li><li>![编辑](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]**&#x200B;以编辑数据集规则配置。</li><li>![删除](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;以删除数据集规则配置。 系统会在“删除数据集”对话框中提示您确认删除操作。 选择&#x200B;**[!UICONTROL Delete]**&#x200B;以永久删除数据集规则配置。</li><ul> |
| **[!UICONTROL Source]** | 数据集的源：Adobe Analytics、Experience Events、Summary（聚合）或Consumer Experience Events。 |
| **[!UICONTROL Schema]** | 数据集所遵循的架构。 您可以快速选择架构名称，以在![架构](/help/assets/icons/Schemas.svg) [架构](../ingest-data/schemas.md)中架构编辑器的新选项卡中打开架构。 |
| **[!UICONTROL Granularity]** | 数据集中的数据粒度。 可能的值包括“每日”、“每周”、“每月”或“每年”。 |
| **[!UICONTROL Start of the week]** | 指定将特定数据集视为一周中新的一周的开始。 |
| **[!UICONTROL Status]** | 字段的状态： ![StatusGray](/help/assets/icons/StatusGray.svg)草稿或![StatusGreen](/help/assets/icons/StatusGreen.svg)活动 |
| **[!UICONTROL Last modified]** | 上次修改数据集规则的数据和时间。 |

{style="table-layout:auto"}

### 创建数据集规则

若要创建数据集规则，请在Mix Modeler的![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]**&#x200B;界面中，在&#x200B;**[!UICONTROL Dataset rules configuration]**&#x200B;向导中选择&#x200B;**[!UICONTROL Create a dataset rule]**。

在&#x200B;**[!UICONTROL Create]**&#x200B;屏幕中，

1. 在&#x200B;**[!UICONTROL Dataset details]**&#x200B;中，从&#x200B;**[!UICONTROL Select dataset]**&#x200B;中选择一个数据集以开始配置。 在列表中，数据集在&#x200B;**[!UICONTROL Summary]**、**[!UICONTROL Adobe Analytics]**、**[!UICONTROL Experience Event]**、**[!UICONTROL Factors]**&#x200B;和&#x200B;**[!UICONTROL Consumer Experience Events]**&#x200B;中分类。

1. 为&#x200B;**[!UICONTROL Start of the week]**&#x200B;选择一天。

1. 为&#x200B;**[!UICONTROL Granularity]**&#x200B;选择&#x200B;**[!UICONTROL Daily]**、**[!UICONTROL Weekly]**、**[!UICONTROL Monthly]**&#x200B;或&#x200B;**[!UICONTROL Yearly]**。

1. 当您选择了&#x200B;**[!UICONTROL Summary]**&#x200B;或&#x200B;**[!UICONTROL Factors]**&#x200B;类别的数据集时，请为&#x200B;**[!UICONTROL Data restatement is by]**&#x200B;选择&#x200B;**[!UICONTROL Aggregation]**&#x200B;或&#x200B;**[!UICONTROL Replacement]**。

   对于营销分析师来说，来自出版商的报告数据非常重要，因为与出版商合作通常意味着大笔支出，而报告数据的变化可能导致截然不同的洞察力和投资计划。 此外，营销分析师需要准确的数据以获得正确的洞察力，并提出令人信服的提议以获得利益相关者的信心。 但是，这些发布者(例如Google和Facebook)在调整数据时经常会重新声明或删除报告数据。 大多数更改的时间范围在报告媒体性能后的7天内。 30天内还可以对数据做其他更改。 通常，在30天后，书籍将被视为已结案且数据已完成。

   Mix Modeler支持数据重述。 确保用于报告、建模和规划的数据准确无误。 这些数据能够支持品牌和营销分析师的期望和需求。

   您可以将重述摘要数据行作为Experience Platform数据集中的增量行发送，并且协调服务使用该重述数据更新协调数据集。 同样，您还可以删除需要在协调服务中反映的汇总数据行。

1. 在&#x200B;**[!UICONTROL Map to harmonized fields]**&#x200B;部分，从&#x200B;**[!UICONTROL Standard harmonized field]**&#x200B;中选择一个协调的字段。 要快速[创建新的协调字段](/help/harmonize-data/fields.md#add-a-harmonized-field)，请选择&#x200B;**[!UICONTROL Create new]**。

   * 当选定的协调字段的类型为指标时：

      1. 从&#x200B;**[!UICONTROL Mapping type]**&#x200B;中选择&#x200B;**[!UICONTROL Count]**&#x200B;或&#x200B;**[!UICONTROL Sum]**。

      1. 选择您希望协调字段默认映射到的&#x200B;**[!UICONTROL *AEP数据集字段&#x200B;*]**。

   * 当选定字段的类型为维时：

      1. 从&#x200B;**[!UICONTROL Mapping type]**&#x200B;中选择&#x200B;**[!UICONTROL Map Into]**&#x200B;或&#x200B;**[!UICONTROL Case]**。

      1. 当您选择了&#x200B;**[!UICONTROL Map Into]**&#x200B;时，请选择&#x200B;**[!UICONTROL Field]**&#x200B;和&#x200B;**[!UICONTROL *AEP数据集字段&#x200B;*]**或&#x200B;**[!UICONTROL Value]**以及默认值，以将协调的字段默认映射到数据集字段或输入的值。

      1. 当您选择&#x200B;**[!UICONTROL Case]**&#x200B;时，请选择&#x200B;**[!UICONTROL Field]**&#x200B;和&#x200B;**[!UICONTROL *AEP数据集字段&#x200B;*]**或&#x200B;**[!UICONTROL Value]**以及默认值，以将协调的字段默认映射到数据集字段或输入的值。

         1. 要显式设置值，可定义一个或多个由一个或多个条件组成的情况。 每个条件都可以检查特定&#x200B;**[!UICONTROL *AEP数据集字段&#x200B;*]**是&#x200B;**[!UICONTROL Exists]**还是&#x200B;**[!UICONTROL Not Exists]**，是否&#x200B;**[!UICONTROL Contains]**、**[!UICONTROL Not Contains]**、**[!UICONTROL Equals]**、**[!UICONTROL Not Equals]**、**[!UICONTROL Starts With]**或&#x200B;**[!UICONTROL Ends With]**在**[!UICONTROL *&#x200B;输入值&#x200B;*]**&#x200B;处输入的值。

         1. 要添加其他案例，请选择![添加](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add case]**；要添加其他条件，请选择![添加](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add condition]**。

         1. 要删除案例或条件，请在相应的容器中选择![关闭](/help/assets/icons/Close.svg)。

         1. 要选择任何条件或所有条件是否适用于案例，请选择&#x200B;**[!UICONTROL Any of]**&#x200B;或&#x200B;**[!UICONTROL All of]**。

         1. 若要设置案例的结果值，请在&#x200B;**[!UICONTROL Then]**&#x200B;处输入值。

     以下示例所示：

      * 使用&#x200B;**[!UICONTROL Map Into]** **[!UICONTROL Mapping type]**&#x200B;将&#x200B;**[!UICONTROL Channel Type At Source]**&#x200B;协调字段映射到&#x200B;**[!DNL Luma Transactions]**&#x200B;数据集中的&#x200B;**[!UICONTROL channel_type]**&#x200B;字段。

      * 使用&#x200B;**[!UICONTROL Case]** **[!UICONTROL Mapping type]**&#x200B;将&#x200B;**[!DNL Luma Transactions]**&#x200B;数据集中的&#x200B;**[!UICONTROL marketing.campaignName]**&#x200B;字段的值有条件地映射到&#x200B;**[!UICONTROL Campaign]**&#x200B;协调字段。 “市场活动协调”字段设置为：

         * **[!UICONTROL marketing.campaignName]**&#x200B;为`_black_friday`或`BlackFriday`时为`Black Friday`。
         * 设置为&#x200B;**[!UICONTROL marketing.campaignName]**&#x200B;的值。

        ![数据集规则事件](/help/assets/dataset-create-event.png)

1. 选择![添加](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add field]**&#x200B;以定义其他字段。

完成后，选择&#x200B;**[!UICONTROL Save as draft]**&#x200B;保存规则的草稿版本，或选择&#x200B;**[!UICONTROL Save]**&#x200B;保存并激活规则。 选择“**[!UICONTROL Cancel]**”以取消规则配置。

>[!NOTE]
>
>摘要数据集规则的专用&#x200B;**[!UICONTROL Map to harmonized fields]**&#x200B;体验已弃用。 现在，无论数据集类型如何，所有数据集规则都使用类似的&#x200B;**[!UICONTROL Map to harmonized fields]**&#x200B;体验。 对于已使用已弃用的&#x200B;**[!UICONTROL Map to harmonized fields]**&#x200B;体验定义规则的摘要数据集，可能需要根据通用&#x200B;**[!UICONTROL Map to harmonized field]**&#x200B;体验验证这些规则。
>

#### 摘要数据集

当您从汇总数据集中映射标准协调字段时，Mix Modeler会尝试推导相应的Experience Platform数据集字段。 成功时：

* 如果该字段的维度类型，则选择&#x200B;**[!UICONTROL Map into]**&#x200B;作为&#x200B;**[!UICONTROL Mapping type]**。
* 如果该字段为度量类型，则选择&#x200B;**[!UICONTROL Sum]**&#x200B;作为&#x200B;**[!UICONTROL Mapping type]**。
* 已选择&#x200B;**[!UICONTROL Field]**&#x200B;作为&#x200B;**[!UICONTROL Default]**&#x200B;映射类型。
* 为&#x200B;*AEPExperience Platform集字段*&#x200B;自动插入相应的数据集字段。

如果任何建议值不正确或不支持您的特定用例，则可以更改这些值。


#### 因子数据集

将协调的字段映射到因子数据集中的字段，这样您可以[添加因子作为模型配置的一部分](/help/models/build.md)。

将协调后的字段映射到因子数据集中的字段时，适用以下情况：

##### 因子名称

当您从因子数据集映射标准协调因子字段，并且因子数据集包含单个因子时，请使用&#x200B;**[!UICONTROL Map into]**&#x200B;作为&#x200B;**[!UICONTROL Mapping type]**，并为&#x200B;**[!UICONTROL Factor Name]**&#x200B;协调字段输入默认值。

![数据集规则 — 映射单因素数据集](../assets/dataset-create-rule-factor-single.png)

如果因子数据集包含多个因子，请使用&#x200B;**[!UICONTROL Case As]**&#x200B;作为&#x200B;**[!UICONTROL Mapping Type]**&#x200B;来定义协调的因子名称字段和每个不同的因子名称之间的映射。

![数据集规则 — 映射单因素数据集](../assets/dataset-create-rule-factor-multiple.png)


##### 因子类型

此字段在因子数据集和架构中是可选的。 如果在因子数据集和架构中定义了&#x200B;**[!UICONTROL Factor type]**&#x200B;并指定了&#x200B;**[!UICONTROL Internal]**&#x200B;或&#x200B;**[!UICONTROL External]**，则使用提供的值。 如果未指定值，则使用默认值&#x200B;**[!UICONTROL Internal]**。

##### 值类型

此字段在因子数据集和架构中是可选的。 如果在因子数据集和架构中定义了&#x200B;**[!UICONTROL Value type]**&#x200B;并指定了&#x200B;**[!UICONTROL Actual]**&#x200B;或&#x200B;**[!UICONTROL Forecasted]**，则使用提供的值。 如果未指定值，则使用默认值&#x200B;**[!UICONTROL Actual]**。


##### 粒度

当因子数据集中的所有因子都具有相同的源粒度时，您可以为因子数据集的粒度定义数据集规则。

一旦协调了因子数据集，所有数据集就会符合协调的数据集的最高粒度级别。


##### 因子值

对于&#x200B;**[!UICONTROL Factor value]**&#x200B;协调字段，请使用聚合运算符之一作为&#x200B;**[!UICONTROL Mapping Type]**。 在因子数据集中定义多个因子时，聚合运算符将应用于所有因子。


##### 示例

* 您有一个因子数据集，其中包含下列示例数据：

  | 时间戳 | 因子名称 | 因子值 |
  |---|---|---:|
  | 2025年3月13日 | _definedsp500 | 10 |
  | 2025年3月13日 | _cpi | 20 |
  | 2025年3月14日 | _definedsp500 | 30 |
  | 2025年3月14日 | _cpi | 40 |
  | 2025年3月15日 | _definedsp500 | 50 |
  | 2025年3月15日 | _cpi | 60 |


* 您为&#x200B;**[!UICONTROL Factor Name]**、**[!UICONTROL Factor Value]**&#x200B;和&#x200B;**[!UICONTROL Granularity]**&#x200B;定义以下数据集规则：

  ![数据集规则 — 因子示例](../assets/dataset-create-rule-factor-example.png)

* 然后，这将产生以下统一数据：

  | 因子名称 | 因子值 | 因子类型 | 值类型 |
  |---|---:|---|---|
  | CPI | 20 | 内部 | 实际 |
  | 标准普尔500指数 | 10 | 内部 | 实际 |

  由于没有为&#x200B;**[!UICONTROL Factor Type]**&#x200B;和&#x200B;**[!UICONTROL Value Type]**&#x200B;定义数据集规则，因此使用默认值。

### 编辑数据集规则

要编辑数据集规则，请在Mix Modeler的![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]**&#x200B;界面中：

1. 在要编辑的数据集规则的&#x200B;**[!UICONTROL Dataset]**&#x200B;列中选择![更多](/help/assets/icons/More.svg)。
1. 从上下文菜单中选择![编辑](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]**&#x200B;以开始编辑数据集规则。 有关更多详细信息，请参阅[创建数据集规则](#create-a-dataset-rule)。


### 删除数据集规则

要删除数据集规则，请在Mix Modeler的![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]**&#x200B;界面中：

1. 在要删除的数据集规则&#x200B;**[!UICONTROL Dataset]**&#x200B;列中选择![更多](/help/assets/icons/More.svg)。
1. 从上下文菜单中选择![删除](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;以删除数据集规则。 系统会提示您进行确认。 选择&#x200B;**[!UICONTROL Delete]**&#x200B;以永久删除所选数据集规则。



## 同步数据

在应用数据集规则中的逻辑时，要在协调的数据与汇总和/或事件数据集之间同步数据，请执行以下操作：

1. 选择 **[!UICONTROL Sync data]**。

1. 从&#x200B;**[!UICONTROL Sync data for dataset rules]**&#x200B;对话框中，选择
   * **[!UICONTROL Refresh harmonized data for summary datasets]**,
   * **[!UICONTROL Refresh harmonized data for event datasets]**，或
   * **[!UICONTROL Refresh harmonized data for both summary + event datasets]**.

1. 若要根据已定义的数据集规则在数据集中的协调数据和数据之间启动同步，请选择“**[!UICONTROL Sync]**”。 若要取消同步，请选择&#x200B;**[!UICONTROL Cancel]**。

   ![同步数据](/help/assets/sync-data.png)


## 数据合并偏好设置 {#data-merge-preferences}


>[!CONTEXTUALHELP]
>id="harmonizeddata_datasetrules_datamergepreferences"
>title="默认量度偏好"
>abstract="在数据协调过程中，当多个数据源尝试更新某个渠道的量度字段时，将应用默认偏好设置。 该偏好在沙盒级别生效，除非在下方为特定量度偏好进行了覆盖设置。"


>[!NOTE]
>
>[!BADGE Beta]{type=Informative}数据合并首选项是Beta版功能，其功能可能会发生变化。

要确保精确的模型预测，可以定义数据合并首选项。 此功能使用户能够解决在合并摘要级别和事件级别数据之后的任何冲突。

可以配置默认度量首选项，以便在发生更新冲突时应用。 此默认度量可以是以下三个选项之一：

* **[!UICONTROL Summary data]**
* **[!UICONTROL Sum of summary and event data]**
* **[!UICONTROL Event data]**

在协调过程中，当多个数据源尝试更新给定渠道的度量字段时，将应用用户配置的默认首选项。 此首选项适用于沙箱级别，除非另外配置某些基于度量的首选项，否则将覆盖此首选项。

在&#x200B;**[!UICONTROL Metric based preferences]**&#x200B;下，用户可以针对给定度量配置特定源（**[!UICONTROL Summary]**&#x200B;或&#x200B;**[!UICONTROL Event]**）以及该度量的相应转换类型。

典型用例包括：

* 在多个数据集中测量和报告相同的广告量度，或者
* 度量度量在某些数据集中可能不完整，而另一个数据集可能是特定度量的超集，导致重复计数。

### 配置

要配置数据合并首选项，请执行以下操作：


1. 选择![数据合并首选项](/help/assets/icons/Merge.svg) [!BADGE 测试版]。

1. 在&#x200B;**[!UICONTROL Data merge preferences]** [!BADGE 测试版]{type=Informative}对话框中：

   ![数据合并首选项](/help/assets/data-merge-preferences.png)

   * 选择&#x200B;**[!UICONTROL Default metric preference]**。 在协调过程中，当多个数据源更新给定渠道的度量字段时，将应用选定的默认度量首选项。 该首选项将应用于沙箱级别，除非基于特定度量的首选项会覆盖该首选项。 您可以在&#x200B;**[!UICONTROL Summary data]**、**[!UICONTROL Event data]**&#x200B;和&#x200B;**[!UICONTROL Sum of summary and event data]**&#x200B;之间进行选择。

   * 要添加基于特定度量的首选项，请执行以下操作：

      1. 选择“![加](/help/assets/icons/AddCircle.svg)”**[!UICONTROL Add a metric]**。
         1. 从&#x200B;**[!UICONTROL *度量选择&#x200B;*]**列表中选择度量。
         1. 选择 **[!UICONTROL CHANNELS]** 或 **[!UICONTROL CONVERSION TYPES]**。 从列表中选择&#x200B;**[!UICONTROL All]**&#x200B;或特定通道或转换类型。
         1. 选择“**[!UICONTROL Summary]**”或“**[!UICONTROL Event]**”以指定合并数据时是否优先使用摘要数据或事件数据作为度量（以及所有或所选通道）。

         要添加一个或多个其他通道或转换类型，请执行以下操作：

         1. 选择![加](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a channel]**&#x200B;或![加](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a conversion type]**。
         1. 选择 **[!UICONTROL Summary]** 或 **[!UICONTROL Event]**。

         若要删除通道或转换类型，请选择![交叉](/help/assets/icons/Close.svg)。

      1. 要添加更具体的基于度量的首选参数，请重复上一步骤。

   * 要删除现有的特定基于度量的首选项，请选择![删除](/help/assets/icons/Delete.svg)。

1. 选择“**[!UICONTROL Save]**”以保存数据合并首选项。 开始重新同步数据。<br/>选择“**[!UICONTROL Cancel]**”以取消。

## 删除源数据集

当您删除协调数据中使用的源数据集时，将从[[!UICONTROL Harmonized data]](/help/harmonize-data/overview.md)中删除该源数据集上的基础条目。 但是，具有已删除源数据集的数据集规则仍保留在数据集规则配置列表中，带有图标![DataRemove](/help/assets/icons/DataRemove.svg)，指示源数据集已删除。 要获取更多详细信息，请执行以下操作：

* 从上下文菜单中选择![更多](/help/assets/icons/More.svg)和![预览](/help/assets/icons/Preview.svg) **[!UICONTROL View]**。
**[!UICONTROL Dataset rule mapping - Fields]**&#x200B;对话框显示有关已删除源数据集的信息以及数据集规则配置中使用的字段。

返回&#x200B;**[!UICONTROL Dataset rules]**&#x200B;配置时，您会看到一个对话框，说明一个或多个源数据集已被删除。 协调后的数据会在下一次临时同步或计划同步时受到影响。 查看数据集规则配置。

经过协调后的数据将在下次临时同步或计划同步时更新，而不包含已删除的源数据。 但是，您仍然会看到警告对话框，提示您根据已删除的源数据集删除数据集规则。 此警报允许用户查看和评估已删除数据集中的受影响字段。 以及确定对于任何模型中可能使用的营销接触点或转换的影响。 查看并减轻此影响后，您应从数据集规则配置列表中删除数据集规则。
