# Operations

- Use a supported pregeneration plugin for actual chunk work; this repository is a workload plan, not a replacement chunk generator.
- Keep an immutable seed/generator manifest with each run.
- Record completed chunk coordinates so restarts are resumable.
- Avoid running pregeneration and region compaction simultaneously.
- Validate backups before deleting any source world.
