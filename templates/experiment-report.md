# Agent 对照实验 / Agent comparison report

> 提交前填写所有关键字段。没有运行的数据标为「未测」，不要补推测值。
> Fill in key fields. Mark unmeasured results as unmeasured; do not invent values.

## 问题与假设 / Question and hypothesis

- 要验证什么 / Question:
- 什么结果会推翻假设 / Falsifying outcome:
- 预先固定的验收与质量门槛 / Preregistered acceptance and quality floor:

## 配置与复现 / Configuration and reproduction

| 项目 / Item | A：基线 / Baseline | B：改动 / Variant |
| --- | --- | --- |
| 模型标识与参数 / Model ID and parameters | | |
| 指令、工具和技能版本 / Instructions, tools, skills | | |
| 上下文和记忆策略 / Context and memory policy | | |
| 角色与编排 / Roles and orchestration | | |
| 预算、重试与停止逻辑 / Budget, retries, stopping | | |
| 验收者或验证程序 / Reviewer or validator | | |

- 唯一改变的因素 / Single changed factor:
- 任务集、版本与样本量 / Dataset, version, sample size:
- 输入、产物与轨迹位置 / Inputs, artifacts, traces:
- 调试集与保留验证集划分 / Development and held-out split:
- 重复次数、顺序随机化与缓存设置 / Repeats, order randomization, caching:
- 环境、时间和外部依赖 / Environment, time, external dependencies:
- 复现步骤 / Reproduction steps:

## 结果 / Results

| 指标 / Metric | A | B |
| --- | --- | --- |
| 通过数 / 总数 / Accepted / total | 未测 / Unmeasured | 未测 / Unmeasured |
| 端到端耗时（注明统计口径） / End-to-end latency | 未测 / Unmeasured | 未测 / Unmeasured |
| 所有尝试的总成本 / Total cost of all attempts | 未测 / Unmeasured | 未测 / Unmeasured |
| 每次合格交付成本 / Cost per accepted delivery | 未测 / Unmeasured | 未测 / Unmeasured |
| 人工介入与返工时间 / Human intervention and rework | 未测 / Unmeasured | 未测 / Unmeasured |
| 重复操作与权限越界次数 / Duplicates and authority violations | 未测 / Unmeasured | 未测 / Unmeasured |

- 币种、人工时间折算及成本边界 / Currency, time valuation, cost inclusions:
- 部署与维护成本是否单列 / Setup and maintenance costs reported separately:
- 不确定性与波动 / Uncertainty and variation:
- 失败样例、严重性与证据 / Failures, severity, evidence:
- 不可比较或被排除的运行及原因 / Excluded or incomparable runs and reasons:

## 结论与局限 / Conclusion and limits

- 结果支持了什么 / Supported conclusion:
- 不能推出什么 / Unsupported generalizations:
- 在保留任务上是否复核 / Held-out validation:
- 下一轮只改哪一项 / Next single change:

零成功时，不报告有限的「每次合格交付成本」。小样本不能被描述成普遍规律。
With zero successes, do not report a finite cost per accepted delivery. Small samples do not establish universal rules.
