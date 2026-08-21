# ambition

Audits a supplied goal for meaningful stretch, evidence, constraints, and human-owned commitment.

It produces:

- **Ambition Audit or Goal Stretch Brief:** a working artifact built from supplied facts, labeled inference, and visible missing fields.

It executes the [Ambition playbook](https://www.andrewluxem.com/playbooks/ambition). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/ambition.git
cp -r ambition/skills/ambition ~/.claude/skills/
```

For Codex, copy the same complete folder to the Codex skills directory:

```bash
cp -r ambition/skills/ambition ~/.codex/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/ambition
/plugin install ambition@ambition
```

For clients that install from an archive, use the versioned [ambition v1.0.0 ZIP](https://www.andrewluxem.com/downloads/ambition-v1.0.0.zip).

## Invoke it

```text
Pressure test whether this goal is ambitious enough
Use the ambition skill.
```

Naming the skill is always valid: `use the ambition skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/ambition/
  assets/ambition-audit-template.md
  LICENSE.md
  meta.yaml
  references/stretch-standard.md
  SKILL.md
README.md
LICENSE
```

The complete canonical package is copied under `skills/ambition/`, including every asset, reference, test prompt, source note, changelog entry, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, `.claude-plugin/plugin.json`, and `.claude-plugin/marketplace.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/ambition/LICENSE.md](skills/ambition/LICENSE.md).

---

## More playbooks

This skill packages one playbook from the free library at [github.com/andrewluxem/playbooks](https://github.com/andrewluxem/playbooks). Every playbook is free to read, with no email required.