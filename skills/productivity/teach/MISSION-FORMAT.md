---
name: mission-format
description: Format of the MISSION.md file at the root of each teaching workspace, the reason the user is learning the topic.
---

# Mission format

`MISSION.md` sits at the root of the workspace. It holds the reason the user is learning the topic, and every teaching decision traces back to it.

## Template

```markdown
# 🦦 Mission · <topic>

## 🎯 Why

<One to three sentences on the concrete goal. What changes in the user's work or life once they have this skill?>

## ✅ Success looks like

- <Something specific and observable the user will be able to do>
- <Another one>

## ⏳ Constraints

- <Time per week, deadline, budget, setup, learning preferences>

## 🚫 Out of scope

- <Nearby topics the user chooses to leave aside for now>
```

## Rules

- **One mission per workspace.** Two unrelated topics make two workspaces.
- **Concrete beats abstract.** "Ship a Rust CLI that profiles Parquet files" beats "learn Rust".
- **Interview before writing.** When the user cannot say why, ask until they can. A vague mission is worse than none.
- **Revise when reality moves.** Update the file when the goal changes, so a stale mission never steers a session.
- **Keep it to one screen.** Past that, it has become a plan instead of a compass.
