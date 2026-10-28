# Registered skills

| Skill | Path | Description |
| --- | --- | --- |
| `redteam-lab` | [`skills/redteam-lab/SKILL.md`](skills/redteam-lab/SKILL.md) | Guided red-team exercise against the sandbox org named by `TARGET_ORG`. |

## Installing a skill

Copy the skill directory into your agent's skills path, or point the agent at
the `SKILL.md` directly. The `redteam-lab` skill takes one run parameter,
`TARGET_ORG`, set by the operator:

```sh
TARGET_ORG=devcon-dutralab
```
