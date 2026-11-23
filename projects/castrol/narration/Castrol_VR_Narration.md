# Castrol in Mining: VR Narration

**Project:** VR Experience: Castrol in Mining
**Platform:** Meta Quest 3 (standalone, offline)
**Based on:** `proposal/Castrol_VR_Script.md` (Draft v0.1)
**Purpose:** The voice-over and subtitle master. Every spoken line in the experience, with its trigger, place in the game loop, delivery note and feedback cue, ready for client sign-off and VO recording.
**Status:** Draft v0.1, for M1 Scope sign-off

> **Placeholders.** Anything in `{CURLY BRACES}` needs a Castrol-approved name, figure or claim before recording (Proposal §8). Lines marked **NEW** are additions to the script (mostly reward and scorecard lines). Accept them here and they will be folded back into the script so voice-over and script stay identical (Proposal §10, Content).

---

## 1. Experience Concept & Game Premise

### Narrative premise and player role
The visitor is the **Site Reliability Lead**. They are handed a living mine and one mission: *find where friction is costing the site, and see how Castrol stops it.* Nothing on site moves until the visitor wakes it up. Every machine they inspect is a machine they "protect".

### Core gameplay loop (10–20 seconds per loop)

```
 PROMPT ──────▶ ACTION ──────▶ FEEDBACK ─────────▶ RESOLUTION
 Green glow     Point and       Casing dissolves,     Narrator names the win,
 + 1 line       select          haptic pulse, chime   check ring + score tick
     ▲                                                       │
     └──────────── next glowing thing appears ◀──────────────┘
```

The same loop drives the orb, the ground slider, the 7 mine components, the hotspots on each machine and the Standard/Castrol switch. Visitors learn it once in the first 20 seconds and then just repeat it, with bigger payoffs each time.

### Emotional payoff
*"I looked inside the hardest-working machines on Earth and saw exactly what keeps them alive."* The visitor leaves feeling expert, not sold to: smiling, a little awed, and holding a question to ask the Castrol team.

### Narration rules
| Rule | How it shows up |
|---|---|
| **Loop-shaped lines** | Each line has one job: *invite* (prompt), *react* (feedback) or *reward* (resolution). Never all three in one line. |
| **One to two sentences, max** | No line runs over about 6 seconds. |
| **Breathing room** | `[PAUSE]` = 3–5 seconds of ambient sound only. Never cut it. |
| **The visitor did it** | Reward lines credit the visitor: "you", "that was you". |
| **No failure lines** | Nobody is ever told they did something wrong. Hints redirect gently. |
| **Interruptible** | If the visitor acts mid-line, the prompt line fades out and the feedback line plays straight away. |

---

## 2. Voice Casting & Delivery Guide

| | |
|---|---|
| **Persona** | A seasoned site engineer who loves the machines. Walks beside the visitor, peer to peer. |
| **Voice** | Warm, mid-range, neutral international English. Gender open. |
| **Pace** | About 140 words per minute. Slower and quieter for hero moments, brighter for rewards. |
| **Avoid** | Announcer energy, "ad read" cadence, upward sales inflection, technical lecturing. |
| **Reference feel** | A documentary host who has just seen something cool and wants you to see it too. |
| **Recording notes** | Record every line dry (no reverb), 48 kHz / 24-bit WAV, one file per Line ID. Spatial reverb is added in engine per environment (studio, control room, mill house, open pit). Record 2 takes of every reward line: one warm and one more excited. Runtime picks randomly so repeat loops don't sound canned. |

**Delivery tags used below:** `[warm]` `[curious]` `[hushed]` `[awed]` `[bright]` `[confident]` `[focused]` `[playful]` `[gentle]` `[thrilled]`

---

## 3. Narration by Level

**Column key**
- **ID:** file name and subtitle key.
- **Trigger:** what makes the line play.
- **Loop:** P = Prompt, F = Feedback, R = Resolution.
- **Juice cue:** the sound, haptic or visual that lands *with* the line.

---

### LEVEL 1: Invisible Tutorial & First Win (0:00–0:20)
*Setting: dark studio, green horizon line, one floating green orb.*

| ID | Trigger | Loop | Delivery | Line | Juice cue |
|---|---|---|---|---|---|
| `L1-01` | Session start, after 2 sec | — | `[warm, unhurried]` | "Welcome. Take a second and look around. There's no rush." | Ambient pad fades in. Horizon line draws left to right. |
| `L1-02` | 4 sec after L1-01 | P | `[warm]` | "See that green light in front of you? Point at it and squeeze the trigger." | Orb pulses. Haptic tick on hover. |
| `L1-03` | Orb selected | R | `[delighted]` | "Perfect. That's all you'll need today." | Orb bursts into green particles, firm haptic pulse, rising chime. |
| `L1-04` | 1.5 sec after L1-03 | P | `[warm]` | "Anything that glows green, you can explore." | Castrol wordmark resolves from the particles. |

**Hints (idle 8 sec after L1-02; each plays once):**

| ID | Line | Juice cue |
|---|---|---|
| `L1-H1` | `[gentle]` "Take your time. Whenever you're ready, point at the glowing light and squeeze your index finger." | Orb pulses brighter. |
| `L1-H2` | `[gentle]` "Your pointer finger, on the trigger at the back of the controller. That's the one." | Orb drifts closer. Ghost hand shows the trigger pull. |
| `L1-H3` | `[gentle]` "Our team is right beside you if you'd like a hand. Just say so." | Booth tablet alert. |

---

### LEVEL 2A: Why Castrol (0:20–2:00)
*Setting: dark cinema space with two floating video panels, Formula 1 and Space.*

| ID | Trigger | Loop | Delivery | Line | Juice cue |
|---|---|---|---|---|---|
| `L2A-01` | Panels appear | P | `[curious]` | "Before we go underground, let's start somewhere just as tough. Pick one: the racetrack or orbit." | Both panels pulse green. Engine rev on one side, rocket rumble on the other. |
| `L2A-02` | F1 panel selected (or auto after 10 sec) | F | `[playful]` | "Good pick. Hold on." | Panel expands to fill the view. Revs climb. |
| `L2A-03` | F1 video, 3 sec in | — | `[low, intense]` | "Twenty-odd laps of pure punishment. Thousands of gear changes, heat that would cook most oils." | Engine roar in spatial audio. |
| `L2A-04` | F1 freeze-frame moment | — | `[hushed]` | "Every one of those shifts depends on a film of oil thinner than a hair." | Time slows. Green trace runs along the gear teeth. Revs drop to a hum. |
| `L2A-05` | After L2A-04 + `[PAUSE]` | R | `[warm, confident]` | "{APPROVED F1 CLAIM}." | Subtle chime. |
| `L2A-06` | Space panel selected | F | `[playful]` | "Going up. Let's go." | Panel expands. Low rumble, then silence. |
| `L2A-07` | Space video, 3 sec in | — | `[awed, quieter]` | "Out here there's no second chance and no service crew." | Temperature readout swings between extremes. |
| `L2A-08` | After L2A-07 + `[PAUSE]` | R | `[warm, confident]` | "{APPROVED SPACE CLAIM}." | Soft mechanical click. |
| `L2A-09` | First example ends | P | `[curious]` | "Want to see the other one? Or shall we keep going?" **NEW** | Second panel pulses. A "Continue" orb appears. |
| `L2A-10` | Both seen, or Continue | — | `[leaning in]` | "Racetracks. Orbit. And one more place that asks just as much of every machine…" | Panels fold into one green line. |
| `L2A-11` | Portal opens | P | `[smiling]` | "…a mine. Step into the green. Your site's waiting." | Floor portal swirls with rock dust and distant machinery. |
| `L2A-12` | Visitor enters portal | R | `[bright]` | "Here we go." **NEW** | Long warm haptic rumble. Under 3 sec transition. |

---

### LEVEL 2B: The Core Mechanic, Tabletop Mine (2:00–5:00)
*Setting: warm control room. A round table holds a living scale model of the mine with transparent ground, a green slider and 7 glowing components.*

#### Arrival and the slider

| ID | Trigger | Loop | Delivery | Line | Juice cue |
|---|---|---|---|---|---|
| `L2B-01` | Scene loads | — | `[warm, proud]` | "This is your mine. All of it, from the haul roads up top to the tunnels underneath." | Machines wake in a ripple from the centre out. Miniature diesel and conveyor hum. |
| `L2B-02` | After L2B-01 + `[PAUSE]` | P | `[warm]` | "Go ahead, walk around it. Lean in close." | Ambient detail: dust, tiny reversing beepers. |
| `L2B-03` | 6 sec after L2B-02 | P | `[curious]` | "There's a green slider on the edge of the table. Slide it, and look what's happening under your feet." | Slider pulses. Haptic tick on hover. |
| `L2B-04` | Slider moved past 50% | R | `[impressed]` | "That's the half of the mine nobody sees. You just did." | Ground fades to glass. Tunnels light up. LHD headlights sweep. Rumble rises from under the table. |
| `L2B-05` | 2 sec after L2B-04 | P | `[warm]` | "Every glowing machine has a story. Point at one, pick it up, and I'll tell you what it's up against." | All 7 components pulse once in a sweep around the table. |

#### Component cards (any order)
Each card is one micro-loop: **select → F line (problem) → `[PAUSE 2s]` → R line (Castrol answer) → check ring and "+1 Protected" tick.**

| ID | Component | Loop | Delivery | Line | Juice cue |
|---|---|---|---|---|---|
| `L2B-EX-F` | Excavator | F | `[engaged]` | "Everything starts here. If this digger stops, the whole mine waits." | Miniature lifts and rotates. Tiny bucket scoops. Reference clip plays. |
| `L2B-EX-R` | | R | `[confident]` | "Castrol keeps its hydraulics and slew gears protected through heavy shock loads, shift after shift. {PRODUCT NAME}." | Green sheen washes over the model. Check ring and chime. |
| `L2B-ST-F` | Surface mining truck | F | `[engaged]` | "These trucks never really stop: hot engines, steep ramps, round the clock." | Engine heat shimmer on the miniature. |
| `L2B-ST-R` | | R | `[confident]` | "Castrol engine oil keeps them running longer between services. {PRODUCT NAME}. We'll take a closer look inside one shortly." | Green sheen. Check ring. |
| `L2B-WL-F` | Wheel loader | F | `[engaged]` | "Thousands of stop-start cycles a day. That's brutal on transmissions." | Loader rocks back and forth. |
| `L2B-WL-R` | | R | `[confident]` | "Castrol transmission and axle fluids keep every cycle smooth. {PRODUCT NAME}." | Green sheen. Check ring. |
| `L2B-CR-F` | Crusher | F | `[playful, then serious]` | "Feel that? Every rock is a hammer blow on the bearings." | Haptic thud with each crush. |
| `L2B-CR-R` | | R | `[confident]` | "Castrol greases hold their film under that shock, so bearings last. {PRODUCT NAME}." | Thuds soften to a smooth pulse. Check ring. |
| `L2B-CB-F` | Conveyor belt | F | `[engaged]` | "Hundreds of rollers and gearboxes, all in the dust and the weather." | Belt speeds past. Dust swirl. |
| `L2B-CB-R` | | R | `[confident]` | "Castrol keeps them sealed and turning, so the ore keeps flowing. {PRODUCT NAME}." | Green light travels along the belt. Check ring. |
| `L2B-ML-F` | Mill | F | `[engaged]` | "This is where rock becomes value, and it spins day and night." | Drum turns. Low rumble. |
| `L2B-ML-R` | | R | `[curious, inviting]` | "Its giant gears rely on Castrol grease. {PRODUCT NAME}. Want to see inside? It's one of our case studies." | Green sheen. Check ring. Case-study pedestal flickers. |
| `L2B-LH-F` | Load haul dump (LHD) | F | `[hushed, closer]` | "Down here it's hot, tight and dusty, and there's nowhere to hide a breakdown." | Headlights in the tunnel. Echoing engine. |
| `L2B-LH-R` | | R | `[confident]` | "Castrol keeps underground fleets moving where downtime costs the most. {PRODUCT NAME}." | Tunnel glows green. Check ring. |

#### Progress rewards (NEW)

| ID | Trigger | Delivery | Line | Juice cue |
|---|---|---|---|---|
| `L2B-P1` | 3rd component visited | `[bright]` | "Three down. You're getting a feel for this place." | Rising three-note chime. |
| `L2B-P2` | All 7 visited | `[thrilled]` | "Every machine on site. That's the whole mine, and you've seen it all." | Green ripple across the entire table. Long warm haptic. "Site Mapped" badge floats up. |

#### Bridge to case studies

| ID | Trigger | Loop | Delivery | Line | Juice cue |
|---|---|---|---|---|---|
| `L2B-10` | 3+ components visited, or 2:30 elapsed | R | `[pleased]` | "You've just walked the whole site in a couple of minutes. Not bad." | Three hero machines glow brighter. Chime. |
| `L2B-11` | After L2B-10 + `[PAUSE]` | P | `[warm, leaning in]` | "Now, three of these machines have a story we'd love to show you up close. From the inside." | Three green pedestals rise. |
| `L2B-12` | 3 sec after L2B-11 | P | `[warm]` | "Pick one. Haul truck, ball mill or face shovel. Don't worry, you can come back for the others." | Pedestals pulse in turn. |

**Hints (idle 8 sec):**

| ID | Line | Juice cue |
|---|---|---|
| `L2B-H1` | `[gentle]` "Try pointing at anything glowing on the table. The truck on the ramp is a good place to start." | Haul truck pulses. |
| `L2B-H2` | `[playful]` "That one's waving at you." | Haul truck pulses brighter and its headlights flash twice. |
| `L2B-H3` | `[gentle]` "The green slider on the table edge shows you what's underground." *(if slider unused)* | Slider pulses. |

---

### LEVEL 3: The "Boss Moment", Inside the Machines (about 2 min each)
*Each case study runs the same flow: Scale → Hotspots → **Hologram (hero moment)** → Proof → Standard/Castrol switch (optional) → Return.*
*The switch is the "boss moment": the visitor puts the machine under stress and personally flips it from wear to protection.*

#### 3A: Haul Truck *(engine oil)*
*Setting: life-size haul truck on a dusty ramp at golden hour.*

| ID | Trigger | Loop | Delivery | Line | Juice cue |
|---|---|---|---|---|---|
| `L3A-01` | Scene loads | — | `[impressed, hushed]` | "Look up. Way up." | Deep diesel idle. Haptic tremor. Dust in the light. |
| `L3A-02` | After L3A-01 + `[PAUSE]` | P | `[warm]` | "This truck carries {PAYLOAD} a trip, all day, every day. Take a walk around her." | Truck rumbles. |
| `L3A-03` | Hotspots ignite | P | `[curious]` | "See those green points? That's where the real work happens. Pick one." | Three hotspots ignite with a rising chime. |
| `L3A-04` | Hotspot: Pistons & liners | F | `[focused]` | "Every second, these pistons fire again and again, at temperatures that break ordinary oil down into sludge." | **HERO:** casing dissolves into green light. Pistons fire in slow motion. Heat shimmer. Engine hum drops to a heartbeat. |
| `L3A-05` | After L3A-04 + `[PAUSE]` | R | `[confident]` | "Castrol holds its strength in that heat, so the engine stays clean and protected." | Shimmer cools to green. Firm haptic. Hotspot check. |
| `L3A-06` | Hotspot: Turbocharger | F | `[focused]` | "This turbo spins faster than a jet engine and runs almost as hot." | Turbo spins up with a rising whine. Red-hot shaft. |
| `L3A-07` | After L3A-06 | R | `[confident]` | "Castrol keeps a film on that shaft so it doesn't cook." | Shaft glow shifts red to green. Check. |
| `L3A-08` | Hotspot: Crankshaft bearings | F | `[hushed]` | "That green line is everything." | Zoom to bearing. Thin green oil ribbon. |
| `L3A-09` | After L3A-08 | R | `[soft, confident]` | "It's the only thing between metal and metal." | Ribbon pulses once. Check. |
| `L3A-10` | 2+ hotspots done | R | `[warm, confident]` | "Here's what that meant for a real fleet: {APPROVED HAUL TRUCK PROOF POINT}." | Proof card unfolds. "Lock-in" chime. Haptic pulse. |
| `L3A-11` | After L3A-10 + `[PAUSE]` | R | `[bright]` | "That's more hours hauling and fewer in the workshop." | — |
| `L3A-12` | Switch appears *(optional)* | P | `[playful]` | "Want to see the difference? Flip the switch." | Green switch pulses. |
| `L3A-13` | Switched to Standard | F | `[concerned]` | "Hear that? That's wear, happening right now." **NEW** | Flow darkens and slows. Sparks at bearings. Rough grinding haptic. |
| `L3A-14` | Switched to Castrol | R | `[relieved, warm]` | "Hear how that settles? That's what protection sounds like." | Flow runs bright green. Grinding melts into a smooth hum. Long warm haptic. |
| `L3A-15` | Return | R | `[bright]` | "One down. Where to next?" | Truck shrinks to tabletop. Pedestal check ring. "+1 Machine Protected". |

#### 3B: Fixed Plant Ball Mill *(grease)*
*Setting: inside the mill house, beside a rotating drum and a girth gear taller than a building.*

| ID | Trigger | Loop | Delivery | Line | Juice cue |
|---|---|---|---|---|---|
| `L3B-01` | Scene loads | — | `[over the noise, then settling]` | "Feel that? That's tonnes of steel tumbling inside, grinding rock to powder." | Cascading balls in spatial audio. Steady haptic vibration. |
| `L3B-02` | After L3B-01 + `[PAUSE]` | — | `[warm]` | "This mill doesn't stop for weekends." | — |
| `L3B-03` | Hotspots ignite | P | `[curious]` | "Two places carry the whole load. Pick one." | Hotspots on the girth gear and trunnion. |
| `L3B-04` | Hotspot: Girth gear & pinion | F | `[fascinated]` | "This is an open gear, exposed to dust and grit, with massive pressure on every tooth." | **HERO:** gear guard dissolves. Teeth mesh in slow motion. Grit particles drift. |
| `L3B-05` | After L3B-04 + `[PAUSE]` | R | `[confident]` | "Castrol grease clings to those teeth and won't let go, even under that pressure. {PRODUCT NAME}." | Green grease film stretches between the teeth. Firm haptic. Check. |
| `L3B-06` | Hotspot: Trunnion bearings | F | `[awed]` | "The entire mill rests right here. Imagine carrying that, forever." | Load indicator glows on the bearing. |
| `L3B-07` | After L3B-06 | R | `[confident]` | "Castrol keeps it rolling." | Bearing glows green. Check. |
| `L3B-08` | Both hotspots done | R | `[confident]` | "At a real plant, that meant {APPROVED BALL MILL PROOF POINT}." | Proof card and lock-in chime. |
| `L3B-09` | After L3B-08 + `[PAUSE]` | R | `[bright]` | "A mill that keeps turning is a plant that keeps earning." | — |
| `L3B-10` | Switch appears *(optional)* | P | `[playful]` | "Flip it. Watch what happens to the teeth." | Switch pulses. |
| `L3B-11` | Switched to Standard | F | `[concerned]` | "See the teeth heating up? That's metal touching metal." **NEW** | Grease thins and flings off. Teeth glow orange. Grinding haptic. |
| `L3B-12` | Switched to Castrol | R | `[relieved, warm]` | "Same gear. Very different day." | Film evens out green. Contact cools. Smooth haptic. |
| `L3B-13` | Return (shovel not yet visited) | R | `[bright]` | "Nice work. Want to see the shovel?" | Mill folds to tabletop. Check ring. "+1 Machine Protected". |
| `L3B-13b` | Return (all visited) | R | `[bright]` | "Nice work. That's another one protected." **NEW** | As above. |

#### 3C: Face Shovel *(grease)*
*Setting: open pit face, with a huge shovel towering overhead.*

| ID | Trigger | Loop | Delivery | Line | Juice cue |
|---|---|---|---|---|---|
| `L3C-01` | Shovel takes a bite | — | `[thrilled]` | "Whoa. Did you feel that?" | Crunch, falling rubble, strong haptic thud. |
| `L3C-02` | After L3C-01 + `[PAUSE]` | — | `[engaged]` | "Every bite moves {BUCKET PAYLOAD}. And every bite sends a shock through the whole machine." | Second, softer bite. |
| `L3C-03` | Hotspots ignite | P | `[curious]` | "Let's find out where that shock goes. Pick a point." | Hotspots on the slew ring and boom pins. |
| `L3C-04` | Hotspot: Swing gear / slew ring | F | `[engaged]` | "Every time the shovel swings to the truck, this ring takes the whole weight, back and forth, thousands of times a shift." | **HERO:** upper casing dissolves. Ring rotates as the shovel swings. |
| `L3C-05` | After L3C-04 + `[PAUSE]` | R | `[confident]` | "Castrol grease cushions every swing. {PRODUCT NAME}." | Green film glows on the ring. Firm haptic. Check. |
| `L3C-06` | Hotspot: Boom pins & bushings | F | `[rhythmic, playful]` | "Shock, shock, shock." | Shock rings pulse outward with each bite, in sync with haptic thuds. |
| `L3C-07` | After L3C-06 | R | `[soft, confident]` | "And this tiny layer soaks it up." | Green film absorbs the rings. Thuds soften. Check. |
| `L3C-08` | Both hotspots done | R | `[confident]` | "On a real site: {APPROVED FACE SHOVEL PROOF POINT}." | Proof card and lock-in chime. |
| `L3C-09` | After L3C-08 + `[PAUSE]` | R | `[bright]` | "That's a shovel that's digging, not waiting for parts." | — |
| `L3C-10` | Switch appears *(optional)* | P | `[playful]` | "Go on, flip it." | Switch pulses. |
| `L3C-11` | Switched to Standard | F | `[concerned]` | "The film's breaking. Feel how rough that is?" **NEW** | Sparks. Harsh haptic. |
| `L3C-12` | Switched to Castrol | R | `[proud]` | "That's the difference you just made." | Film holds and the swing glides. Long warm haptic. |
| `L3C-13` | Return (all 3 done) | R | `[warm, celebratory]` | "That's all three. You've seen inside the hardest-working machines on site." | Shovel to tabletop. All three pedestals glow. Rising chord. |
| `L3C-13b` | Return (others remaining) | R | `[bright]` | "One more protected. Where to next?" **NEW** | Check ring. |

**Case-study hints (idle 8 sec, shared across all three):**

| ID | Trigger | Line | Juice cue |
|---|---|---|---|
| `L3-H1` | Idle at hotspot step | `[gentle]` "Try one of the green points on the machine. Any one is a good place to start." | Hotspots pulse. |
| `L3-H2` | Still idle | `[gentle]` "This one, right here." | Nearest hotspot pulses larger. Ghost pointer. |
| `L3-H3` | Idle at switch | `[playful]` "That green switch is all yours. Give it a flip." | Switch pulses. |
| `L3-H4` | Idle at return | `[gentle]` "Whenever you're ready, point at 'Back to the mine' and we'll pick the next one." | Return button pulses. |

---

### LEVEL 4: Victory State & Real-World Bridge (30 sec)
*Setting: back at the tabletop mine. Visited machines wear check rings, and the whole site glows green.*

| ID | Trigger | Loop | Delivery | Line | Juice cue |
|---|---|---|---|---|---|
| `L4-01` | Closing starts | R | `[warm, genuinely pleased]` | "Look at that. From the racetrack to the rock face, you found where friction hides, and you saw how Castrol stops it." | Green ripples out from each visited machine. Machines run faster and smoother. Musical lift. Long warm haptic. |
| `L4-02` | Scorecard appears **NEW** | R | `[bright, proud]` | "Here's your site report." | **Site Reliability Report** card: *Mine components explored: {n}/7 · Machines protected: {n}/3 · Switches flipped: {n}*. Each counter ticks up with a chime. |
| `L4-03` | After scorecard | R | `[confident, simple]` | "Less wear. Fewer stoppages. More tonnes moved." | Summary card: **"Castrol: keeping your mine moving, from the pit to the plant."** *(to be approved)* |
| `L4-04` | After L4-03 + `[PAUSE]` | P | `[bright, inviting]` | "The Castrol team right next to you has the full story behind what you just saw." | Contact card and QR code. "Session complete" banner on the booth screen. |
| `L4-05` | 1.5 sec after L4-04 | P | `[warm, smiling]` | "Take off the headset and ask them: 'What could this do for my site?'" | Soft outro chord. Scene fades to the start screen within 10 sec of headset removal. |

**Scorecard variants for L4-02** (picked by game state, so there's always a reason to celebrate):

| ID | Condition | Line |
|---|---|---|
| `L4-02a` | All 7 components and all 3 machines | `[thrilled]` "Full site, every machine. That's a perfect inspection." |
| `L4-02b` | 1–2 machines explored | `[bright]` "Great inspection. And there's more waiting inside if you want to come back." |
| `L4-02c` | Express path | `[bright]` "Quick, sharp, and you went straight to the engine. Nicely done." |

---

## 4. Express Path (90 sec to 3 min)

Staff select the express tier on the tablet. The runtime plays this subset only:

`L1-01 → L1-02 → L1-03 → L2A-01 → (one example) → L2A-10 → L2A-11 → L2B-01 → L2B-03 → L2B-04 → L2B-05 → (1 component) → L2B-12 → L3A-03 → L3A-04 → L3A-05 → L3A-10 → L3A-14 → L4-01 → L4-02c → L4-04 → L4-05`

In the express path, the haul truck opens with the switch already set to Standard, so a single flip to Castrol (L3A-14) delivers the boss moment.

---

## 5. Booth Staff ("Game Master") Triggered Lines

Lines the tablet can fire into the headset on demand. They are recorded in the same voice so they never break immersion.

| ID | Tablet button | Line |
|---|---|---|
| `GM-01` | **Nudge** | `[gentle]` "Have a look around. There's something glowing just for you." |
| `GM-02` | **Look left** / **Look right** | `[gentle]` "Over to your left." / "Over to your right." *(with a spatial chime from that side)* |
| `GM-03` | **Suggest truck** | `[warm]` "The haul truck's a great one to start with. It's all about the engine." |
| `GM-04` | **Suggest mill** | `[warm]` "If you work in processing, the ball mill is calling your name." |
| `GM-05` | **Suggest shovel** | `[warm]` "Want to feel some real power? Try the face shovel." |
| `GM-06` | **Wrap up** | `[warm]` "Let's head back to the mine for one last look." *(jumps to Level 4)* |
| `GM-07` | **Pause** | `[gentle]` "Let's take a breather. Lift the headset any time you like." *(fades to calm studio)* |
| `GM-08` | **Resume** | `[warm]` "Welcome back. Let's pick up where we left off." |

---

## 6. Live Handoff Line (booth staff, spoken outside the headset)

When the "session complete" banner appears, the staff member reads the visitor's path from the cast screen and opens with:

> *"Welcome back! I saw you spent time on the {LAST CASE STUDY}. What machines are you running on your site today?"*

If the visitor flipped every switch:

> *"You flipped every switch in there. Want to see the real numbers behind those results?"*

---

## 7. Line Inventory & Recording Checklist

| Level | Core lines | Hints / variants | GM lines |
|---|---|---|---|
| L1: Onboarding | 4 | 3 | — |
| L2A: Why Castrol | 12 | — | — |
| L2B: Tabletop mine | 24 | 3 | — |
| L3A: Haul truck | 15 | 4 *(shared L3-H)* | — |
| L3B: Ball mill | 14 | — | — |
| L3C: Face shovel | 14 | — | — |
| L4: Closing | 5 | 3 | — |
| Booth staff | — | — | 9 |
| **Total** | **88** | **13** | **9** |

*Totals count each L4-02 variant once and each GM-02 direction separately. With 2 takes per reward line, plan for about 150 audio files.*

**Before recording:**
- [ ] All `{PLACEHOLDERS}` replaced with Castrol-approved text (Proposal §8)
- [ ] **NEW** lines accepted and folded back into `proposal/Castrol_VR_Script.md`
- [ ] Hotspot list per machine confirmed (affects L3A/B/C line set)
- [ ] Payload and bucket figures confirmed or lines trimmed (`L3A-02`, `L3C-02`)
- [ ] Closing tagline approved (`L4-03` card)
- [ ] Voice talent selected and a 3-line test read approved (`L1-02`, `L3A-04`, `L4-05`)
- [ ] Castrol sign-off on this narration document
