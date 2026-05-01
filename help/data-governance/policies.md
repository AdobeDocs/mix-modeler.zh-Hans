---
title: 支持
description: 了解如何从Mix Modeler访问策略。
feature: Administration
exl-id: 4dba7c30-ad1e-4213-a2b0-afc55f2448a3
TQID: https://experienceleague.adobe.com/fk6qAZS7Uymx2dzptcazBieXIJ3mGF2pjG-EDhm-Kh4
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
feature_v2:
  - id: f6633d1c-3d2d-4f48-95d4-4bbc9913db52
subfeature_v2:
  - id: fd80ec6b-9b9e-448a-a6d0-b0c9a15da6b8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
autotag-review: '2026-05-01T09:17:02.907Z'
source-git-commit: 5579087b9381c4d8e909ed5fe3099fd42d5c6799
workflow-type: tm+mt
source-wordcount: 507
ht-degree: 2%

---

# 支持

完成工作流创建模型并提交模型的配置后，[策略实施](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/enforcement/overview#automatic-enforcement)将检查是否存在任何违规。 如果发生策略冲突，则会出现一个弹出窗口，指示已违反一个或多个策略。 此检查旨在确保Experience Platform中的数据操作和营销操作符合数据使用策略。

默认情况下，Mix Modeler会检查是否存在与Adobe定义的与以下标签和营销操作关联的策略违规：

| 策略名称 | 关联的标签 | 关联的营销操作 |
|---|---|---|
| 限制使用分析和基于用户的测量 | C8 | Analytics |
| 限制数据科学 | C9 | 数据科学 |
| 限制数据导出 | C12 | 数据导出 |

对于您自己定义的策略以及包含上表中列出的任何营销操作的策略，也会检查违规。

在构建数据集规则时违反策略时，您会看到一个弹出窗口，其中显示有关策略违规的信息。

例如：

- 您已启用具有关联标签[!UICONTROL C9]和关联营销操作[!UICONTROL Data Science]的[!UICONTROL Restrict data science]策略，
- 您已将[!UICONTROL C9] - [!UICONTROL No data science]标签应用于转化数据架构中的`totalCost`字段，
- 要设置数据集规则，以将“转换数据”架构的`totalCost`字段映射到名为`spend`（且显示名称为`Spend`）的协调字段。

当要保存数据集规则时，您会看到&#x200B;**[!UICONTROL Data governance policy violation detected]**&#x200B;弹出窗口，其中显示违反的策略列表。 当您选择策略名称时，在[!UICONTROL Violation summary]中，您会看到[!UICONTROL Active data governance labels]的列表，其中包含应用的[!UICONTROL Entity]、[!UICONTROL Type]、[!UICONTROL Field]和[!UICONTROL Government labels]。

<!-- pending screenshot -->

将数据使用标签应用于已用于协调数据的架构字段时，您会看到一个弹出窗口，其中显示有关策略违规的信息。

例如：

- 您已设置数据集规则，其中将转换数据架构的`totalCost`字段映射到名为`spend`（且显示名称为`Spend`）的协调字段。
- 您至少已成功地同步一次协调数据（请参阅[数据集规则 — 同步数据](/help/harmonize-data/dataset-rules.md#sync-data)）。
- 您启用了具有关联的标签[!UICONTROL C9]和关联的营销操作[!UICONTROL Data Science]的[!UICONTROL Restrict data science]策略，
- 要将[!UICONTROL C9] - [!UICONTROL No data science]标签应用于转化数据架构中的`totalCost`字段。

当要保存架构更新时，您会看到&#x200B;**[!UICONTROL Data governance policy violation detected]**&#x200B;弹出窗口，其中显示违反的策略列表。 选择[!UICONTROL Violation summary]中的策略名称以在[!UICONTROL Data Lineage]列表中查找更多详细信息。

<!-- pending screenshot -->

## 检测到违规的弹出框

检测到的数据治理策略违规弹出框提供有关该违规的特定信息。 您可以通过策略设置和其他与配置工作流不直接相关的度量来解决这些违规。 例如，您可以更改标签，以便允许某些字段用于数据科学目的。 或者，也可以修改模型配置本身，使模型不使用带有数据使用标签的对象。

左边栏中的![隐私](/help/assets/icons/Privacy.svg) **[!UICONTROL Policies]**&#x200B;选项提供对Experience Platform的[!UICONTROL Policies]界面的访问权限，这将允许管理您的策略、标签和营销操作。

<!--
Currently,  Mix Modeler does not support all of the data governance functionality offered by Experience Platform. Field level access control is supported. See [Field level access control](../harmonize-data/dataset-rules.md#field-level-access-control)
-->

>[!MORELIKETHIS]
>
>[数据使用策略概述](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/policies/overview)
>
>

