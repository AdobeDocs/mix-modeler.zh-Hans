---
title: 数据集规则
description: 了解如何在Mix Modeler中定义要用作协调数据一部分的数据集规则。
feature: Harmonized Data, Dataset Rules
exl-id: 57d7940a-2900-4814-a30d-bb02bff7615d
source-git-commit: b631cf8d06fe71d9f5ca547923eb3237c677a915
workflow-type: tm+mt
source-wordcount: '1696'
ht-degree: 0%

---

# 数据集规则

数据集规则可帮助您将协调的字段与您在Mix Modeler中摄取的数据中的字段进行映射。

* 对于在Adobe Experience Platform中摄取的聚合数据，可将一个或多个可用数据集字段映射到相应的协调字段。
* 对于事件数据，您可以直接或使用条件将一个或多个协调的字段单独映射到数据集中的字段。


## 管理数据集规则

要查看可用数据集规则的表，请在Mix Modeler界面中执行以下操作：

1. 从左边栏中选择![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]**。

1. 从顶部栏中选择&#x200B;**[!UICONTROL Dataset rules]**。 您会看到数据集规则的表。

您可以使用![搜索](/help/assets/icons/Search.svg)快速搜索数据集&#x200B;**[!UICONTROL _输入数据集名称_]**。

表列指定有关数据集规则的详细信息：

| 列名称 | 详细信息 |
| ---------------------- | ----------|
| 数据集 | 数据集的名称。  使用![更多](/help/assets/icons/More.svg)为数据集选择操作。 您可以：<ul><li>![预览](/help/assets/icons/Preview.svg) **[!UICONTROL View]**&#x200B;以查看数据集规则配置。 所有字段均被禁用。</li><li>![编辑](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]**&#x200B;以编辑数据集规则配置。</li><li>![删除](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;以删除数据集规则配置。 系统会提示您在“删除数据集”对话框中确认删除。 选择&#x200B;**[!UICONTROL Delete]**&#x200B;以永久删除数据集规则配置。</li><ul> |
| 来源 | 数据集的来源： Adobe Analytics、体验事件、摘要（汇总）或使用者体验事件。 |
| 架构 | 数据集符合的架构。 您可以在![架构](/help/assets/icons/Schemas.svg) [架构](../ingest-data/schemas.md)的架构编辑器中，快速选择架构名称以在新选项卡中打开架构。 |
| 粒度 | 数据集中的数据粒度。 可能的值包括“每日”、“每周”、“每月”或“每年”。 |
| 一周开始 | 指定将一周中的哪一天视为特定数据集的新周的开始。 |
| 状态 | 字段的状态： <p><span style="color:gray">●</span>草稿或 <p><span style="color:green">●</span>处于活动状态 |
| 上次修改时间 | 上次修改数据集规则的数据和时间。 |

{style="table-layout:auto"}

### 创建数据集规则

要创建数据集规则，请在Mix Modeler的![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]**&#x200B;界面中，在&#x200B;**[!UICONTROL Create a dataset rule]**&#x200B;向导中选择&#x200B;**[!UICONTROL Dataset rules configuration]**。

在&#x200B;**[!UICONTROL Create]**&#x200B;屏幕中，

1. 在&#x200B;**[!UICONTROL Dataset details]**&#x200B;中，从&#x200B;**[!UICONTROL Select dataset]**&#x200B;中选择数据集以开始配置。 在列表中，数据集在&#x200B;**[!UICONTROL Consumer Experience Events]**、**[!UICONTROL Adobe Analytics]**、**[!UICONTROL Experience Event]**&#x200B;和&#x200B;**[!UICONTROL Summary]**&#x200B;中分类。

1. 为&#x200B;**[!UICONTROL Start of the week]**&#x200B;选择日期。

1. 为&#x200B;**[!UICONTROL Daily]**&#x200B;选择&#x200B;**[!UICONTROL Weekly]**、**[!UICONTROL Monthly]**、**[!UICONTROL Yearly]**&#x200B;或&#x200B;**[!UICONTROL Granularity]**。

1. 选择&#x200B;**[!UICONTROL Summary]**&#x200B;类别的数据集后，为&#x200B;**[!UICONTROL Aggregation]**&#x200B;选择&#x200B;**[!UICONTROL Replacement]**&#x200B;或&#x200B;**[!UICONTROL Data restatement is by]**。

   对于营销分析人员而言，来自发布者的报表数据非常重要，因为与发布者合作通常意味着大量支出，并且报表数据的更改可能会导致洞察信息和投资计划出现很大差异。 此外，营销分析师需要准确的数据才能获得正确的洞察力，并提出令人信服的提案以获得利益相关者的信心。 但是，这些发布者(如Google和Facebook)在协调数据时通常会重新声明或删除报表数据。 大多数更改的时间范围在报告媒体性能后的7天内。 30天内可能会对数据做其他更改。 通常，在30天后，书籍会被视为已结账且数据已完整。

   Mix Modeler支持数据重述。 确保用于报表、建模和规划的数据准确无误。 并且这些数据能够支持品牌和营销分析师的期望和需求。

   您可以在Experience Platform数据集中将重述的摘要数据行作为增量行发送，协调服务将使用该重述数据更新协调的数据集。 同样，您也可以删除需要反映在协调服务中的汇总数据行。

1. 在&#x200B;**[!UICONTROL Map to harmonized fields]**&#x200B;部分中：

   1. 从&#x200B;**[!UICONTROL Standard harmonized field]**&#x200B;中选择协调字段。

   1. 当所选协调字段为指标类型时：

      1. 从&#x200B;**[!UICONTROL Count]**&#x200B;中选择&#x200B;**[!UICONTROL Sum]**&#x200B;或&#x200B;**[!UICONTROL Mapping type]**。

      1. 选择您希望协调字段默认映射到的&#x200B;**[!UICONTROL *AEP数据集字段&#x200B;*]**。

   1. 当所选字段属于维度类型时：

      1. 从&#x200B;**[!UICONTROL Map Into]**&#x200B;中选择&#x200B;**[!UICONTROL Case]**&#x200B;或&#x200B;**[!UICONTROL Mapping type]**。

      1. 选择&#x200B;**[!UICONTROL Map Into]**&#x200B;后，请选择&#x200B;**[!UICONTROL Field]**&#x200B;和&#x200B;**[!UICONTROL *AEP数据集字段&#x200B;*]**或&#x200B;**[!UICONTROL Value]**以及默认值，以便默认情况下将协调字段映射到数据集字段或输入的值。

      1. 当您选择&#x200B;**[!UICONTROL Case]**&#x200B;时，请选择&#x200B;**[!UICONTROL Field]**&#x200B;和&#x200B;**[!UICONTROL *AEP数据集字段&#x200B;*]**或&#x200B;**[!UICONTROL Value]**以及默认值，以便默认情况下将协调字段映射到数据集字段或输入的值。

         1. 要显式设置值，可定义一个或多个情况，其中包含一个或多个条件。 每个条件都可以检查特定的&#x200B;**[!UICONTROL *AEP数据集字段&#x200B;*]**，无论它是&#x200B;**[!UICONTROL Exists]**还是&#x200B;**[!UICONTROL Not Exists]**，或者它是&#x200B;**[!UICONTROL Contains]**、**[!UICONTROL Not Contains]**、**[!UICONTROL Equals]**、**[!UICONTROL Not Equals]**、**[!UICONTROL Starts With]**还是&#x200B;**[!UICONTROL Ends With]**在**[!UICONTROL *&#x200B;处输入的值输入值&#x200B;*]**。

         1. 要添加另一个案例，请选择![添加](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add case]**；要添加另一个条件，请选择![添加](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add condition]**。

         1. 要删除案例或条件，请在相应的容器中选择![关闭](/help/assets/icons/Close.svg)。

         1. 要选择是应该将任何条件还是所有条件应用于案例，请选择&#x200B;**[!UICONTROL Any of]**&#x200B;或&#x200B;**[!UICONTROL All of]**。

         1. 要设置案例的结果值，请在&#x200B;**[!UICONTROL Then]**&#x200B;处输入值。

      以下示例

      * 使用&#x200B;**[!UICONTROL Map Into]** **[!UICONTROL Mapping type]**&#x200B;将&#x200B;**[!UICONTROL Channel Type At Source]**&#x200B;协调字段映射到&#x200B;**[!UICONTROL channel_type]**&#x200B;数据集中的&#x200B;**[!DNL Luma Transactions]**&#x200B;字段。

      * 使用&#x200B;**[!UICONTROL Case]** **[!UICONTROL Mapping type]**&#x200B;有条件地将&#x200B;**[!UICONTROL marketing.campaignName]**&#x200B;数据集中&#x200B;**[!DNL Luma Transactions]**&#x200B;字段的值映射到&#x200B;**[!UICONTROL Campaign]**&#x200B;协调字段。 Campaign协调字段设置为：

         * `Black Friday`为&#x200B;**[!UICONTROL marketing.campaignName]**&#x200B;或`_black_friday`时的`BlackFriday`。
         * 到所有其它情况下的&#x200B;**[!UICONTROL marketing.campaignName]**&#x200B;的值。

        ![数据集规则事件](/help/assets/dataset-create-event.png)

      当您从摘要数据集中映射标准协调字段时，Mix Modeler会尝试推导相应的Experience Platform数据集字段。 成功后：

      * 如果字段为维度类型，则选择&#x200B;**[!UICONTROL Map into]**&#x200B;作为&#x200B;**[!UICONTROL Mapping type]**。
      * 如果字段为量度类型，则选择&#x200B;**[!UICONTROL Sum]**&#x200B;作为&#x200B;**[!UICONTROL Mapping type]**。
      * 已选择&#x200B;**[!UICONTROL Field]**&#x200B;作为&#x200B;**[!UICONTROL Default]**&#x200B;映射类型。
      * 将自动为&#x200B;*Experience Platform数据集字段*&#x200B;插入相应的AEP数据集字段。

      如果任何建议值不正确或不支持您的特定用例，则可以更改这些值。

1. 选择![添加](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add field]**&#x200B;以定义其他字段。

完成后，选择&#x200B;**[!UICONTROL Save as draft]**&#x200B;以保存规则的草稿版本，或选择&#x200B;**[!UICONTROL Save]**&#x200B;以保存并激活规则。 选择&#x200B;**[!UICONTROL Cancel]**&#x200B;取消规则配置。

>[!NOTE]
>
>摘要数据集规则的专用&#x200B;**[!UICONTROL Map to harmonized fields]**&#x200B;体验已弃用。 现在，无论数据集类型如何，所有数据集规则都使用类似的&#x200B;**[!UICONTROL Map to harmonized fields]**&#x200B;体验。 对于已使用已弃用的&#x200B;**[!UICONTROL Map to harmonized fields]**&#x200B;体验为其定义了规则的摘要数据集，您可能希望根据通用&#x200B;**[!UICONTROL Map to harmonized field]**&#x200B;体验验证这些规则。
>



### 编辑数据集规则

要编辑数据集规则，请在Mix Modeler的![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]**&#x200B;界面中：

1. 在![列中为要编辑的数据集规则选择](/help/assets/icons/More.svg)更多&#x200B;**[!UICONTROL Dataset]**。
1. 从上下文菜单中，选择![编辑](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]**&#x200B;以开始编辑数据集规则。 有关详细信息，请参阅[创建数据集规则](#create-a-dataset-rule)。


### 删除数据集规则

要删除数据集规则，请在Mix Modeler的![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]**&#x200B;界面中：

1. 在![列中为要删除的数据集规则选择](/help/assets/icons/More.svg)更多&#x200B;**[!UICONTROL Dataset]**。
1. 从上下文菜单中，选择![删除](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;以删除数据集规则。 系统会提示您进行确认。 选择&#x200B;**[!UICONTROL Delete]**&#x200B;以永久删除选定的数据集规则。



## 同步数据

要在协调的数据与汇总数据集和/或事件数据集之间同步数据，同时在数据集规则中应用逻辑，请执行以下操作：

1. 选择 **[!UICONTROL Sync data]**。

1. 从&#x200B;**[!UICONTROL Sync data for dataset rules]**&#x200B;对话框中，选择
   * **[!UICONTROL Refresh harmonized data for summary datasets]**，
   * **[!UICONTROL Refresh harmonized data for event datasets]**，或
   * **[!UICONTROL Refresh harmonized data for both summary + event datasets]**。

1. 要根据定义的数据集规则在数据集中的协调数据和数据之间启动同步，请选择&#x200B;**[!UICONTROL Sync]**。 要取消同步，请选择&#x200B;**[!UICONTROL Cancel]**。

   ![同步数据](/help/assets/sync-data.png)


## 数据合并首选项

>[!NOTE]
>
>[!BADGE 测试版]{type=Informative}数据合并首选项是测试版功能，其功能可能会发生更改。

为了确保准确的模型预测，您可以定义数据合并首选项。 此功能使用户能够解决合并摘要级别数据和事件级别数据后的任何冲突。

您可以配置要在更新发生冲突时应用的默认量度首选项。 此默认量度可以是以下三个选项之一：

* **[!UICONTROL Summary data]**
* **[!UICONTROL Sum of summary and event data]**
* **[!UICONTROL Event data]**

在协调期间，当多个数据源尝试更新给定渠道的量度字段时，将应用用户配置的默认首选项。 此首选项应用于沙盒级别，除非被另外配置的特定基于量度的首选项覆盖。

在&#x200B;**[!UICONTROL Metric based preferences]**&#x200B;下，用户可以配置给定量度的特定源（**[!UICONTROL Summary]**&#x200B;或&#x200B;**[!UICONTROL Event]**）以及该量度的相应转化类型。

典型用例包括：

* 在多个数据集中测量和报告相同的广告量度，或
* 某些数据集中的量度测量可能不完整，而另一个数据集可能是特定量度的超集，从而导致重复计数。

### 配置

要配置数据合并首选项，请执行以下操作：


1. 选择![数据合并首选项](/help/assets/icons/Merge.svg) [!BADGE 测试版]。

1. 在&#x200B;**[!UICONTROL Data merge preferences]** [!BADGE 测试版]{type=Informative}对话框中：

   ![数据合并首选项](/help/assets/data-merge-preferences.png)

   * 选择&#x200B;**[!UICONTROL Default metric preference]**。 在协调期间，如果多个数据源更新了给定渠道的量度字段，则会应用选定的默认量度首选项。 首选项应用于沙盒级别，除非针对基于特定量度的首选项被覆盖。 您可以选择介于&#x200B;**[!UICONTROL Summary data]**、**[!UICONTROL Event data]**&#x200B;和&#x200B;**[!UICONTROL Sum of summary and event data]**&#x200B;之间。

   * 要添加基于特定量度的首选项，请执行以下操作：

      1. 选择![加](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a metric]**。
         1. 从&#x200B;**[!UICONTROL *量度选择&#x200B;*]**列表中选择一个量度。
         1. 选择&#x200B;**[!UICONTROL CHANNELS]**&#x200B;或&#x200B;**[!UICONTROL CONVERSION TYPES]**。 从列表中选择&#x200B;**[!UICONTROL All]**&#x200B;或特定的渠道或转化类型。
         1. 选择&#x200B;**[!UICONTROL Summary]**&#x200B;或&#x200B;**[!UICONTROL Event]**&#x200B;以指定在合并数据时汇总数据或事件数据是否优先于量度（以及所有或选定的渠道）。

         要添加一个或多个其他渠道或转化类型，请执行以下操作：

         1. 选择![加号](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a channel]**&#x200B;或![加号](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a conversion type]**。
         1. 选择 **[!UICONTROL Summary]** 或 **[!UICONTROL Event]**。

         要删除渠道或转换类型，请选择![交叉](/help/assets/icons/Close.svg)。

      1. 要添加基于首选项的更具体的量度，请重复上一步骤。

   * 要删除基于现有的特定量度的首选项，请选择![删除](/help/assets/icons/Delete.svg)。

1. 选择&#x200B;**[!UICONTROL Save]**&#x200B;以保存数据合并首选项。 数据重新同步已启动。 <br/>选择要取消的&#x200B;**[!UICONTROL Cancel]**。

## 删除源数据集

当您删除协调数据中使用的源数据集时，该源数据集上的基础条目将从[[!UICONTROL Harmonized data]](/help/harmonize-data/overview.md)中删除。 但是，已删除源数据集的数据集规则仍保留在数据集规则配置列表中，其图标为![DataRemove](/help/assets/icons/DataRemove.svg)，表示已删除源数据集。 要获取更多详细信息，请执行以下操作：

* 从上下文菜单中选择![更多](/help/assets/icons/More.svg)和![预览](/help/assets/icons/Preview.svg) **[!UICONTROL View]**。
**[!UICONTROL Dataset rule mapping - Fields]**&#x200B;对话框显示有关已删除的源数据集的信息以及数据集规则配置中使用的字段。

当您返回&#x200B;**[!UICONTROL Dataset rules]**&#x200B;配置时，您会看到一个对话框，说明一个或多个源数据集已删除。 协调后的数据会在下一次临时或计划同步时受到影响。 查看数据集规则配置。

在下次特定同步或计划同步时，在不删除源数据的情况下更新协调数据。 但是，您仍会看到警告对话框，提示您根据已删除的源数据集删除数据集规则。 此警报允许用户查看和评估已删除数据集中受影响的字段。 并确定对在任何模型中可能使用的营销接触点或转化的影响。 查看并减轻此影响后，您应该从数据集规则配置列表中删除数据集规则。
