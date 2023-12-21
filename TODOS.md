Collection of all active todos

```dataviewjs
dv.taskList(dv.pages().file.tasks
	.where(t => !t.completed))

```
