# SCENE 4 — THE CHECKPOINT
*Act 1, Scene 4 — Act 1 Closer*

---

## GM Background — What This Scene Is

> *For the GM.*

The IDs work. That was the whole point of Scene 3. The party is no longer walking error messages — they have names, records, a data trail. By every standard they should be able to walk through a routine checkpoint without incident.

This scene exists because *should be able to* is not *will be able to.*

The Watson fringe checkpoint is understaffed, underfunded, and staffed by people who checked out of caring roughly two years ago. The standard scanner array reads chips, confirms identity, checks for outstanding warrants. The party will clear all of that. The issue is what's bolted to the side of the standard scanner array: a newer unit, Arasaka contractor markings, officially described in the city's infrastructure manifest as a **biometric cohesion scanner** — there to detect illegal cyberware that might destabilise the civic grid.

That is not what it does.

It is a **soul-integrity reader** — a Soulkiller network integration point, one of dozens distributed quietly across Night City's entry infrastructure over the last eighteen months. Its job is to measure whether a person's soul-signature matches Night City's ambient baseline. Everyone in the city carries trace soul-drain. The scanner confirms you're part of the network before letting you in.

The party is not part of the network. The party is as clean as the day they were born, a thousand years ago, in a different world.

If the scanner runs a full cycle on them, it will flag. The flag routes directly to a `CVGNC-OPS` alert. The Director will be notified within minutes.

**The official running the checkpoint does not know what the scanner actually does.** She was told it catches illegal hardware mods. She has never seen it flag anything. She does not know what happens when it does.

---

## The Scene

### Arrival

The Watson checkpoint is a concrete booth in a gap in a retaining wall — the unofficial border between the fringe and the district proper. The wall is grafitti-layered and pre-dates the current infrastructure by at least thirty years. The booth is newer and more tired somehow.

**One official on duty.** Late forties, city employee, the specific energy of someone who has survived this job by caring precisely as much as required and no more. She sits in the booth with a coffee that's gone cold and a tablet she's reading something on. The standard scanner arch is live — a low hum, a green status light.

Beside it, mounted on a secondary arm: the cohesion scanner. Matte grey casing. Arasaka contractor sticker, partially peeled. A blue status light. Newer than everything around it, which out here means approximately eighteen months old.

**The process:** Approach the arch, the chip broadcasts, the standard scanner reads, the official glances at the tablet, waves through. Standard. Thirty seconds per person.

The cohesion scanner runs automatically, parallel to the chip scan. The party has no way to know this from the outside. Its cycle takes **ten seconds per person** — long enough to complete during a normal passage if nothing flags. If it flags, it flags before the person has cleared the arch.

---

### What Each Character Sees

**Non-magic characters:** Standard checkpoint. Some piece of equipment they don't recognise. Nothing obviously wrong.

**Magic-sensitive characters (Arcana DC 12, or passive if 15+):** The cohesion scanner has it — faint, but there. The **purple-black iridescence**, the same trace they saw in the tomb's walls, in the Arasaka agents' eyes. Not aggressive. Passive, the way the tomb's drain residue was passive. But networked — a thread of it running back from the scanner into the city infrastructure like a root in concrete. *This scanner is part of the same system that drained them for a thousand years.* It is looking for what it recognises. They are exactly what it doesn't.

They have roughly **one round** — as the first person approaches the arch — before the scan begins.

---

### Resolution Options

The party can attempt one approach per person, or set something up before anyone walks through.

---

**Option 1 — Walk through and hope**

The scan runs. Each character makes a saving throw — **Charisma DC 15** (the soul-integrity reading; clean souls should flag but the scanner is an imperfect instrument and a high personal resonance might pass as noise).

- *Success:* The scanner reads anomalous but within tolerance. Blue light stays blue. Move through.
- *Failure by 4 or less:* The scanner hesitates — the blue light flickers. The official notices and gives it a look but shrugs it off as a hardware glitch. Move through, barely. One flag event is already logged silently.
- *Failure by 5+:* The scanner flags. See *If It Flags* below.

Each failure (even partial) is logged silently in `CVGNC-OPS`. The party won't know. The Director won't act on one anomalous reading. He'll act on a pattern.

---

**Option 2 — Bribe the official**

A persuasion or deception approach — tell her the scanner is glitching, that it's been flagging clean people all week, that this is above her pay grade and she should just wave them through.

**Persuasion DC 13** to get her to stop watching closely. **Deception DC 15** to convince her the scanner has a known fault. Either success means she processes them with minimal attention.

This does not stop the scanner running. It means she's not looking when it does. If it flags — she *misses it*, or minimises it, depending on how well the roll went. A DC 15+ success means she waves them through without noticing a flag at all. A partial success means she notices but doesn't act immediately, giving them a window to move.

**Bribery (no roll, flat cost):** 300 eddies or equivalent. She pockets it. She processes them. She does not look at the scanner. She has done this before. She will do it again.

The bribery does not suppress the flag log. The CVGNC-OPS record still writes silently. But nobody in that chain will know the official was paid — they only see the flag event, if they look.

---

**Option 3 — Interfere with the scanner (netrunner)**

The cohesion scanner is a networked device. It has a local wireless access point — a convenience for Arasaka's maintenance contractors.

A netrunner can attempt a **quick wireless intrusion** — not a full run, just enough to scramble the scanner's cycle for thirty seconds. This uses the standard mechanics at a simplified scale:

- **No architecture to navigate.** It's a single node, single ICE (a basic Watchdog, DC 12 to bypass or destroy).
- **Wireless intrusion starts the Trace Clock at DETECTED** — the scanner's parent network knows someone is touching it. This does not alert the checkpoint official. It does start a timer: **4 rounds** before an automated flag routes to Arasaka's maintenance team (not CVGNC-OPS — a different channel, lower priority).
- On **success:** The scanner runs an error cycle for 30 seconds. Blue light blinks amber, resets. Anyone who passes through in that window gets no soul-integrity scan. The chip scan completes normally.
- On **failure:** The scanner runs normally. The intrusion attempt is logged but not acted on immediately.

---

**Option 4 — Interfere with the scanner (magic)**

A magic user can attempt to disrupt the scanner directly — a subtle application of whatever school fits their character. Not destruction. Interruption.

**Arcana DC 13.** Success: the scanner reads their interference as a calibration error and pauses its cycle — same 30-second window as Option 3, covering whoever passes through during it. The scanner cannot identify the source of the interruption; it has no pattern for arcane interference.

**On failure:** The scanner completes its cycle normally on the attempting character. On a failure by 5+, the scanner registers *something actively wrong* — not a standard flag but a secondary alert that routes separately: `ANOMALOUS SIGNAL — ARCANE ORIGIN`. This is a flag the Director has set personally. He gets this one fast.

**The cost:** Disrupting the scanner requires a 1st-level spell slot and 30 seconds of maintaining the effect — meaning the magic user is the last through, covering everyone else but exposed longest.

---

**Option 5 — Avoid the checkpoint entirely**

The checkpoint is the *official* entry. There are unofficial ones.

Splice mentioned, without being asked, that the storm drain system that runs under the Watson retaining wall empties out three blocks into the district. The drain access is behind a fuel depot on the fringe side — not monitored, not scanned, not on any official entry record. It is also, reportedly, occupied.

**Using this option:** No scanner. No official. No ID check. The party enters Watson without any checkpoint record at all, which is useful — no log, no flag, nothing for anyone to find.

The complication: the same drain system from Scene 3's Option B. The woman with the amber eye is here. She was there then and she is here now, which means she has *moved*. Same stillness. Same clean soul signature for any magic user who checks. She is between them and the drain exit.

She doesn't attack. She looks at them for a long moment. Then she says — the first thing she's said either time:

> *"You shouldn't be here yet."*

She steps aside.

They come up in Watson with no record of entry and one new question that has no answer.

---

## If It Flags

The blue light goes red. A tone — not loud, not an alarm, a soft administrative sound.

The official looks up from her tablet. She looks at her panel. She looks at the party. She does not know what `CVGNC-OPS CONVERGENCE SIGNAL — VERIFY AND HOLD` means. She knows it means she's supposed to do something.

> *"I'm going to need you to step back from the arch. This'll just be a minute."*

She is not hostile. She is not reaching for a weapon. She is reaching for a phone.

**The window:** They have roughly **2 minutes** before someone who knows what that flag means picks up the call. Not the Director himself — a duty officer in the CVGNC-OPS chain, who will ask the official to describe what she's seeing, confirm the signal, and issue a hold instruction. After that: 8 minutes before an AV.

**What the party can do in the window:**

| Action | What It Buys |
|---|---|
| Run — back into the fringe | They're out of the checkpoint. The flag is logged but unconfirmed. The duty officer gets a "subjects fled" report. Pattern is building but still deniable. |
| Talk her down fast | Persuasion DC 16 to convince her this is a known equipment fault before she reaches anyone. Hard, not impossible. |
| Take the phone / break the call | Buys the full 8 minutes before anyone knows the call wasn't completed. Leaves the official as a witness. |
| Netrunner kills the flag at source | The scanner's node is live. A wireless intrusion, now under pressure, can delete the flag event before it routes. DC 14, Trace Clock starts at DETECTED, 2 rounds before the duty officer's terminal shows the incoming flag — they need to move faster than the alert. |
| Magic user collapses the scanner | Destroys the unit. No more flag, no more routing — but a broken Arasaka scanner at a city checkpoint is itself a reportable incident. Different problem. Slower response. |

---

## Crossing the Threshold

However they get through — cleanly, barely, or sideways through a drain — there is a moment when the city is on both sides of them and the fringe is behind them.

Give it to the players. The skyline from inside is different from the fringe — not the distant glow they've been moving toward since Scene 1, but towers overhead, sound that has layers, the smell of food and chemicals and the particular warmth of a city that never entirely goes cold. Ads running on building faces six storeys tall. People who do not look up.

They are in Night City.

They have fake names, fresh chips, and a flag somewhere in an Arasaka duty log that may or may not get followed up on.

**Act 1 ends here.**

---

## Act 1 Closing — What the Party Should Have

Before moving to Act 2, confirm the party has touched the following threads. Any they missed remain available — they don't disappear, they just sit:

- [x] Escaped the tomb and the Arasaka response
- [x] Made uneasy contact with Rook and the nomads
- [x] Seen Night City from outside and inside
- [ ] The woman in the pocket dimension — heard the grandmother's story (Rook) and possibly the woman in the drain
- [x] First encounter with corruption in Arasaka personnel (the agents at the tomb)
- [x] Received a lead on the Archivist (Rook's map)
- [ ] The old woman's death certificate — Watson, 107 years old, Director notified
- [ ] "Soul-clear" — a phrase exists for what they are

---

## Thread Seeds — End of Scene 4 / Act 1

| Thread | Hook | Urgency |
|---|---|---|
| The CVGNC-OPS flag | May or may not have been logged. Pattern building. | Background — slow escalation |
| The woman in the drain | "You shouldn't be here yet." Clean soul. Moving. | Active question |
| The old woman's record | Director-notified, 107-year-old Watson resident | Actionable in Act 2 |
| The Archivist signal | Southeast, on Rook's map | Waiting |
| "Soul-clear" | Voodoo Boys have a word for what they are | Act 2 faction hook |
| Night City | They're in. They need shelter, contacts, a direction. | Immediate |

---

## Notes / Table Variants
*(Add session notes after running)*
