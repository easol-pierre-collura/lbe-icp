# LBE ICP: Helen vs Shan definition comparison

**Purpose:** help the team agree on one canonical LBE ICP definition by reviewing `definition-helen.md` and `definition-shan.md` in two ways:

- **Part A: Inconsistencies and differences.** Where the two files disagree, where a rule exists in only one file, and where a file contradicts itself.
- **Part B: Inference gaps.** Places where either file relies on context the agent (or a new reader) can't get from the text, so it has to guess.

The decisions needed to resolve both are in a separate file, `icp-decisions.md`, so they can be shared with the team.

**How to read this:** both files are built on the same base text: the same gate, the same taxonomy, the same eight shape-of-supply gaps (S1–S8) and the same CARR formula. Shan's file adds a layer of commercial prioritisation and stricter research rules. Helen's file has two extra instructions at the end. Line references are written as `H:` (Helen) and `S:` (Shan).

---

# Part A: Inconsistencies and differences across files

## 1. Summary

| Area | Helen | Shan | Type |
| --- | --- | --- | --- |
| Waiver handling | Flag for verification; not necessarily a dealbreaker | Forced waiver → exclude, unless it's the only gap and CARR ≥ $1m | **Conflict** |
| Ticketing partner source | Airscale first; for Strategic Opportunity rows, Airscale only | Confirm from the live booking journey; don't rely on Airscale | **Conflict** |
| Online booking requirement | Not required | Required for every bucket; enquiry-only businesses are excluded | **Conflict** |
| Immersive category (ASSESS) | "Experiential F&B & Narrative" | "Timed Immersive & Narrative"; F&B not required | **Conflict (scope)** |
| Excluded businesses in output | End of file: show them with reasons | Never shown | **Conflict** |
| Festivals / music | Disqualify | Not mentioned | **Helen only** |
| Outbound priority (P1–P4) | None | Full priority layer | **Shan only** |
| CARR floor for ASSESS types | None | $20k floor; $50k–$200k sweet spot | **Shan only** |
| Golf simulators | No rule | Socially led only; max 2 per 25-account batch | **Shan only** |
| Native app dependency | Not checked | Checked; lowers priority | **Shan only** |
| Seating, group enquiries | Not covered | PF8 and PF9: explicitly not concerns | **Shan only** |
| Output columns | 11 | 17 | **Shan only** |
| Performance feature labels | P1–P7 | PF1–PF9 | Naming |

---

## 2. Rules where the two files conflict

These rules can't both be true. Each one needs a decision.

### 2.1 Waivers (S6)
- **Helen** (`H:211`, `H:250-252`): waivers are flagged. In multi-activity venues, a waiver "is not necessarily a dealbreaker if waivers can be collected in-venue using a standalone tool. Flag it for verification."
- **Shan** (`S:316-322`, `S:372-374`): a forced online waiver, or a waiver clearly required before participation → **exclude**. The one exception is when the waiver is the only material gap and CARR ≥ $1m; then the business becomes Strategic Opportunity / P2. If a waiver is likely but not visible → Target — verify.
- **Impact:** a multi-activity venue with axe throwing and a required waiver is Target — verify under Helen and excluded under Shan.

### 2.2 Where the Current Ticketing Partner comes from
- **Helen** (`H:21`): "From Airscale if available, otherwise note what platform the booking flow runs on. For Strategic Opportunity rows, use Airscale value only — do not fetch the website for this."
- **Shan** (`S:37`, `S:248`, `S:418`): "Do not rely on Airscale if the booking journey shows a different platform." Record the booking URL checked and the evidence used.
- **Impact:** the two files reverse which source wins. Helen also bans fetching the website for Strategic Opportunity rows, while Shan requires a website check for them (see 2.3).

### 2.3 Online booking requirement
- **Helen:** no requirement. A Skip-type business with CARR ≥ $350k becomes Strategic Opportunity whatever its booking model (`H:29`, `H:139`).
- **Shan** (`S:52`, `S:216`, `S:250`, `S:423`): there must be a "clear online bookable journey" to be included at all, Strategic Opportunity included. Enquiry-only, "contact us" and quote-request businesses are excluded.
- **Impact:** a large business that only takes enquiries is a Strategic Opportunity under Helen and excluded under Shan.

### 2.4 Scope of the immersive ASSESS category
- **Helen** (`H:113`): **Experiential F&B & Narrative**: "Narrative/theme-wrapped experience, often with food or drink." Examples: Alcotraz, The Bletchley, Dans le Noir, murder mystery dinners.
- **Shan** (`S:184-186`): **Timed Immersive & Narrative Experiences**: "Narrative, theatrical, game-show, role-play, cinematic, themed or interactive experiences… Food and drink are… not required for this type." Examples: Taste Film, The Murder Express, The Traitors Live Experience, The Cube, Alcotraz.
- **Impact:** Shan's category is broader. Game shows, cinematic experiences and role-play without F&B are in scope under Shan, and arguably out of scope under Helen.

### 2.5 Whether excluded businesses appear in the output
- **Helen, end of file** (`H:295`): "When producing the final document present the qualified businesses AND disqualified businesses with reasoning as to why they failed."
- **Shan, and Helen's own main text** (`S:7`, `S:427-428`; `H:7`, `H:290-291`): "Excluded businesses do not appear in the output at all." "When a business is excluded… do not… write a summary… Move immediately to the next row."
- **Impact:** the two can't be done together. Logging reasons for exclusions needs at least a short reason per row, which goes against the "no further work" rule. See also 4.1.

---

## 3. Rules in only one file

These don't contradict the other file. The canonical version needs to decide whether to keep them.

### 3.1 In Shan's file only
| Rule | Where | Notes |
| --- | --- | --- |
| **Outbound priority:** P1 Quick Win, P1 Balanced, P2 Enterprise / Strategic, P3 Escape Room, P4 Below CARR Floor | `S:54-66`, `S:395`, `S:420` | Kept separate from the qualification bucket. Escape rooms default to P3. |
| **CARR thresholds:** < $20k not a new cold prospect; $20k–$50k only with strong signals; $50k–$200k sweet spot; > $200k P1 only if manageable | `S:68-75`, `S:421` | Helen has no CARR minimum for ASSESS types. |
| **No ceiling on target count**, "quality takes precedence over stopping at 150 companies" | `S:77` | Refers to a 150 figure that isn't explained anywhere. |
| **TTV** shown in the output, in source currency and USD | `S:33`, `S:83`, `S:106` | Helen only outputs CARR. |
| **Golf simulator handling** | `S:156`, `S:422` | Socially led only; practice-led businesses excluded from P1; max 2 per 25-account batch. |
| **Ticketing partner verification:** check the booking URL, footer, "powered by" text; look past the first landing page | `S:248`, `S:254`, `S:418` | Adds two columns: Booking URL Checked and Ticketing Partner Evidence. |
| **Online bookability check** | `S:250`, `S:423` | See 2.3. |
| **Native app dependency** | `S:267` | Said to "materially reduce outbound priority". |
| **PF8 Seating:** simple assigned seating is fine | `S:353` | |
| **PF9 Group / private-event enquiries:** fine if the core product is bookable online | `S:355` | |
| **Primary LBE Segment** column: lane/bay/resource, private room, timed immersive | `S:42` | These three segments aren't defined anywhere in the file (see 4.2). |
| **Included on Ismelka's List** column, plus a rule to treat that list as a source, not as qualification | `S:44`, `S:419` | Depends on an outside list that isn't in this repo. |
| **Skip-type research depth** allows checking bookability and ticketing partner | `S:216` | Helen allows only "what's needed for CARR estimation" (`H:139`). |

### 3.2 In Helen's file only
| Rule | Where | Notes |
| --- | --- | --- |
| **Disqualify festivals or music-related businesses** | `H:299` | Added at the end and not linked to any step. See 4.1. |
| **Show disqualified businesses with reasons** | `H:295` | See 2.5. |

### 3.3 Naming and formatting only
- Performance features are labelled **P1–P7** in Helen (`H:221-233`) and **PF1–PF9** in Shan (`S:339-355`). Helen's labels clash with Shan's outbound priorities P1–P4. If priorities are kept, keep the PF labels.
- Helen's output-columns table is broken: it's flattened into one paragraph (`H:21`). The section dividers (`---`) and quote blocks are missing, and the asterisks for italics are written as `&#x2A;` codes. This looks like a copy-paste from another tool and doesn't change the rules.

---

## 4. Inconsistencies inside each file

### 4.1 Inside Helen's file
1. **The end-of-file instructions contradict the main text.** "Show disqualified businesses with reasons" (`H:295`) clashes with `H:7`, `H:17`, `H:83`, `H:143`, `H:290` and `H:291`, which all say excluded rows are dropped with no further work.
2. **The festival/music rule has no defined scope.** It isn't attached to the gate (Step 1) or the taxonomy (Step 2). "Music related" is unclear: does it cover karaoke, music bingo, silent discos, immersive concerts or venues with live music? Karaoke is listed as a strong example in the support summary, so this rule could knock out targets the team wants.
3. **Strategic Opportunity research is impossible to follow.** `H:21` says not to fetch the website for the ticketing partner on Strategic Opportunity rows. But CARR estimation falls back to "what you can observe on the website" (`H:39`), and `H:139` allows fetching pages for CARR. So the website is both banned and needed for these rows.

### 4.2 Inside Shan's file
1. **The waiver exception sends businesses to a bucket they can't be in.** `S:320` routes a waiver business with CARR ≥ $1m to "Strategic Opportunity / P2". But Strategic Opportunity is defined only for **Skip** types with CARR above $350k (`S:52`, `S:393`). A waiver-only business in an ASSESS type, like a multi-activity venue, has no valid bucket under those definitions. The label also mixes a bucket and a priority.
2. **It's unclear what happens to ASSESS businesses below $20k CARR.** P4 is a priority (`S:66`), so these rows seem to stay in the output. But the same line says "do not add new cold prospects below the floor", which implies leaving them out. Step 5 (`S:378-395`) doesn't use CARR to exclude anyone. It needs to say clearly: excluded, or included as P4?
3. **The golf simulator quota is per batch, but the process is per row.** "No more than two simulator-led businesses" per 25-account batch (`S:156`) needs a count kept across the batch. That clashes with "process each business sequentially" (`S:116`) and with "do not create a fixed… ceiling; quality takes precedence" (`S:77`). It's also unclear whether practice-led simulator businesses are **excluded** or just **not P1**.
4. **Native app dependency has no defined effect.** It's collected (`S:267`) and said to "materially reduce outbound priority". No priority level or routing rule uses it.
5. **The Primary LBE Segment column has no definitions.** `S:42` lists three segments. Nothing in the file says how to map the taxonomy to them; for example, which segment a multi-activity venue or a room-based escape room falls under.
6. **A login wall clashes with the online-booking rule.** If the booking flow needs a login, `S:252` says Target — verify. But `S:250` requires a *confirmed* online bookable journey to include a business at all.
7. **Escape rooms vs large accounts.** Escape rooms "default to P3" and large slow-burn accounts "default to P2" (`S:395`). A large multi-site escape room chain (e.g. Escape Hunt, listed as an example at `S:176`) matches both defaults.
8. **"150 companies"** (`S:77`) refers to a target number that isn't explained anywhere.

### 4.3 In both files
1. **Airscale CARR: ignored, then used.** The trust policy lists the Airscale fields that can be used, and Estimated CARR isn't one of them (`H:13`, `S:15`). Yet the CARR divergence check compares the agent's figure with the Airscale Estimated CARR (`H:58`, `S:110`). The policy should list Airscale CARR as allowed, but only for this comparison.
2. **"Exceeds" vs "≥".** The Strategic Opportunity definition says CARR "exceeds $350,000" (`H:29`, `S:52`), while the routing rule says "≥ $350,000" (`H:139`, `S:216`). This only matters at exactly $350k, but the canonical version should pick one.
3. **Classes and workshops aren't covered.** The support summary excludes cooking classes and paint-and-sip. Neither definition says how to handle them; they aren't in the gate's fail list or the taxonomy.

---


# Part B: Inference gaps

These aren't disagreements between the files. They're places where **both** files (unless marked otherwise) rely on context that isn't written down. An agent following the rules has to fill these gaps from its own general knowledge, and different agents or readers will fill them differently. That makes results inconsistent even if Part A is fully resolved.

## 5. Inference gaps

### 5.1 Categories are defined by type, not at sub-vertical level
- The taxonomy (`H:93-131`, `S:150-208`) defines each **type**, e.g. "Single-Concept Venues", but never the **sub-vertical** above it. Nothing says what makes a business "Competitive Socialising" or "Immersive Experiences & Attractions" in the first place.
- **Impact:** a business that doesn't match a listed type has no rule for which sub-vertical it belongs to. Examples: interactive bingo, karaoke, or a game-show format that isn't immersive theatre.
- Shan's file adds a second grouping, the **Primary LBE Segment** column (`S:42`). It isn't defined in the file and doesn't map onto the taxonomy (see 4.2.5). "Table" games sit under Competitive Socialising, while "room" games sit under Escape Rooms, so a grouping like "Table / Room Games" would cut across both.

### 5.2 Named example businesses carry the definition
- Each type is explained mostly through brand names. There are about 35 in both files, e.g. Flight Club, Electric Shuffle, Bounce, Topgolf, NQ64, Fairgame and Five Iron Golf for Single-Concept Venues (`H:95`, `S:154`). Shan's file adds Taste Film, The Murder Express, The Traitors Live Experience and The Cube (`S:186`).
- **The files don't say what each example is meant to show.** To learn anything from "Flight Club", the agent has to already know how Flight Club takes bookings. It falls back on whatever it knows about these brands, which may be missing, out of date or wrong, especially for smaller or newer brands.
- **Unclear names.** "Bounce", "Daytona", "Fairgame" and "The Cube" could each refer to several different businesses.
- **Some examples are debatable.** Topgolf is an enterprise-scale chain listed as a Single-Concept Venue; Immersive Gamebox is listed under escape rooms.
- **Relationship to Easol isn't stated.** Nothing says whether the examples are Easol customers, prospects, competitors' customers or just familiar names.

### 5.3 No rule for existing Easol customers
- Neither file says what to do when a business in the input is already an Easol customer, or is under contract elsewhere. If Flight Club appears in the Experience Index, the agent would assess it as a new prospect.

### 5.4 Easol product terms are undefined
- The Easol limitation notes in S1–S8 (`H:201-215`, `S:289-333`) use product terms that are never defined: *variant*, *Extras*, *resource allocation*, *inventory*, *package*, *line item*, *shared stock*.
- Easol itself is only described as "an all-in-one platform for experience creators" (`H:3`, `S:3`).
- **Impact:** the agent can follow S1–S8 literally but can't reason about a booking model they don't cover, e.g. whether "core variant + Extras" can model a new format.

### 5.5 Data, lists and people that aren't provided
| Reference | File | What's missing |
| --- | --- | --- |
| Experience Index / Airscale | Both | Input format, field definitions, and how Airscale calculates its Estimated CARR |
| Ismelka's Fever account list | Shan (`S:44`, `S:419`) | The list itself, and who Ismelka is |
| "150 companies" | Shan (`S:77`) | Where this target comes from |
| "25-account discovery batch" | Shan (`S:156`) | The batch size isn't set anywhere else |
| "unless the user asks otherwise" | Shan (`S:156`) | Who "the user" is in an automated run |
| Known product gaps "for that type" | Both (`H:29`, `S:52`) | No list linking each SKIP type to its gaps for the Strategic Opportunity notes; the agent has to work them out from S1–S8 |
| `reference/current_lbe_icp_rulebook.md` | Summary | The file has been deleted |

### 5.6 Sales signals that aren't visible on public websites (Shan)
- P1 Quick Win depends on a "warm route into the account", an "owner-led buying group", an "active buying signal" and a "weak or fragmented current solution" (`S:58`, `S:64`).
- None of these can be seen on a public website, and no source such as a CRM export, warm-intro list or AE notes is provided. The agent will guess at P1 vs P3.

### 5.7 Terms, numbers and reasons that aren't explained
- **CARR, TTV and AE** are never spelled out.
- **Why 2.3%,** and whether the rate is the same in every market.
- **Currency conversion:** thresholds are in USD, while many examples are UK businesses. No rate or source is given; Shan's file only asks for the conversion to be shown (`S:106`).
- **No reasons for the thresholds:** $350k for Strategic Opportunity (both), $1m for the waiver exception and the $20k floor (Shan). Without the reasoning, nobody can judge edge cases.
- **Festivals / music (Helen, `H:299`):** no reason given, e.g. whether another Easol team covers them. That reason would define how far the rule reaches.

### 5.8 Tools and output the agent is assumed to have
- **A real browser:** the process asks the agent to pick a Friday 2–3 weeks out and work through the booking flow (`H:169`, `S:252`). A simple page fetch can't do that on JavaScript booking sites such as ROLLER or DesignMyNight.
- **Paid or registration-only sources:** Crunchbase and Companies House for reported revenue (`H:37`, `S:87`).
- **Ticketing platform knowledge:** the agent needs to recognise DesignMyNight, Fever, Bookeo, ROLLER, Booked It and others. Nothing says which are OTAs, competitors or neutral tools.
- **Output:** "a single spreadsheet", with no format, file location or template.
