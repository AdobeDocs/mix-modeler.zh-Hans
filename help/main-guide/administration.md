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

使用[Adobe Admin Console](https://helpx.adobe.com/cn/enterprise/using/admin-console.html)管理Mix Modeler产品和用户。

要使Mix Modeler正常运行，您必须设置正确的权限。

在Adobe Experience Cloud UI中：

1. 从左边栏中选择&#x200B;**[!UICONTROL ADMINISTRATION]**&#x200B;下的&#x200B;**[!UICONTROL Permissions]**。

1. 从左侧面板中选择![用户](/help/assets/icons/User.svg) **[!UICONTROL Roles]**。

1. 选择现有角色，或使用&#x200B;**[!UICONTROL Create role]**&#x200B;创建角色(例如，**Mix Modeler**)。 如果选择现有角色，请选择![编辑](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]**&#x200B;以编辑该角色的权限。 有关详细信息，请参阅[管理角色](https://helpx.adobe.com/cn/enterprise/using/admin-console.html)。

1. 确保您为角色选择了一个或多个沙箱。

1. 将&#x200B;**Adobe Mix Modeler**&#x200B;资源添加到该角色的资源列表中。

1. 请确保为您配置的角色选择正确的&#x200B;**[!UICONTROL Adobe Mix Modeler]**&#x200B;权限。 您可以选择以下一个或多个角色：

   - **[!UICONTROL View Adobe Mix Modeler Harmonized Data]**
   - **[!UICONTROL Manage Adobe Mix Modeler Harmonized Data]**
   - **[!UICONTROL View Adobe Mix Modeler Models Configuration]**
   - **[!UICONTROL Manage Adobe Mix Modeler Models Configuration]**
   - **[!UICONTROL View Adobe Mix Modeler Plans Configuration]**
   - **[!UICONTROL Manage Adobe Mix Modeler Plans Configuration]**

     ![Mix Modeler的RBAC](/help/assets/mix-modeler-rbac.png)


1. 请确保为该角色选择其他权限。 例如，要查看或管理数据集和架构，您可以选择：

   - **[!UICONTROL Data Management]**：选择相关选项： **[!UICONTROL View Datasets]**&#x200B;或&#x200B;**[!UICONTROL Manage Datasets]**。

   - **[!UICONTROL Data Modeling]**：选择相关选项： **[!UICONTROL Manage Schemas]**&#x200B;或&#x200B;**[!UICONTROL View Schemas]**。

   <!--
    * **[!UICONTROL Data Governance]**: ensure you select **[!UICONTROL View User Activity Log]** and **[!UICONTROL View Data Usage Policies]**.
    -->

   <!--![Permissions](assets/permissions-including-privacy.png)-->

   选择&#x200B;**[!UICONTROL Save]**&#x200B;以保存权限。

1. 在&#x200B;**[!UICONTROL Role]**&#x200B;内的&#x200B;**[!UICONTROL Details]**&#x200B;中，添加相应的&#x200B;**[!UICONTROL Users]**&#x200B;或&#x200B;**[!UICONTROL User groups]**&#x200B;以提供用户访问Mix Modeler的权限。
