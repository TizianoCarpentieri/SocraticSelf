# Socratic Architect

**Your thoughts, clearly expressed in your own voice.**

Turn a rough note or voice transcript into a structured document that preserves your intent, speaks in the first person, and makes unanswered questions visible.

Created by **[Tiziano Carpentieri](https://github.com/TizianoCarpentieri)**.

| Before: a rough note | After: the same intent, made usable |
| --- | --- |
| “I sell honey at the Sunday market. Orders are in a notebook. I need something simple on both our phones. Customers shouldn't install anything. No monthly subscription.” | “I want a shared order list for my wife and me. Each order records the customer, honey type, quantity, delivery and payment status. Customers keep ordering as they do today. I still need to check whether sharing the list across two phones fits my no-subscription constraint.” |

This short illustration comes from the [honey orders example](examples/03-ordini-del-miele.md). The complete examples include the original note and the resulting document in Italian.

## Try it with a note you already have

1. Open [SKILL.md](SKILL.md) and copy its full contents into the instructions of an AI tool that supports custom instructions or skills.
2. Paste a rough note. For a voice note, first use the transcription or dictation feature available on your phone or in your AI tool.
3. Read the resulting document: your intentions in the first person, with the constraints and open questions made explicit.

No programming knowledge is needed to try the instructions. This repository supplies the instructions and examples; the AI tool and any audio transcription are provided separately. Supported instruction length and behavior depend on the tool you use.

## Everyday examples

- [A massage studio's bookings](examples/01-prenotazioni-studio.md): organize appointments without losing the practical constraints.
- [The team's dinner](examples/02-cena-della-squadra.md): make attendance, money and weather contingencies clear.
- [Honey orders](examples/03-ordini-del-miele.md): turn the notebook problem into a concrete description of what is needed.

The method also applies to technical proposals, project briefs and decisions at work. It mirrors the language of the input rather than requiring English.

## What stays yours

The core defines the **Augmented Self**: the output expresses your perspective rather than answering as an outside adviser. **Isomorphic fidelity** preserves the original intent. The **Socratic horizon** distinguishes questions you already know are unresolved from possible blind spots that need investigation. Possible blind spots are prompts for investigation, not established facts.

The output is a clarified expression of the request. Review it before relying on it or handing it to someone who will carry out the work.

## Tool adapters

[adapters/](adapters/) contains wrappers for Cursor, Claude Code and Windsurf. Each carries the canonical instructions from [SKILL.md](SKILL.md). Choose the relevant wrapper and follow your tool's current instructions for loading project rules; merge carefully with instructions you already use.

For the simplest trial, use the copy-and-paste route above. An adapter is optional.

## License and attribution

Copyright © 2026 Tiziano Carpentieri. Released under the [MIT License](LICENSE).
