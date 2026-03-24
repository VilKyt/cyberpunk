# NETRUNNING — MECHANICS
*A hybrid system: Cyberpunk Red architecture + D&D 5e dice economy*

---

## Design Philosophy

Cyberpunk Red's netrunning is grid-based and tactical but adds parallel complexity that can stall a table when only one player is doing it. D&D 5e is fast and skill-check-driven but has no native framework for hacking. This system takes:

- **From CP Red:** The architecture concept (nodes as rooms), ICE as obstacles, the vulnerability of the runner's physical body, programs as limited resources, brain damage as a real consequence
- **From D&D 5e:** Skill checks, saving throws, action economy, the existing spell slot / ability structure for magic users, advantage/disadvantage
- **Added:** A clock that keeps non-netrunners engaged, a risk-escalation track, and a simple way to run magic users interfacing directly instead of through conventional tech

The goal: a netrunning sequence that takes **10–20 minutes of table time**, keeps everyone at the table relevant, and has real stakes without requiring a separate mini-game rulebook.

---

## Core Concepts

### Architecture
The GM builds a node map before the session — a sequence of locations inside the system, like rooms in a dungeon. Each node has:
- A **type** (see below)
- A **DC** for interacting with it
- Any **ICE** present
- What can be **done** there (read, copy, delete, execute)

Nodes are connected in sequence. The runner moves through them one at a time. They cannot skip nodes unless a path around them exists in the architecture (the GM decides this when designing).

**Node Types:**

| Type | Description | Default DC |
|---|---|---|
| **Gateway** | Entry/exit point. Must be passed to enter or leave. | 12 |
| **File** | Data storage. Read, copy, or delete records here. | 10 |
| **Security** | System monitoring. Hosts watchdog ICE. Alerts if triggered. | 15 |
| **Daemon** | An active running program — could be hostile ICE or a useful tool. | 14 |
| **Root** | The deepest layer. Full system control. Heavily defended. | 18+ |

### ICE (Intrusion Countermeasure Electronics)
ICE is the system's defence. Think of it as a trap or a guard — it exists at a node and activates when the runner triggers it (usually by failing a check at that node).

ICE has two states: **Passive** (scanning, not yet aware) and **Active** (engaged, fighting back).

**ICE Types:**

| ICE | Passive Effect | Active Effect |
|---|---|---|
| **Watchdog** | Sweeps on a timer. Adds +2 to next Detection Roll if runner is slow. | Alerts system admin. Starts the Trace Clock. |
| **Tar Pit** | Slows movement — runner spends an extra action to leave the node. | Holds the runner in place until destroyed or bypassed. |
| **Asp** | No passive effect. | Deals psychic damage (1d6) on a failed CON save DC 13. |
| **Hellhound** | No passive effect. | Deals psychic damage (2d8) on a failed CON save DC 15. Aggressive — pursues. |
| **Black Ice** | No passive effect. | Deals psychic damage (3d10) on a failed CON save DC 17. On a failed save by 5+: unconscious. |

**Psychic damage from ICE:** This is real HP damage. The runner's mind is inside the system. What hurts the mind hurts the body. A runner reduced to 0 HP by ICE falls unconscious at their physical location — their body slumps, chip still jacked in. Someone needs to physically pull the cable, which ends the run immediately.

### Programs
Programs are the runner's tools — limited-use abilities that give them an edge in the net. They work like a small pool of resources, similar to spell slots.

A conventional netrunner starts each run with **3 program slots** (this can scale with level/equipment). Each program is single-use per run. Programs are not recharged mid-run.

**Basic Program List:**

| Program | Effect | Cost |
|---|---|---|
| **Worm** | Auto-pass one File or Gateway check. No roll needed. | 1 slot |
| **Sword** | Deal 2d6 damage to one ICE. | 1 slot |
| **Shield** | Gain advantage on one CON save against ICE damage. | 1 slot |
| **Cloak** | Advantage on one Stealth check to avoid detection. | 1 slot |
| **Decoy** | Reset the Trace Clock by one step. | 1 slot |
| **Nuke** | Destroy one ICE outright. No check. Loud — advance Trace Clock by one step. | 2 slots |

Magic users interfacing directly do not use programs. They use their existing spell slots, transposed into this framework (see below).

---

## The Run — Procedure

### Step 1: Jack In
The runner connects to the system — physically (hardline) or wirelessly. Wireless is faster but detectable. Hardline requires being at a physical access point but is harder to trace.

**Jacking in is a free action.** The run begins.

### Step 2: Map the Architecture
On entry, the runner can make an **Investigation check (DC 12)** to get a rough map of the system's structure — how many nodes, which direction the Root is, whether the Security node is between them and their target. On a failure they go in blind.

### Step 3: Move and Act
Each round in the net, the runner gets **2 actions:**
- **Move** to an adjacent node (1 action)
- **Interact** with a node — read a file, copy data, delete a record, attempt to bypass ICE (1 action)
- **Use a program** (1 action)
- **Jack out** (1 action — see Jacking Out)

Other party members take their turns normally in the real world. The run happens simultaneously with real-world time. Establish at the start: **1 net round = 1 real-world round.**

### Step 4: Node Checks
When the runner interacts with a node, they make a skill check against the node's DC:

| Node Action | Skill |
|---|---|
| Bypass a Gateway | Dexterity (Sleight of Hand) or Intelligence (Investigation) |
| Read/copy a File | Intelligence (Investigation) |
| Delete a record | Intelligence (Investigation) — DC +2 for deletion vs. reading |
| Bypass ICE (stealth) | Dexterity (Stealth) — opposed by ICE's passive detection |
| Fight ICE directly | Attack roll (use Intelligence modifier) vs. ICE AC |
| Navigate a Daemon | Wisdom (Insight) to understand it; Intelligence to control it |

**On a success:** The runner does what they intended. No alarm.
**On a failure:** Choose one — the runner fails the action *and* the node's ICE activates, OR the runner succeeds but the Trace Clock advances one step.

This choice belongs to the GM. It should be based on the fiction — a very loud failure in a Security node should always advance the clock. A quiet slip in a File node might just mean the data wasn't there.

### Step 5: The Trace Clock
Every system has a Trace Clock — a measure of how aware the system (and its owners) are of the intrusion. It has **four steps:**

```
[CLEAN] → [DETECTED] → [TRACED] → [BURN]
```

- **CLEAN:** Nothing is wrong. Normal operation.
- **DETECTED:** Something is in the system. Watchdog ICE activates. Security nodes add +2 to DCs.
- **TRACED:** The intrusion is being actively tracked. A human admin has been alerted. Real-world response begins — assume 5–10 minutes before physical arrival at the access point.
- **BURN:** The system executes a full lockdown and counter-intrusion. All ICE activates. The runner takes 2d6 psychic damage immediately and must jack out or be forcibly ejected (jack out, take 3d6 psychic damage, land at DETECTED on next run).

**Advancing the clock:** Failed checks (GM's choice), using Nuke, being detected by a Watchdog sweep, staying in a Security node more than 1 round without bypassing it.

**Rolling back the clock:** Using Decoy, successfully neutralising all ICE on a Security node, completing the objective and jacking out cleanly.

### Step 6: Jacking Out
The runner can jack out at the start of their turn, before taking any actions. Clean exit — no consequence.

If the runner jacks out **after** being hit by ICE in the same round, they take the ICE damage regardless.

If the runner is **forcibly ejected** (by Black Ice, or by reaching BURN), they take full damage and may be unconscious.

---

## The Real World During a Run

The party is not idle. Establish this clearly.

Someone needs to **watch the runner's body.** A jacked-in runner is physically vulnerable — eyes unfocused, unresponsive to touch, cannot act. If their physical body is attacked, they take damage normally but cannot defend themselves. If they take damage, they must make a **Concentration check (DC 10 + damage taken)** or be forcibly ejected from the net.

The rest of the party handles:
- Physical security (guarding the access point)
- Real-world threats arriving while the run is in progress
- Feeding information to the runner if they have a comms link
- Making decisions the runner can't — if a guard shows up at the junction box, someone has to deal with that without the runner

This keeps everyone at the table active. The run is not a solo event.

---

## Magic Users in the Net

Characters with spellcasting can interface with systems directly — without conventional netrunning hardware, or in addition to it. This is not how technology works. It is also, demonstrably, what happens when they touch the junction box in Scene 3.

**The mechanic:** A magic user can treat a node interaction as a spellcasting action, using **Arcana** instead of Investigation or Sleight of Hand, and spending a **spell slot** instead of a program slot.

| Spell Slot Level | Net Effect |
|---|---|
| 1st | Equivalent to a standard program (Worm, Shield, Cloak) |
| 2nd | Equivalent to a Sword program, or advantage on any one node check |
| 3rd | Equivalent to Nuke — destroy ICE, or force-pass a check. Does NOT advance the clock if cast subtly (the system cannot categorise what it's seeing). |
| 4th+ | Extraordinary effects — rewrite a running Daemon, open a locked Root node, leave no trace whatsoever of the intrusion |

**The tradeoff:** Magic in the net is slow. Each spell-slot action costs 2 actions instead of 1 — the interference between arcane and digital is mutual. But it is *very* hard to detect. Standard ICE has no recognition pattern for magic. A Watchdog sweep will not flag it. Only purpose-built Arasaka deep-scan ICE (which the party should not be encountering in Act 1) has any response.

**The corruption complication (GM note):** Any system that runs on Arasaka infrastructure carries trace soul-drain code. A magic user who spends more than 3 rounds in an Arasaka-owned system must make a **Wisdom save DC 13** at the end of the run. On a failure: they feel the drain. Not damaging — not yet. A sense of something pulling at the edges, like a sound heard in a dream. They lose one 1st-level spell slot that does not recover on a short rest. It recovers on a long rest. This is the network noticing them. File it.

---

## Sample Sequence — The Watson Node (Scene 3)

For reference: how the Scene 3 node run plays out under this system.

**Architecture (pre-built):**

```
[GATEWAY DC12] → [FILE DC10] → [SECURITY DC15 / Watchdog] → [FILE DC12] → [ROOT DC18]
```

The party needs nodes 2 and 4 (write their IDs, delete Splice's record). Node 3 is between them and has a Watchdog on a 4-minute sweep — which translates to **4 rounds** before it sweeps again.

**Default run path:**
- Round 1: Pass Gateway (Sleight of Hand or Investigation DC 12)
- Round 2: Interact with File 1 — write IDs (Investigation DC 10)
- Round 3: Handle Security — bypass Watchdog (Stealth, opposed) or neutralise it (attack roll)
- Round 4: Interact with File 2 — find and delete Splice's record (Investigation DC 14 to find it, DC 12 to delete)
- Round 5: Jack out

Total: 5 rounds, approximately 5 minutes of table time at a relaxed pace.

**If the Watchdog activates:** Clock advances to DETECTED. Security node DCs increase. The runner has roughly 3–4 more rounds before Trace triggers and a human admin is alerted. They can still complete the job — they just have less margin.

**Magic user path:** Can skip the Watchdog entirely by spending a 2nd-level slot on the Security node (Arcana check DC 13, advantage if 3rd-level slot). The Watchdog has no response pattern for what it's seeing. Clock does not advance.

---

## Scaling — Act 1 vs. Later Acts

### Act 1 (Fringe/Municipal Systems)
- 4–5 nodes
- ICE: Watchdog, Tar Pit at most
- Trace Clock moves slowly
- DCs 10–15
- 2–3 program slots sufficient

### Act 2 (Corp-Adjacent Systems)
- 6–8 nodes, branching paths
- ICE: Asp, Hellhound introduced
- Trace Clock moves faster
- DCs 13–17
- Program quality matters; magic users start encountering corruption risk

### Act 3 (Arasaka Core)
- 8–12 nodes, non-linear
- ICE: All types including Black Ice
- Trace Clock starts at DETECTED (they know someone is coming)
- DCs 15–20
- Soulkiller integration code is present — active threat to magic users
- The Archivist, if still active, may be able to assist from inside

---

## Quick Reference Card

```
ACTIONS PER ROUND: 2
  Move to adjacent node        (1 action)
  Interact with node           (1 action)
  Use program                  (1 action)
  Jack out                     (1 action, start of turn only)

NODE CHECKS:
  Bypass gateway/ICE stealth   DEX (Sleight of Hand)
  Read/copy/delete data        INT (Investigation)
  Fight ICE                    Attack roll (INT mod)
  Read a Daemon                WIS (Insight)
  Magic interface              INT (Arcana) — costs 2 actions, 1 spell slot

TRACE CLOCK: CLEAN → DETECTED → TRACED → BURN
  Advance: failed check (GM choice), Nuke, Watchdog sweep
  Roll back: Decoy, neutralise Security ICE, clean exit

ICE DAMAGE: psychic damage, real HP, CON save to resist
BODY GUARD: runner is unconscious/vulnerable while jacked in
CONCENTRATION: CON DC 10 + damage to stay in net when hit
```

---

*Updated as the system is playtested.*
