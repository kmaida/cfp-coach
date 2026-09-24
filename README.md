# CFP coach

CFP coach helps you prepare conference talk proposals using reviewer criteria, prior programs, and evidence from your own work. Use it to choose an angle, develop abstract seeds, or review a draft before you submit it.

The skill supports six kinds of work:

| Mode | Output |
|---|---|
| Conference research | Reviewer criteria, recurring topics, program gaps, and audience fit |
| Trend research | Dated evidence about topics and their relevance by the event date |
| Angle suggestions | Ranked ideas tied to experience you can demonstrate |
| Seed drafts | Working titles, rough abstracts, attendee takeaways, and missing facts |
| Review | A verdict, blocking issues, focused edits, and a comparison with the target program |
| Record keeping | Submission outcomes and research with sources, dates, and acceptance routes |

You control the final proposal. The skill doesn't submit or publish anything without your explicit instruction.

## Installation

With Node.js and npm installed, run these commands in your terminal:

```sh
npx skills add kmaida/cfp-coach --skill cfp-coach
npx skills add kmaida/deslop-skills --skill deslop-writing
```

The second command installs the strongly recommended writing skill. Follow the prompts to choose your agent. The default installation applies to the current project; add `--global` to each command to install for your user account across projects. See the [skills CLI documentation](https://github.com/vercel-labs/skills) for installation options.

For manual installation, place the `cfp-coach` folder in your agent's skills directory. Your agent needs file access to read the supporting references. Current conference research also needs web access.

## Get started

Ask for the work you need:

> Use cfp-coach to review this abstract for a practitioner audience. Identify blocking issues and suggest focused edits. Don't rewrite the whole abstract.

> Use cfp-coach to suggest talk angles from my wetland restoration study. Ask for any study details you need before making claims about the results.

You can start without a saved profile. Supply your draft or relevant experience, and the coach asks only for missing information needed for that request.

## Save your speaker preferences

Copy [the blank profile](speaker-profile-template.md) to `profiles/your-name/profile.md`. Add your expertise, voice preferences, and speaking goals as needed. You can also record product restrictions or link to submission history and planning documents.

To make that profile the default, create `local-config.md` in the skill folder:

```text
Default profile: profiles/your-name/profile.md
```

Name another speaker or profile in your request to override the default. Your explicit instructions take precedence over profile preferences; profile preferences take precedence over shared coaching defaults. Missing information stays unknown.

We strongly recommend [`deslop-writing`](https://github.com/kmaida/deslop-skills) for abstracts, titles, bios, and rewrites. It helps remove stock phrasing and filler while preserving your voice. The coach uses it when available, unless you specify another writing approach; built-in writing defaults let you start without it. If your profile requires a separate writing skill, install it before requesting drafts. The coach reports missing required dependencies and withholds the prose that depends on them.

## Research and private records

The [evidence bank](references/bank/README.md) includes dated AI conference schedules and YouTube view counts. Those captures provide historical examples; use sources from your own field and verify current deadlines before acting. Video views measure audience attention and don't establish why a committee accepted a talk.

Keep your submissions, organizer correspondence, and personal strategy in your profile directory. Store only public evidence in the shared bank. Public schedule rows may name speakers and employers; they don't define your profile.

Before committing local changes to a public repository, exclude personal files. Suggested `.gitignore` entries:

```gitignore
local-config.md
profiles/
migration/
.DS_Store
```

Ignore rules don't remove files already tracked by Git. Review the files you plan to publish, including research notes, before pushing.

## Updates

Follow [the setup and update instructions](SETUP.md) to replace shared core files while preserving your profiles, local configuration, and evidence records. Copy updated documentation alongside the core. Avoid replacing your entire personalized skill folder with a fresh download.
