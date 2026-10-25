# 上下文交接 / Context handoff

> 用于 compact、reset、换执行者或跨会话恢复。不要粘贴全部历史；保留可恢复任务所需的信息与证据入口。
> For compaction, resets, reassignment, or session recovery. Preserve actionable state and evidence pointers.

- 任务 ID / Task ID:
- 更新时间与时区 / Updated at, timezone:
- 当前目标与最新约束 / Current goal and latest constraints:
- 当前配置版本 / Configuration version:

## 已验证的事实 / Verified facts

| 事实 / Fact | 证据位置与版本 / Evidence and version | 核验时间 / Checked at |
| --- | --- | --- |
| 填写 / Fill in | | |

## 工作状态 / Work state

- 已完成且验收的产物 / Completed and accepted artifacts:
- 已做但未验证的工作 / Work awaiting verification:
- 未完成的事项 / Remaining work:
- 已知失败与原因 / Known failures and causes:
- 已排除的方案及依据 / Rejected options and evidence:
- 外部动作及确认状态 / External actions and confirmation status:

## 下一步与失效条件 / Next steps and invalidation

- 下一项具体动作 / Next concrete action:
- 当前阻塞与需要的输入 / Blockers and required inputs:
- 剩余预算与重试次数 / Remaining budget and retries:
- 恢复后需重新获取的动态状态 / Dynamic state to refresh:
- 哪些旧结论可能已经失效 / Potentially stale conclusions:
- 不能重复的操作及检查方式 / Non-repeatable actions and status checks:

## 恢复确认 / Recovery check

- [ ] 最新目标与权限已确认 / Latest goal and authority confirmed.
- [ ] 关键证据可读取且版本一致 / Key evidence accessible and version-matched.
- [ ] 外部操作状态已核实 / External action status checked.
- [ ] 未把未经验证的总结当事实 / Unverified summaries not treated as facts.
