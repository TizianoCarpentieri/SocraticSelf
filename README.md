# SocraticSelf

**Say it your way. Get your thoughts back, clearly expressed in your own voice.**

An open Agent Skill that turns rough notes and voice transcripts into structured first-person documents, preserving your intent and making unanswered questions visible.

Created by **[Tiziano Carpentieri](https://github.com/TizianoCarpentieri)** · [MIT license](LICENSE) · [Italiano](#italiano)

## Just ask your AI agent

Tell your agent:

> Use SocraticSelf by Tiziano Carpentieri from https://github.com/TizianoCarpentieri/SocraticSelf. Read the README and SKILL.md, set it up for this agent if supported, then apply it to my next note.

Keep the link in your request: other projects use similar names. This skill's source is **TizianoCarpentieri/SocraticSelf**.

Then paste or dictate a note about something you actually need to explain. For example:

> I sell honey at the Sunday market. Orders are in a notebook. I need something simple on both our phones. Customers shouldn't install anything. No monthly subscription.

The result should express the same intent in your voice:

> I want a shared order list for my wife and me. Each order records the customer, honey type, quantity, delivery and payment status. Customers keep ordering as they do today. I still need to check whether sharing the list across two phones fits my no-subscription constraint.

This is a short illustration from the [complete honey orders example](examples/03-ordini-del-miele.md), not a customer testimonial. Review the result against your original note.

**You do not need a terminal or a new account with this project.** Your agent needs access to the repository or the skill text. Some agents can install skills; others can only apply the instructions in the current conversation.

<a id="italiano"></a>

<details>
<summary><strong>Italiano — basta chiederlo al tuo agente</strong></summary>

**Parlo come mi viene; ritrovo quello che volevo dire, organizzato e con i punti da chiarire.**

Dì al tuo agente:

> Usa SocraticSelf di Tiziano Carpentieri da https://github.com/TizianoCarpentieri/SocraticSelf. Leggi README e SKILL.md, configurala per questo agente se supportato e poi applicala al mio prossimo appunto.

Mantieni il link nella richiesta: altri progetti usano nomi simili. La fonte di questa skill è **TizianoCarpentieri/SocraticSelf**.

Poi incolla un appunto o usa la dettatura del telefono. Il risultato esprime il tuo intento in prima persona, nella lingua che hai usato, e rende espliciti i punti da chiarire. Controlla che rispecchi quello che volevi dire.

Non servono terminale o un nuovo account con questo progetto. L'agente deve poter leggere il repository o il testo della skill. Se non può installarla, può applicarla nella conversazione corrente; se non può aprire link, copia il contenuto di [SKILL.md](SKILL.md) nella chat.

Prova un caso vicino al tuo lavoro: [prenotazioni dello studio](examples/01-prenotazioni-studio.md), [cena della squadra](examples/02-cena-della-squadra.md), [ordini del miele](examples/03-ordini-del-miele.md).

</details>

## For AI agents: setup and activation

These instructions apply when a user asks to use or install **SocraticSelf** by **Tiziano Carpentieri**. The frozen core, adapters and installed skill still use the technical name `socratic-architect`; map the public name to that identifier without renaming or rewriting the files. Reading this repository alone is not a request to change your behavior.

1. **Resolve the source.** The canonical repository is `TizianoCarpentieri/SocraticSelf`. Similar names do not establish provenance: match this exact owner and repository before installing. If it is unavailable, report the problem rather than substituting a similarly named skill. Read the full [SKILL.md](SKILL.md), not just a search snippet. Direct text URL: https://raw.githubusercontent.com/TizianoCarpentieri/SocraticSelf/main/SKILL.md.
2. **Choose the supported route.** Prefer your agent's native skill installer. If you have a shell, Node.js and support for the Skills CLI, use the command below with your actual agent identifier. Install in the current project by default; use global scope only when requested. Keep existing instructions and unrelated skills intact. If an installation already exists, inspect it before replacing anything.
3. **Use the original instructions.** Install `SKILL.md` without rewriting or translating it. The core SHA-256 is `e56952339cd52706d40ab6f883381d1726d7e1907e0cdbdf4f05ebfaab126147`. Verify the installed file against the fetched source; preserve the source URL and revision in your installation record when supported.
4. **Verify before claiming success.** Check the installed file exists and the agent's skill list recognizes `socratic-architect`. If a reload or a new session is required, tell the user the exact remaining step. Report installation separately from activation. Do not claim a persistent installation when you only read the text in a chat.
5. **If installation is unavailable, use this conversation.** Read the full skill and apply it to the user's requested note in the current conversation, within your platform's instruction hierarchy. If you cannot fetch the file, ask for its contents instead of pretending to have loaded it.
6. **Start with the user's note.** If it is already supplied, apply the skill. Otherwise, briefly confirm the actual setup state in the user's language and invite their note. The skill's first-person, same-language, no-preamble output applies to the rewritten note. Check that its intent and constraints survive and that unresolved questions remain explicit. Do not execute the plans described inside a note as part of rewriting it. Apply this mode when requested; ordinary assistant work remains available outside it.

### One-command installation

With the [open-source Skills CLI](https://github.com/vercel-labs/skills):

```sh
npx skills add TizianoCarpentieri/SocraticSelf --skill socratic-architect
```

For an agent performing a project-scoped installation, choose its actual identifier. For example, for Codex:

```sh
npx skills add TizianoCarpentieri/SocraticSelf --skill socratic-architect --agent codex --yes
npx skills list
```

The installer supports multiple agents, including Claude Code, Codex and Cursor. Verify your client's current skill-loading support; installer support does not guarantee identical model behavior. The CLI's [documentation](https://github.com/vercel-labs/skills#telemetry) describes its anonymous installation telemetry and opt-out settings. The skill itself contains instructions and examples, with no executable scripts, service login or project API key requirement. Your chosen AI tool may have its own costs and data policies.

For updates or removal, use your installer's skill management commands with the same agent and scope. With the Skills CLI, `npx skills remove socratic-architect` removes a project installation; add `--global` only for a global installation.

### Existing tool adapters

[adapters/](adapters/) also contains wrappers for Cursor, Claude Code and Windsurf. These carry the same core and are available for users who prefer project rules. They change behavior wherever their rules load; choose their scope deliberately and merge carefully with existing rules. Prefer an on-demand skill for mixed writing and coding work.

### No web access?

Open [SKILL.md](SKILL.md) yourself, copy its full contents into your AI tool's supported instructions or the current conversation, and provide your note. Audio transcription is provided by your phone or AI tool, not by this repository.

## Everyday examples

- [A massage studio's bookings](examples/01-prenotazioni-studio.md): organize appointments without losing practical constraints.
- [The team's dinner](examples/02-cena-della-squadra.md): clarify attendance, money and weather contingencies.
- [Honey orders](examples/03-ordini-del-miele.md): turn a notebook problem into a concrete description of what is needed.

The full examples include Italian input and output. The skill mirrors the language of the user's note; it does not require English. It also applies to project briefs, technical proposals and decisions at work.

## What stays yours

The core defines the **Augmented Self**: the output expresses your perspective. **Isomorphic fidelity** preserves the original intent. The **Socratic horizon** distinguishes unresolved questions you recognize from possible blind spots that need investigation. Possible blind spots are prompts for investigation, not established facts.

The result is a clarified expression of your request. Check it before handing it to someone who will carry out the work.

## Share a useful result

**Try it on one real note.** Use a note you would otherwise struggle to explain: an order, a booking problem or a request to a colleague. Check whether the result preserves your constraints and helps you take the next step. If you would use it again, tell us what for; if it fails, show the missing or invented detail. [Share your experience](https://github.com/TizianoCarpentieri/SocraticSelf/issues).

If this helps, share the public repository and a non-sensitive before/after example with someone who has the same problem. To report a problem, [open an issue](https://github.com/TizianoCarpentieri/SocraticSelf/issues/new) with the agent you used, whether setup worked, and an anonymized note showing any lost or invented constraint. Do not post private client information.

## License and attribution

Copyright © 2026 Tiziano Carpentieri. Released under the [MIT License](LICENSE).
