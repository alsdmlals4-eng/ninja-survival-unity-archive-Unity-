# Ninja Survival Unity Archive Manifest

## Archive status

This repository is **ARCHIVE_ONLY**. It preserves an earlier Unity snapshot for historical inspection and comparison. It is not an implementation, release, QA, or asset-production authority.

- Current archive commit inspected: `a6499f0e62175609147bd2d66b6c48b16cb2331e`
- Snapshot file: `ninza.zip`
- SHA-256: `72e08c6d552ea5dfd25175082844cf360dd40eb3bf53544f229aae2887f20491`
- Current implementation authority: [`alsdmlals4-eng/ninja-survival-godot`](https://github.com/alsdmlals4-eng/ninja-survival-godot)

## Verified inventory boundary

2026-08-24 archive inspection used the ZIP central directory only; the ZIP was not edited or promoted to a runnable Unity build. Its file listing contains the expected Unity project roots:

- `Assets/`
- `Packages/`
- `ProjectSettings/`

The listing also contains earlier C# gameplay/UI scripts, scene/art content, and Unity project settings. This is evidence that the snapshot is inspectable, **not** evidence that the Unity project imports, builds, runs, has valid asset rights, or provides a player-ready experience.

## Use rules

1. Use this snapshot only to recover historical reference material or compare a narrowly defined behavior.
2. Re-design any selected behavior in Godot 4.x/GDScript; do not line-by-line port Unity code, MonoBehaviour structure, prefabs, scenes, or generated assets.
3. Keep production decisions, current code, visual/audio contracts, tests, and play evidence in `ninja-survival-godot` and its linked project system.
4. Any future extraction must occur in a disposable local workspace and record the inspected file set and source/rights assumptions before reuse.

## Evidence limits

The following were **NOT_RUN** by this audit: Unity import/build, Unity scene execution, human play, device validation, visual/audio quality evaluation, asset-rights verification, and conversion feasibility. Do not infer any of them from the archive file alone.
