---
title: 数据集规则
description: 了解如何在Adobe组合建模器中定义要用作协调数据一部分的数据集规则。
feature: Harmonized Data, Dataset Rules
source-git-commit: ac17f5a9fcf036c8e689879578e4b745b789cea3
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---


# 数据集规则

数据集规则可帮助您将协调的字段与您在Adobe组合建模器中摄取的数据中的字段进行映射。

* 对于在Adobe Experience Platform中摄取的聚合数据，可将一个或多个可用数据集字段映射到相应的协调字段。
* 对于事件数据，您可以直接或使用条件将一个或多个协调的字段单独映射到数据集中的字段。


## 管理数据集规则和映射

要查看可用数据集映射的表，请在Adobe组合建模器界面中：

1. 选择 ![数据搜索](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** 从左边栏开始。

1. 选择 **[!UICONTROL Dataset rules]** 从顶部栏中。 您会看到数据集映射的表。

表列指定有关数据集映射的详细信息：

| 列名称 | 详细信息 |
| ---------------------- | ----------|
| 数据集 | 数据集的名称。 |
| 来源 | 数据集的源，可以是Adobe Analytics、体验事件、摘要（汇总）或使用者体验事件。 |
| 架构 | 数据集符合的架构。 您可以快速选择架构名称以在“Adobe混合建模器 — 架构”的架构编辑器的新选项卡中打开架构。 |
| 粒度 | 数据集中的数据粒度。 可能的值包括“每日”、“每周”、“每月”或“每年”。 |
| 一周开始 | 指定将一周中的哪一天视为特定数据集的新周的开始。 |
| 上次修改时间 | 上次修改数据集映射的数据和时间。 |

{style="table-layout:auto"}

### 创建数据集映射

要创建数据集映射，请在 ![数据搜索](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** Adobe混合建模器中的界面，选择 **[!UICONTROL Create Dataset Mapping]**.

在 **[!UICONTROL Create]** 屏幕，

1. 在 **[!UICONTROL Dataset Details]**，从中选择数据集 **[!UICONTROL Select dataset]** 以开始配置。

1. 选择日期 **[!UICONTROL Start of the week]**.

1. 选择 **[!UICONTROL Daily]**， **[!UICONTROL Weekly]**， **[!UICONTROL Monthly]** 或 **[!UICONTROL Yearly]** 对象 **[!UICONTROL Granularity]**.

1. 当您选择了 **[!UICONTROL Summary]** 数据集类型：

   1. 映射每个 **[!UICONTROL Available dataset fields]** 到对应的 **[!UICONTROL Standard harmonized fields]**. 如果不想将数据集字段映射到协调字段，请明确选择 **[!UICONTROL -- None --]**.

   1. 如果您需要新的协调字段，但无法从列表中获得，请选择 **[!UICONTROL Create New]** 创建新的协调字段。 您会看到中概述的对话框 [添加新的协调字段](fields.md#add-a-harmonized-field) 以快速添加新的协调字段。

   1. 完成所有字段的映射后，选择 **[!UICONTROL Save]**. 选择 **[!UICONTROL Cancel]** 以取消映射。

      ![创建数据集规则](../assets/dataset-create-summary.png)

1. 选择事件类型的数据集后，位于下面的阴影框中 **[!UICONTROL Map to harmonized fields]**：

   1. 从中选择协调字段 **[!UICONTROL Standard harmonized field]**.

   1. 当所选协调字段为指标类型时：

      1. 选择 **[!UICONTROL Count]** 或 **[!UICONTROL Sum]** 从 **[!UICONTROL Mapping type]**.

      1. 选择 **[!UICONTROL *AEP数据集字段&#x200B;*]**您希望协调字段默认映射到的字段。

   1. 当所选字段属于维度类型时：

      1. 选择 **[!UICONTROL Map Into]** 或 **[!UICONTROL Case]** 从 **[!UICONTROL Mapping type]**.

      1. 当您选择后 **[!UICONTROL Map Into]**，选择 **[!UICONTROL Field]** 和 **[!UICONTROL *AEP数据集字段&#x200B;*]**或&#x200B;**[!UICONTROL Value]**和默认值，默认将协调字段映射到数据集字段或输入值。

      1. 当您选择 **[!UICONTROL Case]**，选择 **[!UICONTROL Field]** 和 **[!UICONTROL *AEP数据集字段&#x200B;*]**或&#x200B;**[!UICONTROL Value]**和默认值，默认将协调字段映射到数据集字段或输入值。

         1. 此外，您还可以定义一个或多个情况，其中包含一个或多个条件以显式设置值。 每个条件都可以检查特定的 **[!UICONTROL *AEP数据集字段&#x200B;*]**是否&#x200B;**[!UICONTROL Exists]**或&#x200B;**[!UICONTROL Not Exists]**还是说&#x200B;**[!UICONTROL Contains]**，**[!UICONTROL Not Contains]**，**[!UICONTROL Equals]**，**[!UICONTROL Not Equals]**，**[!UICONTROL Starts With]**，或&#x200B;**[!UICONTROL Ends With]**输入的值**[!UICONTROL *&#x200B;输入输入值&#x200B;*]**.

         1. 要添加其他案例，请选择 ![添加](../assets/icons/AddCircle.svg) **[!UICONTROL Add case]**，要添加其他条件，请选择 ![添加](../assets/icons/AddCircle.svg) **[!UICONTROL Add condition]**.

         1. 要删除案例或条件，请选择 ![关闭](../assets/icons/Close.svg) 在相应的容器中。

         1. 要选择是应该将任何条件还是所有条件应用于案例，请选择 **[!UICONTROL Any of]** 或 **[!UICONTROL All of]**.

         1. 要设置案例的结果值，请在以下位置输入值 **[!UICONTROL Then]**.

      以下示例

      * 使用 **[!UICONTROL Map Into]** **[!UICONTROL Mapping type]** 以映射 **[!UICONTROL Channel Type At Source]** 将字段统一到 **[!UICONTROL channel_type]** 中的字段 **[!DNL Luma Transactions]** 数据集。

      * 使用 **[!UICONTROL Case]** **[!UICONTROL Mapping]** 键入以有条件地映射 **[!UICONTROL marketing.campaignName]** 中的字段 **[!DNL Luma Transactions]** 数据集到 **[!UICONTROL Campaign]** 协调字段。 Campaign协调字段设置为：

         * `Black Friday` 当 **[!UICONTROL marketing.campaignName]** 是 `_black_friday` 或 `BlackFriday`.
         * 至的值 **[!UICONTROL marketing.campaignName]** 在所有其他情况下。

        ![数据集规则事件](../assets/dataset-create-event.png)

1. 选择 ![添加](../assets/icons/AddCircle.svg) **[!UICONTROL Add field]** 以定义附加字段。

完成后，选择 **[!UICONTROL Save]** 以保存映射，或选择 **[!UICONTROL Cancel]** 以取消映射。


### 编辑数据集映射

要编辑数据集映射，请在 ![数据搜索](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** Adobe组合建模器中的接口：

1. 选择 ![更多](../assets/icons/More.svg) 在 **[!UICONTROL Dataset]** 要编辑的数据集映射的列。
1. 从上下文菜单中，选择 ![编辑](../assets/icons/Edit.svg) **[!UICONTROL Edit]** 以开始编辑数据集映射。 请参阅 [创建数据集映射](#create-a-dataset-mapping) 以了解更多详细信息。


### 删除数据集映射

要删除数据集映射，请在 ![数据搜索](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** Adobe组合建模器中的接口：

1. 选择 ![更多](../assets/icons/More.svg) 在 **[!UICONTROL Dataset]** 要删除的数据集映射的列。
1. 从上下文菜单中，选择 ![删除](../assets/icons/Delete.svg) **[!UICONTROL Delete]** 以删除数据集映射。


## 同步数据

要在协调的数据与汇总数据集和/或事件数据集之间同步数据，请遵循数据集规则中的所有逻辑：

1. 选择 **[!UICONTROL Sync data]**。

1. 从 **[!UICONTROL Sync data for dataset rules]** 对话框，请选择 **[!UICONTROL Refresh harmonized data for summary datasets]**， **[!UICONTROL Refresh harmonized data for event datasets]**，或 **[!UICONTROL Refresh harmonized data for both summary + event datasets]**.

1. 选择 **[!UICONTROL Sync]** 根据定义的数据集规则在数据集中协调的数据和数据之间开始同步。 要取消同步，请选择 **[!UICONTROL Cancel]**.

   ![同步数据](../assets/sync-data.png)

