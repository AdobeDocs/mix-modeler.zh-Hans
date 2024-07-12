---
title: 管理
description: 了解如何管理Mix Modeler。
feature: Administration
exl-id: 76d6d15d-a838-4ee2-9929-e55ea8946b80
source-git-commit: 4d84c93121fc476cc6610ad572bab161bbacfc23
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 2%

---

# 管理

使用 [Adobe Admin Console](https://helpx.adobe.com/cn/enterprise/using/admin-console.html) 管理Mix Modeler产品和用户。

要使Mix Modeler正常运行，您必须设置正确的权限。

在Adobe Experience Cloud UI中：

1. 选择 **[!UICONTROL Permissions]** 从左边栏，下面 **[!UICONTROL ADMINISTRATION]**.

1. 选择 ![用户](/help/assets/icons/User.svg) **[!UICONTROL Roles]** 从左侧面板。

1. 选择现有角色，或使用以下方式创建角色 **[!UICONTROL Create role]** (例如， **Mix Modeler**)。 如果选择现有角色，请选择 ![编辑](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]** 编辑角色的权限。 请参阅 [管理角色](https://helpx.adobe.com/cn/enterprise/using/admin-console.html) 以了解更多信息。

1. 确保您为角色选择了一个或多个沙箱。

1. 添加 **Adobe Mix Modeler** 资源到角色的资源列表。

1. 确保您选择正确的 **[!UICONTROL Adobe Mix Modeler]** 您正在配置的角色的权限。 您可以选择以下一个或多个角色：

   - **[!UICONTROL View Adobe Mix Modeler Harmonized Data]**
   - **[!UICONTROL Manage Adobe Mix Modeler Harmonized Data]**
   - **[!UICONTROL View Adobe Mix Modeler Models Configuration]**
   - **[!UICONTROL Manage Adobe Mix Modeler Models Configuration]**
   - **[!UICONTROL View Adobe Mix Modeler Plans Configuration]**
   - **[!UICONTROL Manage Adobe Mix Modeler Plans Configuration]**

     ![MIX MODELERRBAC](/help/assets/mix-modeler-rbac.png)


1. 请确保为该角色选择其他权限。 例如，要查看或管理数据集和架构，您可以选择：

   - **[!UICONTROL Data Management]**：选择相关选项： **[!UICONTROL View Datasets]** 或 **[!UICONTROL Manage Datasets]**.

   - **[!UICONTROL Data Modeling]**：选择相关选项： **[!UICONTROL Manage Schemas]** 或 **[!UICONTROL View Schemas]**.

   <!--
    * **[!UICONTROL Data Governance]**: ensure you select **[!UICONTROL View User Activity Log]** and **[!UICONTROL View Data Usage Policies]**.
    -->

   <!--![Permissions](assets/permissions-including-privacy.png)-->

   选择 **[!UICONTROL Save]** 以保存权限。

1. 在 **[!UICONTROL Details]** 范围 **[!UICONTROL Role]**，添加相应的 **[!UICONTROL Users]** 或 **[!UICONTROL User groups]** 向用户提供访问Mix Modeler的权限。
