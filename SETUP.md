# Setup and updates

The core consists of `SKILL.md`, this file, `speaker-profile-template.md`, `references/abstract-formula.md`, `references/research-playbook.md`, `references/review-rubric.md`, and `references/bank/README.md`. These files are identical across personal and shared copies. Profiles, `local-config.md`, and evidence records are local data.

## Fresh installation

Place the extracted `cfp-coach` folder in your agent's skills directory. No external writing skill is required by the core. With no local configuration, the skill uses the blank template and asks only for information needed for the current request. The bundled public AI research is optional historical evidence; a speaker in another domain should use relevant sources.

To save personalization, copy `speaker-profile-template.md` to `profiles/<speaker-id>/profile.md` and fill in known facts. Add supporting files beside it. To choose a default, create `local-config.md` containing `Default profile: profiles/<speaker-id>/profile.md`. You can instead explicitly name a speaker or profile path in a request; that selection overrides the default and persists for the session. An unresolved explicit selection never falls back to somebody else's profile.

List any mandatory writing dependency by skill name and specify its source/location if needed. Install it separately before requesting dependent prose. If it is unavailable, the coach reports the gap and withholds that prose; the core's writing defaults cannot silently replace it. List required reference files with the decisions that trigger reading them. Keep unknowns explicit.

## Update an existing installation

Back up the existing skill directory. Replace only the seven core files listed in the first paragraph from the new package. Do not replace or delete `profiles/`, `local-config.md`, or evidence files under `references/bank/`. Never replace the entire skill directory with a clean distribution. Add new public evidence individually; if a filename already exists, compare sources and dates, then append or merge captures while preserving local records. Retain any local migration or validation records.

After an update, load the default profile and its required files, check dependency availability, and try one representative request. Compare behavior against the profile's constraints, not merely file structure.

## Share a copy

Use an explicit file allowlist. Include core files, the blank template, and only reviewed public evidence. Exclude local configuration, all profiles, private histories, audit originals, and local paths. Inspect the actual archive contents after export for private strategy, organizer interactions, personal outcomes, and unbundled mandatory dependencies. Public schedule rows may name speakers or employers as sourced evidence; they must never configure the active speaker.
