---
title: Mix Modeler用例
description: Mix Modeler用例。
feature: Schemas, Datasets, Conversions, Harmonized Data, Marketing Touch Points, Models, Plans
exl-id: cc82abec-d0ce-44bf-ad7e-fc379a394185
source-git-commit: 1a9df9f9819d9e0031e58443ec6a9e755a151ba0
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 3%

---

# Mix Modeler用例

Mix Modeler支持以下主要用例。

## 了解全渠道增量性能

此用例可帮助您衡量营销对所有付费、免费和自有渠道的影响。

+++ 详细信息

### 挑战

这些用例解决的挑战包括：

* 很难从孤立的客户历程数据、信号丢失和带围墙的花园中测量增量性能。
* 从MMM和MTA分开的方法得到的见解不一致，降低了对结果的信心。
* 对推动成功的营销渠道和策略的了解有限。

### 方针

此用例的基于步骤的方法是：

| 步骤 | 详细信息 |
|---|---|
| 摄取 | 识别数据源并将其摄取到常用架构下。 <br/>将Adobe Analytics或Customer Journey Analytics中的现有投资应用到快速通道部署。 |
| 配置 | 使用AI-as-a-Service框架为特定业务目标配置灵活的模型<br/>通过双向传输学习自动确保接触点和摘要级别之间的一致性。 |
| 分析 | 清楚地了解整体营销和单个渠道/子渠道的ROI。<br/>清楚地了解哪些接触点最能推动增量转化。 |

{style="table-layout:auto"}


### 影响

成功实施此使用可能会产生以下影响：

* 合并聚合数据、接触点数据和外部变量，以获得最佳的测量视图。
* 使用AI-as-a-Service解决方案快速创建模型，并通过访问模型透明度来提高置信度，从而推动成功。
* 通过在摘要级别和接触点级别的结果中保持一致，提高对战略和战术决策的信心。

+++


## 制定营销计划以优化ROI

此用例使用用户友好、支持AI的优化和方案规划工具来最大限度地提高ROI。

+++ 详细信息

### 挑战

这些用例解决的挑战包括：

* 根据效率曲线制定数据驱动型营销投资计划，而不依赖直觉。
* 同时实现跨多个地区、业务线和渠道的最大化结果。
* 创建并比较多个预算方案需要较长的迭代周期，且需要大量手动工作。


### 方针

此用例的基于步骤的方法是：

| 步骤 | 详细信息 |
|---|---|
| 配置 | 轻松根据业务目标自定义测量模型。<br/>单击几下即可定义参数，无需编码：例如渠道、地理位置、销售周期、滞后、内部和外部业务因素等。 |
| 训练 | 训练配置的AI/ML模型如何学习最适合输入数据的情况，从而提供最准确的结果。 |
| 优化 | 根据模型预测获取自动优化的预算分配。<br/>使用直观的UI，通过单击几下即可开发和比较多个预算方案。 |

{style="table-layout:auto"}


### 影响

成功实施此使用可能会产生以下影响：

* 创建营销投资计划，以实现多个目标和优先级之间投资回报的最大化。
* 使用递增的ROI曲线来确定转移预算的机会。
* 使用自助式民主化工具快速获取每月或每周预测。

+++

<!-- This use case is not supported with initial release

## Make data-driven inflight optimizations

This use case helps you to improve ROI weekly by assessing actual and forecasted performance to make inflight improvements.

+++ Details

### Challenges

The challenges this use case addresses are:

* Campaign performance is often slow, or lacks granularity need to confidently optimize.
* Messy, non-standardized data across dozens of channels and sources drives slow time to insight.
* No democratized access to tools and overreliance on select experts or external vendors, increasing turnaround times.



### Approach

The step based approach for this use case:

| Step | Details |
|---|---|
| Ingest | Ingest data in common schemas for easy model refreshes and reusability across Experience Platform applications.<br/>Streamline data piping, cleaning & QA with automated harmonization tools. |
| Refresh | Build and refresh AI/ML  models using a user-friendly, self-service platform.<br/>Get new results, including historic and forecasted ROIs by channel, on a weekly or monthly basis. |
| Optimize | Make rapid inflight optimizations by shifting spend across channels based on measured performance. |

{style="table-layout:auto"}


### Impact 

Successful implementation of this use can have the following impact:

* Maximize speed, scalability, and usability across measurement & analytic use cases with standardized data schemas and common data foundation.
* Rapidly make weekly or monthly inflight optimizations and maximize ROI with data-driven spend shifts that reflect best forecasted ROIs.

+++

-->

## 跨Adobe应用程序激活战术见解

此用例可帮助您通过访问接触点得分获取有关客户区段和历程的增量战略见解。

+++ 详细信息

### 挑战

这些用例解决的挑战包括：

* 仅靠自上而下的解决方案可能无法发现精细的关键优化机会。
* 测量模型的输出是压倒性的，描述过于夸张，并且不容易产生洞察或操作。
* 无法进行临时分析以获得见解，因为模型不透明，并且粒度分数不可用。


### 方针

此用例的基于步骤的方法是：

| 步骤 | 详细信息 |
|---|---|
| 模型 | 配置和训练AI/ML模型，以获得一致的MTA接触点分数和MMM聚合结果。 |
| 分析 | 将增量接触点得分导出到Customer Journey Analytics或外部BI工具中。<br/>执行粒度分析，并使用接触点得分构建高级仪表板。 |
| 操作 | 使用Real-Time Customer Data Platform为热门消费者区段创建和激活回顾链接。<br/>根据客户细分制定数据驱动型营销策略，以供未来活动使用。 |

{style="table-layout:auto"}


### 影响

成功实施此使用可能会产生以下影响：

* 了解增量客户行为和营销策略，为营销和整个组织的战略优先事项提供信息。
* 通过快速发现影响客户和您的业务的趋势以制定战略应对措施，最大限度地提高ROI。


+++
