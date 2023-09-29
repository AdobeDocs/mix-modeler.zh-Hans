---
title: 比较计划
description: 了解如何在Adobe组合建模器中比较计划。
source-git-commit: 1eaebc6f6178270a9e8aebb6b250e0b0a6289f52
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 7%

---


# 管理

使用 [Adobe Admin Console](https://helpx.adobe.com/cn/enterprise/using/admin-console.html) 管理Adobe Mix Modeler产品和用户。

要使Adobe Mix Modeler正常运行，您必须设置正确的权限。

在Adobe Experience Cloud UI中，

1. 选择 **[!UICONTROL Permissions]** 从左边栏的下面 **[!UICONTROL ADMINISTRATION]**.

1. 选择 ![人员](assets/icons/User.svg) **[!UICONTROL Roles]** 从左侧面板。

1. 选择现有角色，或使用以下方式创建角色 **[!UICONTROL Create role]**. 如果您选择了现有角色，请选择 ![编辑](assets/icons/Edit.svg) **[!UICONTROL Edit]** 编辑角色的权限。 请参阅 [管理角色](https://helpx.adobe.com/cn/enterprise/using/admin-console.html) 以了解更多信息。

1. 请确保为角色选择以下权限：

   * **[!UICONTROL Sandboxes]**：至少选择一个沙盒。

   * **[!UICONTROL Data Management]**：确保选择相应的选项 **[!UICONTROL View Datasets]** 和 **[!UICONTROL Manage Datasets]**.

   * **[!UICONTROL Data Modeling]**：确保选择相应的选项 **[!UICONTROL Manage Schemas]** 和 **[!UICONTROL View Schemas]**.

   * **[!UICONTROL Destinations]**：确保选择 **[!UICONTROL Manage and Activate Dataset Destination]**， **[!UICONTROL Destination Authoring]**， **[!UICONTROL Activate Destinations]** 和 **[!UICONTROL View Destinations]**.

   * **[!UICONTROL Data Ingestion]**：确保选择 **[!UICONTROL View Sources]** 和 **[!UICONTROL Manage Sources]**.

   为角色设置的权限应该如下所示：

   ![Permissions](assets/permissions.png)

   选择 **[!UICONTROL Save]** 以保存权限。

1. 在 **[!UICONTROL Details]** 范围 **[!UICONTROL Role]**，添加相应的 **[!UICONTROL Users]** 和/或 **[!UICONTROL User groups]** 向用户提供访问Adobe Mix Modeler的权限。
