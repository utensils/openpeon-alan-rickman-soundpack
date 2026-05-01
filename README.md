# Alan Rickman

A [Claudette](https://github.com/utensils/claudette) sound pack voiced in the manner of the late Alan Rickman. Slow. Deliberate. Faintly amused.

## About

Claudette supports custom notification sound packs in the [OpenPeon](https://openpeon.com) format. This pack replaces the default notification sounds with spoken-word cues voiced in the style of Alan Rickman, giving your Claude Code sessions the particular energy of a man who has infinite patience for your nonsense and would like you to know it.

Alan Rickman's voice carries weight, precision, and barely-concealed wit — the opposite of a beep. This pack is for people who want their tools to feel like someone extraordinarily capable is keeping an eye on things, and will inform you of developments at a pace that suits *him*.

If you spend hours a day in Claudette, the audio character of your notifications matters more than you'd think.

## Installation

### In-app (recommended)

1. In Claudette, open **Settings → Notifications → Sound Packs**
2. Browse the OpenPeon community packs and install **Alan Rickman** from the in-app browser
3. Set **Alan Rickman** as your active pack

### Manual (clone)

Claudette stores sound packs in `~/.claudette/packs/` and picks up new packs automatically — no restart needed. The directory name **must** match the manifest's `name` field (`openpeon-alan-rickman-soundpack`), otherwise Claudette's pack-management UI won't be able to find or remove it later.

**macOS / Linux:**

```bash
mkdir -p ~/.claudette/packs
git clone https://github.com/utensils/openpeon-alan-rickman-soundpack.git \
  ~/.claudette/packs/openpeon-alan-rickman-soundpack
```

**Windows (PowerShell):**

```powershell
git clone https://github.com/utensils/openpeon-alan-rickman-soundpack.git `
  "$env:USERPROFILE\.claudette\packs\openpeon-alan-rickman-soundpack"
```

Then open **Settings → Notifications → Sound Packs** in Claudette and select **Alan Rickman** as your active pack.

To update later, `git pull` inside the pack directory. To uninstall, delete the directory.

Requires a version of Claudette with OpenPeon community pack support.

## What's included

This pack covers the six CESP categories defined in `openpeon.json`, each with ten phrasing variants so the same line doesn't repeat back-to-back. Claudette picks one of the ten at random per event.

### `input.required` — agent needs your input

Polite authority. Not a request — a summons dressed as one. Plays when Claudette needs you (permission prompts, questions).

1. "A moment of your time, if you'd be so kind."
2. "I find myself... requiring your attention."
3. "Forgive the interruption. There is a matter."
4. "Your input would be most welcome. Whenever you're ready."
5. "Tell me — and do be specific."
6. "There is something I must ask. Indulge me."
7. "A small clarification, if you would."
8. "Pause, please. I have need of you."
9. "Before we proceed... a question."
10. "Your attention, briefly. If it isn't too much trouble."

### `task.acknowledge` — plan ready for review

The plan has been devised. You will hear about it. Plays when an agent has drafted a plan and is awaiting your sign-off.

1. "I have devised a plan. Do let me know what you think."
2. "A strategy, drafted for your consideration."
3. "The arrangements have been made. Awaiting your approval."
4. "I've taken the liberty of preparing something. Have a look."
5. "Consider this my opening move."
6. "A modest proposal. For your scrutiny."
7. "Behold — the plan. Such as it is."
8. "I've sketched the path forward. Tell me where I've erred."
9. "Here lies my approach. Approve, or do not."
10. "The blueprint is yours. Examine it at your leisure."

### `task.complete` — work finished

Dry. Final. Slightly self-satisfied. Plays when an agent finishes and hands control back.

1. "It is done."
2. "Finished. As promised."
3. "Complete. Returning the floor to you."
4. "There. That wasn't so terrible, was it?"
5. "Concluded. Without incident."
6. "Done. And rather well, if I say so myself."
7. "The matter is settled."
8. "Finished. You may resume breathing."
9. "Complete. The world, somehow, still turns."
10. "There. Tied with a neat little bow."

### `task.error` — something went wrong

Resigned. Never panicked. Faintly disappointed in the situation, if not in you specifically.

1. "We have encountered... a complication."
2. "Something has gone rather sideways, I'm afraid."
3. "An obstacle. Most inconvenient."
4. "I regret to inform you — it did not go to plan."
5. "Things have... not gone as intended."
6. "A misstep. Distinctly my own."
7. "Disaster, in miniature. Your assistance, please."
8. "It has all gone rather pear-shaped."
9. "An error. Singularly unhelpful."
10. "Something has broken. Tediously so."

### `session.start` — new session begins

Ready. On his own terms.

1. "At your service."
2. "Shall we begin?"
3. "I am, as ever, ready."
4. "Speak. I'm listening."
5. "Here I am. Once more."
6. "And so we begin again."
7. "Pleasantries dispensed with — what is it?"
8. "A new day. A new task. Presumably."
9. "Awaiting instruction. As one does."
10. "I am here. The rest is up to you."

### `resource.limit` — context or quota reached

Accepting limits with immense dignity.

1. "We have, alas, reached our limit."
2. "Even I have my boundaries."
3. "That, I'm afraid, is all I can offer for the moment."
4. "The well, regrettably, has run dry."
5. "I have, regrettably, run out of road."
6. "The ceiling, I'm afraid, has been reached."
7. "No further. Not today."
8. "We have exhausted our allotment."
9. "That, as they say, is that."
10. "The threshold. Crossed. Reluctantly halted."

## Customization

OpenPeon packs are just structured archives — the `openpeon.json` manifest plus an mp3 per labeled variant. You can swap individual sounds without rebuilding the whole pack: drop a replacement mp3 into `sounds/` under the same filename and the manifest will continue to point at it. See the [OpenPeon documentation](https://openpeon.com) for the full pack format spec.

## Attribution

Audio generated using AI voice synthesis in the style of Alan Rickman. This pack is a tribute to his work; it has no affiliation with his estate. The voice characterization is inspired by his public performances and is intended for personal, non-commercial notification use.

## License

The audio files in this repository are released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — free to use, modify, and redistribute with attribution.

The pack metadata, scripts, and any code in this repo are released under the [MIT License](LICENSE).

## Contributing

Found a line that doesn't land right, or have an idea for how Alan Rickman would handle a new event type? Open an issue or PR. Feedback from people actually using the pack day-to-day is the most valuable input.

## Related

- [Claudette](https://github.com/utensils/claudette) — Claude's missing better half
- [r/ClaudetteApp](https://reddit.com/r/ClaudetteApp) — community subreddit
- [Claudette Discord](https://discord.gg/Ks9Ghnem) — chat with the team
- [OpenPeon](https://openpeon.com) — the sound pack ecosystem this format comes from
