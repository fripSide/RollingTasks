# RollingTask

```mermaid
flowchart LR
    A[task-new.md<br/>新任务] --> B[task.md<br/>本轮处理]
    B --> C[task-done.md<br/>已完成]
```

1. Agent 将 `tasks/task-new.md` 中的现有任务移到 `tasks/task.md`，用户可继续在task-new中添加新任务。
2. Agent 只处理并验证本次`task.md`移入的任务。
3. 完成后，Agent 将`task.md`中的任务移到 `tasks/task-done.md`。
