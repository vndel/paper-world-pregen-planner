# paper-world-pregen-planner

Operational plans for pre-generating Paper worlds without turning generation into an uncontrolled background workload. World generation is CPU- and I/O-intensive; isolate it from peak player hours and validate storage headroom.

## Safe rollout
1. Back up world data and record the world seed and generator/plugin versions.
2. Estimate target region volume and available disk space.
3. Run bounded batches on a staging copy; monitor MSPT, disk latency, and queue depth.
4. Stop on sustained tick pressure or storage alarms; resume from recorded coordinates.
5. Verify region files and perform a staged server boot before promotion.

Do not promise a TPS outcome from configuration alone. MIT licensed.
