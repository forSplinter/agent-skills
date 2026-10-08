---
name: resources-format
description: Format of the RESOURCES.md file in each teaching workspace, the curated sources lessons are built from.
---

# Resources format

`RESOURCES.md` lists the trusted sources for the topic. Lessons draw their knowledge from here, and wisdom comes from the communities listed here.

## Template

```markdown
# 🦦 Resources · <topic>

## 📚 Knowledge

- [The Rust Programming Language (official book)](https://doc.rust-lang.org/book/)
  The canonical introduction. Use it for ownership, borrowing, error handling and the module system.

## 🗣️ Wisdom

- [Rust Users Forum](https://users.rust-lang.org/)
  Well-moderated and beginner-friendly. Use it for code critique and idiom questions.

## 🕳️ Gaps

- <An area the mission needs that no good resource covers yet>
```

## Rules

- **High trust only.** Prefer official docs, recognised experts and well-moderated communities. Leave out marketing that poses as teaching.
- **Annotate every entry.** One line on what it covers and when to reach for it, because a bare link means nothing three months later.
- **Name the gaps.** When the mission needs something no good source covers, list it under Gaps so later sessions keep searching.
- **Prune hard.** Remove a source that turned out wrong, shallow or off-mission. Five sharp sources beat thirty average ones.
- **Respect opt-outs.** When the user prefers not to join communities, note it here so later sessions stop proposing them.
