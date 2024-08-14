---
title: 访问控制
description: 了解如何在Mix Modeler中配置访问控制。
feature: Administration
source-git-commit: 6776a91563f120db1341adef923aab4b0f582c9d
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 1%

---

# 访问控制

Mix Modeler的访问控制是通过[Adobe Admin Console](https://adminconsole.adobe.com/)中的Experience Platform以及Experience Platform中的[权限](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home#platform-permissions)提供的。 此功能利用Admin Console中的产品配置文件，它将用户与权限和沙盒关联起来。

有关访问控制的详细信息，请参阅[访问控制概述](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home)。

## 基于角色的访问控制

请参阅[管理](../main-guide/administration.md)，了解如何为Experience Platform中的Mix Modeler用户和用户组配置基于角色的访问权限。

## 基于属性的访问控制

[基于属性的访问控制](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview)是一种Experience Platform功能，它使管理员能够根据属性控制对特定对象和/或功能的访问。 属性可以是添加到对象的元数据，例如添加到架构字段或区段的标签。 管理员定义包括管理用户访问权限的属性的访问策略。

此功能允许您使用定义组织或数据使用范围的标签来标记Experience Data Model (XDM)架构字段。 同时，管理员可以使用用户和角色管理界面定义XDM架构字段上的访问策略。 并更好地管理授予用户或用户组（内部、外部或第三方用户）的访问权限。 此外，基于属性的访问控制允许管理员管理对特定区段的访问。

通过基于属性的访问控制，管理员可以控制用户对所有平台工作流和资源的敏感个人数据(SPD)和个人身份信息(PII)的访问。 管理员可以定义仅有权访问特定字段以及与这些字段对应的数据的用户角色。

为协调的数据集配置数据集规则时，在字段级别强制实施Experience Platform的[基于属性的访问控制](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview)。 将标签附加到架构字段时，字段受限。 并且启用了拒绝您访问该字段的活动策略。 因此：

* 在创建数据集规则时，您看不到为您限制的架构字段，
* 您无法查看或编辑受限制的一个或多个架构字段的映射。 在编辑或查看包含此类受限字段的数据集规则时，您会看到以下屏幕。
  ![不允许执行操作](/help/assets//action-not-permitted.png)

