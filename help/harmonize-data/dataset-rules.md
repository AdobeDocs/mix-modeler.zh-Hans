---
title: 数据集规则
description: 了解如何定义要用作协调Mix Modeler中数据一部分的数据集规则。
feature: Harmonized Data, Dataset Rules
exl-id: 57d7940a-2900-4814-a30d-bb02bff7615d
source-git-commit: a066cdff03eade86b09f03209a08ebfa2ab32e8e
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 0%

---

# 数据集规则

数据集规则可帮助您将协调的字段与您在Mix Modeler中引入的数据中的字段进行映射。

* 对于在Adobe Experience Platform中摄取的聚合数据，可将一个或多个可用数据集字段映射到相应的协调字段。
* 对于事件数据，您可以直接或使用条件将一个或多个协调的字段单独映射到数据集中的字段。


## 管理数据集规则

要查看可用数据集规则的表，请在Mix Modeler界面中：

1. 选择 ![数据搜索](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** 从左边栏开始。

1. 选择 **[!UICONTROL Dataset rules]** 从顶部栏中。 您会看到数据集规则的表。

表列指定有关数据集规则的详细信息：

| 列名称 | 详细信息 |
| ---------------------- | ----------|
| 数据集 | 数据集的名称。 |
| 来源 | 数据集的来源： Adobe Analytics、体验事件、摘要（汇总）或使用者体验事件。 |
| 架构 | 数据集符合的架构。 您可以快速选择架构名称，以在架构编辑器的新选项卡中打开架构。 ![架构](../assets/icons/Schemas.svg) [架构](../ingest-data/schemas.md). |
| 粒度 | 数据集中的数据粒度。 可能的值包括“每日”、“每周”、“每月”或“每年”。 |
| 一周开始 | 指定将一周中的哪一天视为特定数据集的新周的开始。 |
| 状态 | 字段的状态： <p><span style="color:gray">●</span> 草稿或 <p><span style="color:green">●</span> 活动 |
| 上次修改时间 | 上次修改数据集规则的数据和时间。 |

{style="table-layout:auto"}

### 创建数据集规则

要创建数据集规则，请在 ![数据搜索](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** 界面中，选择Mix Modeler **[!UICONTROL Create a dataset rule]** 在 **[!UICONTROL Dataset rules configuration]** 向导。

在 **[!UICONTROL Create]** 屏幕，

1. 在 **[!UICONTROL Dataset details]**，从中选择数据集 **[!UICONTROL Select dataset]** 以开始配置。 在列表中，数据集分类为 **[!UICONTROL Consumer Experience Events]**， **[!UICONTROL Adobe Analytics]**， **[!UICONTROL Experience Event]** 和， **[!UICONTROL Summary]**.

1. 选择日期 **[!UICONTROL Start of the week]**.

1. 选择 **[!UICONTROL Daily]**， **[!UICONTROL Weekly]**， **[!UICONTROL Monthly]** 或 **[!UICONTROL Yearly]** 对象 **[!UICONTROL Granularity]**.

1. 当您选择的数据集为 **[!UICONTROL Summary]** 类别：

   1. 要定义数据集的数据是聚合还是替换现有数据，请选择 **[!UICONTROL Aggregation]** 或 **[!UICONTROL Replacement]** 对象 **[!UICONTROL Data restatement is by]**.

   1. 映射每个 **[!UICONTROL Available dataset fields]** 到对应的 **[!UICONTROL Standard harmonized fields]** 在 **[!UICONTROL Map to harmonized fields]**. 如果不想将数据集字段映射到协调字段，请明确选择 **[!UICONTROL -- None --]**.

   1. 如果您需要新的协调字段，但无法从列表中获得，请选择 **[!UICONTROL Create New]** 创建新的协调字段。 您会看到中概述的对话框 [添加新的协调字段](fields.md#add-a-harmonized-field).

   1. 为规则的所有字段完成映射后，选择 **[!UICONTROL Save as draft]** 保存规则的草稿版本或 **[!UICONTROL Save]** 以保存并激活规则。 选择 **[!UICONTROL Cancel]** 以取消规则配置。

      ![创建数据集规则](../assets/dataset-create-summary.png)

1. 选择事件类别数据集后(**[!UICONTROL Experience Events]**， **[!UICONTROL Adobe Analytics]**， **[!UICONTROL Consumer Experience Events]**)，在下面的框中 **[!UICONTROL Map to harmonized fields]**：

   1. 从中选择协调字段 **[!UICONTROL Standard harmonized field]**.

   1. 当所选协调字段为指标类型时：

      1. 选择 **[!UICONTROL Count]** 或 **[!UICONTROL Sum]** 从 **[!UICONTROL Mapping type]**.

      1. 选择 **[!UICONTROL *AEP数据集字段&#x200B;*]**您希望协调字段默认映射到的字段。

   1. 当所选字段属于维度类型时：

      1. 选择 **[!UICONTROL Map Into]** 或 **[!UICONTROL Case]** 从 **[!UICONTROL Mapping type]**.

      1. 当您选择后 **[!UICONTROL Map Into]**，选择 **[!UICONTROL Field]** 和 **[!UICONTROL *AEP数据集字段&#x200B;*]**或&#x200B;**[!UICONTROL Value]**和默认值，默认将协调字段映射到数据集字段或输入值。

      1. 当您选择时 **[!UICONTROL Case]**，选择 **[!UICONTROL Field]** 和 **[!UICONTROL *AEP数据集字段&#x200B;*]**或&#x200B;**[!UICONTROL Value]**和默认值，默认将协调字段映射到数据集字段或输入值。

         1. 要显式设置值，可定义一个或多个情况，其中包含一个或多个条件。 每个条件都可以检查特定的 **[!UICONTROL *AEP数据集字段&#x200B;*]**是否&#x200B;**[!UICONTROL Exists]**或&#x200B;**[!UICONTROL Not Exists]**还是说&#x200B;**[!UICONTROL Contains]**，**[!UICONTROL Not Contains]**，**[!UICONTROL Equals]**，**[!UICONTROL Not Equals]**，**[!UICONTROL Starts With]**，或&#x200B;**[!UICONTROL Ends With]**输入的值**[!UICONTROL *&#x200B;输入输入值&#x200B;*]**.

         1. 要添加其他案例，请选择 ![添加](../assets/icons/AddCircle.svg) **[!UICONTROL Add case]**，要添加其他条件，请选择 ![添加](../assets/icons/AddCircle.svg) **[!UICONTROL Add condition]**.

         1. 要删除案例或条件，请选择 ![关闭](../assets/icons/Close.svg) 在相应的容器中。

         1. 要选择是应该将任何条件还是所有条件应用于案例，请选择 **[!UICONTROL Any of]** 或 **[!UICONTROL All of]**.

         1. 要设置案例的结果值，请在以下位置输入值 **[!UICONTROL Then]**.

      以下示例

      * 使用 **[!UICONTROL Map Into]** **[!UICONTROL Mapping type]** 以映射 **[!UICONTROL Channel Type At Source]** 将字段统一到 **[!UICONTROL channel_type]** 中的字段 **[!DNL Luma Transactions]** 数据集。

      * 使用 **[!UICONTROL Case]** **[!UICONTROL Mapping type]** 有条件地映射 **[!UICONTROL marketing.campaignName]** 中的字段 **[!DNL Luma Transactions]** 数据集到 **[!UICONTROL Campaign]** 协调字段。 Campaign协调字段设置为：

         * `Black Friday` 当 **[!UICONTROL marketing.campaignName]** 是 `_black_friday` 或 `BlackFriday`.
         * 至的值 **[!UICONTROL marketing.campaignName]** 在所有其他情况下。

        ![数据集规则事件](../assets/dataset-create-event.png)

1. 选择 ![添加](../assets/icons/AddCircle.svg) **[!UICONTROL Add field]** 以定义附加字段。

完成后，选择 **[!UICONTROL Save as draft]** 保存规则的草稿版本或 **[!UICONTROL Save]** 以保存并激活规则。 选择 **[!UICONTROL Cancel]** 以取消规则配置。


### 编辑数据集规则

要编辑数据集规则，请在 ![数据搜索](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** 界面Mix Modeler：

1. 选择 ![更多](../assets/icons/More.svg) 在 **[!UICONTROL Dataset]** 要编辑的数据集规则的列。
1. 从上下文菜单中，选择 ![编辑](../assets/icons/Edit.svg) **[!UICONTROL Edit]** 以开始编辑数据集规则。 请参阅 [创建数据集规则](#create-a-dataset-rule) 以了解更多详细信息。


### 删除数据集规则

要删除数据集规则，请在 ![数据搜索](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** 界面Mix Modeler：

1. 选择 ![更多](../assets/icons/More.svg) 在 **[!UICONTROL Dataset]** 要删除的数据集规则的列。
1. 从上下文菜单中，选择 ![删除](../assets/icons/Delete.svg) **[!UICONTROL Delete]** 以删除数据集规则。 系统会提示您进行确认。 选择 **[!UICONTROL Delete]** 以永久删除选定的数据集规则。


## 同步数据

要在协调的数据与汇总数据集和/或事件数据集之间同步数据，请遵循数据集规则中的所有逻辑：

1. 选择 **[!UICONTROL Sync data]**。

1. 从 **[!UICONTROL Sync data for dataset rules]** 对话框，请选择
   * **[!UICONTROL Refresh harmonized data for summary datasets]**，
   * **[!UICONTROL Refresh harmonized data for event datasets]**，或
   * **[!UICONTROL Refresh harmonized data for both summary + event datasets]**。

1. 要根据定义的数据集规则在数据集中的协调数据和数据之间启动同步，请选择 **[!UICONTROL Sync]**. 要取消同步，请选择 **[!UICONTROL Cancel]**.

   ![同步数据](../assets/sync-data.png)


## 数据合并首选项

>[!NOTE]
>
>[!BADGE beta]{type=Informative}

数据合并首选项有助于在合并来自汇总的数据和事件数据源的数据时解决冲突。 用例包括：

* 在多个数据集中测量和报告相同的广告量度，或
* 某些数据集中的量度测量可能不完整，而另一个数据集可能是特定量度的超集，从而导致重复计数。

要确保准确的模型预测，您可以定义数据合并首选项：

1. 选择 ![数据合并首选项](../assets/icons/Merge.svg) [!BADGE beta].

1. 在 **[!UICONTROL Data merge preferences]** [!BADGE beta]{type=Informative}

   ![数据合并首选项](../assets/data-merge-preferences.png)

   * 选择 **[!UICONTROL Default metric preference]**. 在协调期间，如果多个数据源更新了给定渠道的量度字段，则会应用选定的默认量度首选项。 首选项应用于沙盒级别，除非针对基于特定量度的首选项被覆盖。 您可以选择 **[!UICONTROL Summary data]**， **[!UICONTROL Event data]** 和 **[!UICONTROL Sum of summmary and event data]**.

   * 要添加基于特定量度的首选项，请执行以下操作：

      1. 选择 ![加号](../assets/icons/AddCircle.svg) **[!UICONTROL Add a metric]**.
         1. 从中选择一个量度 **[!UICONTROL *量度选择&#x200B;*]**列表。
         1. 选择 **[!UICONTROL CHANNELS]** 或 **[!UICONTROL CONVERSION TYPES]**. 从列表中，选择 **[!UICONTROL All]** 或特定渠道或转化类型。
         1. 选择 **[!UICONTROL Summary]** 或 **[!UICONTROL Event]** 指定在合并数据时是否首选度量使用摘要数据或事件数据（以及所有或所选渠道）。

         要添加一个或多个其他渠道或转化类型，请执行以下操作：

         1. 选择 ![加号](../assets/icons/AddCircle.svg) **[!UICONTROL Add a channel]** 或 ![加号](../assets/icons/AddCircle.svg) **[!UICONTROL Add a conversion type]**.
         1. 选择 **[!UICONTROL Summary]** 或 **[!UICONTROL Event]**。

         要删除渠道或转化类型，请选择 ![交叉](../assets/icons/Close.svg).

      1. 要添加基于首选项的更具体的量度，请重复上一步骤。

   * 要删除基于现有特定量度的首选项，请选择 ![删除](../assets/icons/Delete.svg).

1. 选择 **[!UICONTROL Save]** 以保存数据合并首选项。 数据重新同步已启动。 <br/>选择 **[!UICONTROL Cancel]** 以取消。


## 字段级访问控制

在为协调的数据集配置数据集规则时，Experience Platform [基于属性的访问控制](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview) 在字段级别强制实施。 当标签附加到架构字段并启用拒绝您访问该字段的活动策略时，字段会受到限制。 因此：

* 在创建数据集规则时，您看不到为您限制的架构字段，
* 您无法查看或编辑受限制的一个或多个架构字段的映射。 在编辑或查看包含此类受限字段的数据集规则时，您会看到以下屏幕。
  ![不允许操作](../assets/action-not-permitted.png)
