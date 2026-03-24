# SCENE 3 — GHOST IDs
*Act 1, Scene 3 — The Night City Fringe*

---

## GM Background — The ID Problem

> *For the GM. The mechanics of identity in Night City.*

Every person in Night City carries a **neural signature chip** — a subdermal implant installed at birth or on first entry into city infrastructure. It broadcasts a low-level signal: name, citizenship tier, corp affiliation if any, credit access level, outstanding warrants. Every door scanner, transit node, checkpoint, bar entrance, and Arasaka camera grid reads it passively. It is not optional. It is not something people think about. It is simply what you are in this city.

The party has nothing. No signal. No entry in any database. To a checkpoint scanner they are the equivalent of a walking error message — not criminals, not runners, not ghosts. *Errors.* That draws people. That draws questions. That draws, eventually, Arasaka, who are already looking.

**The surface fix:** A chip that broadcasts *something* — a fabricated identity, plausible enough to pass routine scans. Every fringe fixer can supply these. They last until a serious checkpoint probes deeper than the surface broadcast.

**The real fix:** Getting those fabricated identities written into an actual city database so they have a data trail, a history, records. Then the chip isn't broadcasting a fiction — it's broadcasting a shallow truth. This is harder, requires a netrunner, and involves touching city infrastructure without getting caught.

**The GM's constraint:** Even a perfect fake ID doesn't solve the deep problem. The party's clean soul-integrity will still read as anomalous to anything that probes at the level Arasaka uses. The IDs buy them freedom of movement in most of the city. They do not make the party invisible to the Director's eyes. Let the players feel the win without giving them false safety.

---

## Setup — Rook's Dropoff

Rook stops the vehicle at a dust-caked service road that dead-ends at a collapsed overpass. Beyond it, the city begins in increments — light pollution first, then sound, then the smell of something burning that never quite stops.

She doesn't get out. She rolls down the window.

> *"There's a place about half a kilometre up, under the bridge stanchion. Splice. She runs a body shop — legitimate on the surface, don't look too hard. She does work for people who need to not exist. Or need to start existing. Tell her I sent you."*

She pauses.

> *"She's going to want something. Not just eddies. Figure out what it is before you agree to it."*

She hands over the hand-drawn map (from Scene 2) if she hasn't already. She does not look back when she drives away. The vehicle's lights disappear into the dust.

**The city on the horizon:** This is the party's first ground-level view. Not the distant skyline from the Badlands — close enough now to see individual tower windows lit against the smog, AVs moving between buildings like slow insects, a corpo logo the size of a city block running in pale light. Nothing from Wildemount prepared them for scale like this. Give them a moment before moving them forward.

---

## Splice — First Contact

*[See NPC file: [Splice](../npcs/splice.md)]*

The body shop is under the bridge stanchion — a converted vehicle repair bay, three walls and a reinforced roll-door, the fourth side open to the underpass. It smells of metal and antiseptic and the particular ozone of active cyberware calibration equipment.

Splice is mid-thirties, shaved head, tattoos running from both temples down to her collarbones in a pattern that any magic-sensitive character will recognise as deliberately mimicking the look of circuit traces — it is aesthetic, not functional, but she had someone design it knowing that. She has done her research on things that live at the edge of what Night City calls real.

She does not seem surprised to see them.

> *"Rook's people. Okay."*

She looks them over — not rude, systematic.

> *"You're running dark. No broadcast at all. That's not a malfunction, that's never happened. Who are you?"*

She asks it genuinely, not as a challenge. She is *interested*.

---

## Beat 1 — The Negotiation

Splice can provide:
- **Ghost chip installation** — the hardware, subdermal, takes twenty minutes per person
- **Shallow ID packages** — fabricated identities with enough surface detail to pass automated scans and most human checkpoints
- **Database insertion** — this is the harder part, and it costs separately

**What she wants:**

She has a problem she hasn't been able to solve. There's a specific **city records node** — a municipal archive server, mid-tier security, not Arasaka-controlled — that holds the civil registry for the Watson district. She needs three things from it:

1. A specific file deleted — a record that connects her to an old name she no longer uses
2. Their fabricated identities written in as legitimate citizens
3. In and out clean, no trace of the intrusion

She had a netrunner lined up. The netrunner is currently in a hospital after a job went wrong. She's been sitting on this problem for two weeks.

**The offer:** She does all the hardware work, all the ID fabrication, for free, if they get into that node and do what she needs done. She provides the access point and everything she knows about the node's architecture. The rest is on them.

**If they ask about the deleted record:** She'll say it's personal and the conversation ends there. If they press hard enough later, with trust built: she changed sides on something years ago and the old record is evidence. She's not proud of which side she was on. She doesn't say which one.

---

## Beat 2 — Getting Into the Node

### The Access Point
Splice has a hardline tap into a decommissioned city infrastructure relay about three blocks into the fringe — a physical connection point to the Watson civil net, old enough that it's not on Arasaka's active monitoring list. Getting to it requires moving through a block of fringe territory that is nominally controlled by a small gang (the **Rust Dogs**) who mostly care about turf fees and mostly leave corporate-looking strangers alone.

*Mostly.*

**Option A — Pay the turf fee.** A few hundred eddies, or an item of value, gets them through without incident. The Rust Dogs don't look too hard at people who pay without arguing. Splice can front the money if the party is entirely broke, which she'll note without warmth.

**Option B — Go around.** Longer. Takes them through a storm drain system that comes out behind the relay. No gang contact. Instead, the drain system is home to a woman — clearly once human, heavily augmented, far past any corp maintenance contract — who has been living there for what appears to be years. She doesn't attack. She watches them pass. One eye is standard, the other is something older and glows faint amber. **Magic-sensitive characters:** there is no corruption signature on her. None. She is as clean as the party. She does not speak. She disappears back into the dark.

*(GM note: She is not a plot point for this scene. She is a question mark. File it.)*

**Option C — Bluff through.** The party's lack of ID signal is actually useful here — the Rust Dogs' scanner shows them as errors, which reads, sometimes, as corp dark-op. A confident lie and a plausible cover story might get them waved through with more speed than Option A.

### The Node
The relay access point is a locked junction box on the side of a building that probably used to be a post office. Splice provided a physical key. Inside is a hardline port and a nest of cables that haven't been touched since someone who is now definitely dead last maintained them.

**The node itself — what they're dealing with:**

| Layer | Description | Challenge |
|---|---|---|
| Surface | Old municipal OS, outdated security protocols | Straightforward entry for anyone with basic netrunning capability |
| Registry | Civil records — searchable, editable, logged | Finding the right records requires knowing what to look for; Splice gave them the file reference |
| Watchdog | A legacy ICE program — not sophisticated, but persistent. It runs sweeps every four minutes. | Must be neutralised or evaded; it will lock the connection and alert a human admin if it catches them |
| Depth | Archived records going back decades — this is where Splice's old record is buried | Takes longer to reach; the watchdog runs more frequently down here |

**For the party without a dedicated netrunner:**

This campaign assumes the party may not have conventional netrunning skills. Options:
- A magic user can interface directly with the node — the junction box responds to arcane touch in a way that should not be possible. Treat it as a modified version of their normal spellcasting: they're reading and writing the node like a text they can alter. This is slow and strange and leaves a different kind of trace than normal netrunning. Splice will have questions.
- Physical work: the node's terminal has a manual access mode, older than the wireless system, that a skilled enough operator can use with direct input. Slower. More exposed. Effective.
- Combination: one person interfaces while another watches the clock and calls out when the watchdog sweep is due.

**The four-minute clock:** Run this with actual tension. When the watchdog sweeps, anyone still in the system needs to either be very quiet (hide their presence) or be out. Getting caught doesn't immediately end the run — it starts a countdown to a human admin getting an alert, which gives them maybe ten minutes before someone physically checks the relay.

### What They Find In There
While in the node — if they look beyond the immediate task — there is other data.

They don't have time to read it all. But one record catches: a flagged file, dated six months ago, marked with an access tag that reads `CVGNC-OPS / DIRECTOR-NOTIFIED`. The flag is on a civil record. A person. Female, Watson district, no corp affiliation.

The record beneath the flag is a death certificate. **Cause of death: natural causes.** Someone died of old age in Watson. The Director was notified. Why would the Director care about one old woman dying of old age?

**If they copy the record:** The woman's name and address are on it. She died in an apartment in Watson. She was, according to the record, **107 years old** — plausible but extreme. No family listed. No corp history. One note in the file, handwritten and scanned in: *"She always said she'd outlast them."*

This is a thread. Do not explain it here. Let them carry it.

---

## Beat 3 — Installation

Back at Splice's shop. She reviews what they did — not in detail, she doesn't need details, she just needs to know the deletions went through and the IDs are written. She checks on a screen that looks like it's running six things simultaneously.

> *"Clean. Better than I expected."*

She does not elaborate on what she expected.

### The Chipping
Each party member gets a chip installed — twenty minutes per person, local anaesthetic, a small incision behind the ear. Splice works fast and well. She narrates what she's doing in a low, professional tone, which is somehow more unsettling than if she were silent.

**The mechanical anomaly:**

When the chip initialises and attempts to sync with the host's biology, there is a moment — half a second — where the calibration reading goes wrong. Not dramatically. Just:

> *"Huh."*

She looks at the readout. Looks at the person. Looks back.

> *"Your baseline is different. Not in a bad way. In a way I've never seen."*

She finishes the installation. She doesn't ask the follow-up question out loud. She logs it privately, the way people who survive in the fringe log things they don't understand.

**For magic users specifically:** The chip seats in the nervous system and goes quiet. But in the first twenty-four hours, any spell they cast produces a very faint secondary signal — the chip momentarily reads the arcane discharge as biometric data and tries to log it. This manifests as a brief warmth behind the ear where the chip sits. It doesn't interfere with casting. It is simply there. A record of something the city's systems have no category for.

### New Identities
Splice hands over a physical card for each person — a backup authentication token, in case the subdermal chip is ever damaged. The card has their new name on it.

She lets each player name their own character's fake identity, or she has a list of plausible Night City names if anyone is at a loss. The names should feel slightly wrong — close but not quite right, the way a forged document always has something slightly off if you know what to look for.

**Splice's Name List** *(pre-generated, pull from this if players want one)*

| Female | Male |
|---|---|
| Vera Scholt | Dax Reiner |
| Nika Voss | Cael Muro |
| Sable Ortiz | Renz Takeda |
| Priya Holt | Ivo Crane |
| Zoe Marek | Bram Sorel |
| Kass Ellroy | Lev Nada |
| Mira Kade | Finn Okafor |
| Taja Wren | Rook — no, she says flatly, pick another |
| Cori Ashfeld | Soren Vael |
| Nyx Palvo | Dio Kestrel |

Names are real people — or were. Watson district residents, low profile, recently deceased or relocated out of city records. Splice picked ones with no living relatives in the system. She doesn't say this unless asked.

> *"These will hold everywhere that doesn't matter. Bars, transit, street checkpoints. Don't walk into an Arasaka facility expecting them to hold."*

She pauses.

> *"Don't walk into an Arasaka facility."*

---

## Beat 4 — What Splice Knows

If the party has treated her straight — not lied unnecessarily, done the job cleanly — she gives them something unprompted before they leave.

> *"You're not the first people Rook has sent me who didn't have a signal. You're the first ones where I couldn't figure out why. Most people running dark are hiding something. You're not hiding anything. You just — aren't there, in the way the city expects people to be."*

She looks at them.

> *"There's a word for that, out in the Blackwall communities. 'Soul-clear.' I always thought it was mysticism. People talking about something they didn't have a real word for."*

She doesn't know what the word means in the context she's using it. She heard it from a Voodoo Boys adjacent contact and filed it. But she's giving the party a thread: the phrase exists. Someone out there has a name for what they are.

---

## End of Scene — Into the City

They have IDs. They have chips. They are, for the first time, *people* as far as Night City's infrastructure is concerned.

The city is right there.

Give them the approach — the checkpoint at the Watson border fringe is understaffed and tired. The scanner reads four new names. No flags. The guard waves them through without looking up.

Night City opens. Scene 4 begins.

---

## Thread Seeds — End of Scene 3

| Thread | Hook | Status |
|---|---|---|
| The old woman's record | Director-notified death cert, 107-year-old Watson resident | Active — they have the file or the name |
| "Soul-clear" | Splice heard the word from Voodoo Boys contacts. A name for what they are exists. | Planted |
| The woman in the drain | Clean soul, no corruption signature, watching from the dark. Not explained. | Open |
| Splice's old record | What was she, before? She's not corp-aligned now. | Slow burn |
| Chip-magic interaction | The subdermal chip logs arcane discharge as biometric data | Mechanical detail, long-term complication |
| Mote's scan log | Now the chip data will join it — two sets of anomalous records on the party | Risk, background |

---

## Notes / Table Variants
*(Add session notes after running)*
