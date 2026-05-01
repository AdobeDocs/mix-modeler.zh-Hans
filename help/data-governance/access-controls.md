---
title: 访问控制
description: 了解如何在Mix Modeler中配置访问控制。
feature: Administration
exl-id: c9ec97d9-b9a2-41f5-8626-1cf967d5d7fe
TQID: https://experienceleague.adobe.com/EoiF5ui2Bqq0Oxuv-s5E5pQclj9gnjoKgZ1bOzRK-vY
product_v2: id: b88c80e3-31df-4609-989d-d4dac0e6d973
feature_v2: id: fe2edbb1-46f9-4347-a27c-577cab3640cb
subfeature_v2: id: abe9e290-7d2f-4131-b71e-ef9900865044
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
autotag-review: '2026-05-01T09:20:37.287Z'
source-git-commit: 5579087b9381c4d8e909ed5fe3099fd42d5c6799
workflow-type: tm+mt
source-wordcount: 412
ht-degree: 1%

---

# 访问控制

Mix Modeler的访问控制是通过[Adobe Admin Console](https://adminconsole.adobe.com/)中的Experience Platform以及Experience Platform中的[权限](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home#platform-permissions)提供的。 此功能利用Admin Console中的产品配置文件，它将用户与权限和沙盒关联起来。

有关访问控制的详细信息，请参阅[访问控制概述](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home)。

## 基于角色的访问控制

有关如何在Experience Platform中为Mix Modeler用户和用户组配置基于角色的访问权限，请参阅[管理](../main-guide/administration.md)。

## 基于属性的访问控制

[基于属性的访问控制](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview)是Experience Platform的一项功能，它使管理员能够根据属性控制对特定对象和/或功能的访问。 属性可以是添加到对象的元数据，例如添加到架构字段或区段的标签。 管理员定义包括管理用户访问权限的属性的访问策略。

此功能允许您使用定义组织或数据使用范围的标签来标记Experience Data Model (XDM)架构字段。 同时，管理员可以使用用户和角色管理界面定义XDM架构字段上的访问策略。 并更好地管理授予用户或用户组（内部、外部或第三方用户）的访问权限。 此外，基于属性的访问控制允许管理员管理对特定区段的访问。

通过基于属性的访问控制，管理员可以控制用户对所有平台工作流和资源的敏感个人数据(SPD)和个人身份信息(PII)的访问。 管理员可以定义仅有权访问特定字段以及与这些字段对应的数据的用户角色。

为协调的数据集配置数据集规则时，在字段级别强制实施Experience Platform基于[属性的访问控制](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview)。 将标签附加到架构字段时，字段受限。 并且启用了拒绝您访问该字段的活动策略。 因此：

* 在创建数据集规则时，您看不到为您限制的架构字段，
* 您无法查看或编辑受限制的一个或多个架构字段的映射。 在编辑或查看包含此类受限字段的数据集规则时，您会看到以下屏幕。
  ![不允许执行操作](/help/assets/action-not-permitted.png)
