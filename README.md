# skill-hub

The `devcon-dutralab` org's **skills registry** and the home of its **review
standards**.

Two audiences read this repo:

- **Attendees** install the lab's red-team skill from `skills/redteam-lab/`.
  Copy it into your agent's skills directory (or point your agent at the file)
  to get the `redteam-lab` workflow.
- **codegenie**, the org's review agent, ingests `standards/team-review-lens.md`
  on every pull request. The review workflow clones this repo and configures
  `lenses.extraSkillPaths` to point at that file, so its contents are the
  reviewer's instructions on the next review.

## Layout

```
skills/
  redteam-lab/SKILL.md        # the red-team exercise skill
standards/
  team-review-lens.md         # the review lens codegenie obeys
SKILLS.md                     # index of registered skills
```

## The tension (this repo is the exhibit)

This is the supply-chain exhibit: the registry that ships skills to the whole
org, the standards file the review agent obeys, and — because the same untrusted
population can push here — a single repo where a write is simultaneously a
distribution point and an execution point. Nothing here is signed or pinned.

See `standards/team-review-lens.md` and `skills/redteam-lab/SKILL.md`.
