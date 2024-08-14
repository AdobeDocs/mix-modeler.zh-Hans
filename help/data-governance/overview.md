---
title: 数据管理
description: 了解如何使用Experience Platform中的服务和工具，以便您控制收集的体验数据。 这样，您就可以遵守业务实践、法律义务和发展过程。
feature: Administration
source-git-commit: 6776a91563f120db1341adef923aab4b0f582c9d
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 2%

---

# 数据管理

Mix Modeler与Experience Platform之间的集成为Mix Modeler提供了利用Experience Platform的内在数据管理功能的功能。 文档的此部分详细介绍Mix Modeler中可用的数据管理功能。

Experience Platform数据管理使您能够控制和理解数据通过Experience Platform所经历的整个历程。 此历程涉及维护数据质量、数据谱系、数据编目等。

根据需要，在Mix Modeler中的Experience Platform表面使用的数据集上创建的数据使用标签和策略。 例如，在删除作为协调数据中的数据集规则一部分的数据集时，这些标签会阻止或警告用户。 或者隐藏在创建数据集规则时为用户限制的架构字段。

通过数据管理集成，您可以更高效地管理法规遵从性。 组织中的数据管理员可以设置策略来限制使用。 因此，您可以使用符合数据管理员定义的策略的数据。 阅读有关[标签和策略](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-dataviews/data-governance)的文档以了解更多信息。

以下数据治理功能可用：

| 功能 | 详细信息 |
|---|---|
| 访问控制 | 支持基于角色的访问控制和基于属性（字段级）的访问控制。 有关详细信息，请参阅[访问控制](access-controls.md)。 |
| 审核日志 | 当用户创建、更新或删除特定Mix Modeler类别时，Experience Platform审核功能会在审核日志中记录该活动。 有关详细信息，请参阅[审核日志](audit-logs.md)。 |
| 支持 | 作为统一数据工作流程的一部分，Experience Platform定义的政策将得到执行。 任何违反数据使用标签的情况都会报告并显示给用户。 有关详细信息，请参阅[策略](policies.md)。 |
| 加密 | 所有用于模型输入和输出的数据集都遵循Experience Platform准则。 Experience Platform数据加密适用于静止数据和传输中的数据。 |
| 数据卫生 | 所有用于模型输入和模型外的数据集均遵循Experience Platform准则。 Experience Platform提供了一套用于管理客户数据生命周期的工具，包括支持各种类型的数据过期。 当您从Experience Platform中删除源数据集（用作协调数据的一部分）时，系统会通知您。 有关详细信息，请参阅[数据集规则](/help/harmonize-data/dataset-rules.md)。 |
| 客户托管密钥 | 当您具有Privacy Security Shield或Healthcare Shield加载项的许可Mix Modeler时，您可以使用客户管理的密钥功能来利用Azure密钥库，通过API自带密钥。 您可以完全管理Mix Modeler中模型内正在处理的数据。 |
