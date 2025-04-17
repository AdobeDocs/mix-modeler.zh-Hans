---
title: 审核日志
description: 了解如何从Mix Modeler访问审核日志。
feature: Administration
exl-id: aa65aac5-bea4-43ff-b0d0-9e8a6a97d3ca
source-git-commit: 85f9b42a775006cd3566447b2bb9d0a806fa3e73
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 5%

---

# 审核日志

为了提高系统中执行活动的透明度和可见性，Mix Modeler审核日志会捕获Experience Platform工作流中的用户活动，以了解对Mix Modeler类别进行的任何用户驱动更改。 这些日志形成审核记录，可以帮助解决问题，并帮助您的企业有效地遵守公司数据管理政策和法规要求。

<!-- DO WE HAVE TO ADD THIS
If you are subject to the Health Insurance Portability and Accountability Act (HIPAA) and create, receive, maintain, or transmit permitted sensitive personal data through Mix Modeler, you are responsible for executing a BAA with Adobe and licensing Healthcare Shield.
-->

审核日志会告知执行了什么操作以及何时执行。 日志中记录的每个操作都包含元数据，这些元数据指示操作类型、日期和时间、执行操作的用户的电子邮件ID以及与操作类型相关的其他属性。 它跟踪用户在Mix Modeler中执行的创建、更新和删除操作。

要在Mix Modeler界面中检查审核日志，请执行以下操作：

1. 从&#x200B;**[!UICONTROL PRIVACY]**&#x200B;中选择![任务列表](/help/assets/icons/TaskList.svg) **[!UICONTROL Audits]**。

1. 在&#x200B;**[!UICONTROL Audits]**&#x200B;中，您可以找到&#x200B;**[!UICONTROL Activity log]**。 活动日志显示以下Mix Modeler类别、操作和状态的条目。

   | 类别 | 操作 | 状态 |
   |---|---|---|
   | Mix Modeler数据集规则 | 创建 | 允许或拒绝 |
   | Mix Modeler数据集规则 | 更新 | 允许或拒绝 |
   | Mix Modeler数据集规则 | Delete | 允许或拒绝 |
   | Mix Modeler字段 | 创建 | 允许或拒绝 |
   | Mix Modeler字段 | 更新 | 允许或拒绝 |
   | Mix Modeler字段 | Delete | 允许或拒绝 |
   | Mix Modeler营销接触点 | 创建 | 允许或拒绝 |
   | Mix Modeler营销接触点 | 更新 | 允许或拒绝 |
   | Mix Modeler营销接触点 | Delete | 允许或拒绝 |
   | Mix Modeler转换 | 创建 | 允许或拒绝 |
   | Mix Modeler转换 | 更新 | 允许或拒绝 |
   | Mix Modeler转换 | Delete | 允许或拒绝 |
   | Mix Modeler模型 | 创建 | 允许或拒绝 |
   | Mix Modeler模型 | 更新 | 允许或拒绝 |
   | Mix Modeler模型 | Delete | 允许或拒绝 |
   | Mix Modeler模型 | Rescore | 允许或拒绝 |
   | Mix Modeler模型 | 克隆 | 允许或拒绝 |
   | Mix Modeler模型 | 培训/重新培训 | 允许或拒绝 |
   | Mix Modeler模型 | 下载/保存元数据 | 允许或拒绝 |
   | Mix Modeler计划 | 创建 | 允许或拒绝 |
   | Mix Modeler计划 | 更新 | 允许或拒绝 |
   | Mix Modeler计划 | 更改关联的模型 | 允许或拒绝 |
   | Mix Modeler数据协调 | 触发器同步 | 允许或拒绝 |


1. 在活动日志中选择一个条目，以打开面板了解更多详细信息。

   ![Mix Modeler审核](/help/assets/mix-modeler-audit.png)

1. 要筛选&#x200B;**[!UICONTROL Category]**、**[!UICONTROL Action]**、**[!UICONTROL Request ID]**、**[!UICONTROL User]**、**[!UICONTROL Status]**&#x200B;或&#x200B;**[!UICONTROL Date]**&#x200B;范围，请选择![筛选器](/help/assets/icons/Filter.svg)。

1. 要修改活动日志中显示的列，请选择![列](/help/assets/icons/ColumnSetting.svg)，然后在&#x200B;**[!UICONTROL Customize table]**&#x200B;对话框中选择要显示的列。 选择&#x200B;**[!UICONTROL Apply]**&#x200B;以应用选择，**[!UICONTROL Cancel]**&#x200B;以取消选择。

1. 要下载审核日志，请选择![下载](/help/assets/icons/Download.svg) **[!UICONTROL Download log]**。 在&#x200B;**[!UICONTROL Download log]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL CSV]**&#x200B;或&#x200B;**[!UICONTROL JSON]**&#x200B;作为格式并选择&#x200B;**[!UICONTROL Download]**。

## 访问审核日志

为您的组织启用该功能后，系统会在活动发生时自动收集审核日志。 您无需手动启用审核日志收集。

要查看和导出审核日志，您必须已被授予审核日志访问访问控制权限。 要了解如何管理Mix Modeler功能的各个权限，请参阅[访问控制文档](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home)。
