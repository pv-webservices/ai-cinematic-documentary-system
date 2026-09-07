# Skill Versioning Strategy

- `v1.0` — initial usable production version.
- `v1.1` — backward-compatible refinement, stronger checks, wording/schema extension that does not redefine the Skill's purpose.
- `v2.0` — major structural/behavioral change or incompatible output schema.

Whenever evidence changes a Skill, record:
- Skill;
- previous version;
- new version;
- reason;
- evidence (analytics/experiment/editorial incident);
- expected effect;
- date.

Git history retains old versions. Do not overwrite history with undocumented “optimization.”
