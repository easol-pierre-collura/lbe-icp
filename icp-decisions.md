# LBE ICP: Decisions needed for a single canonical definition

**Purpose:** list the decisions the team needs to make to merge `definition-helen.md` and `definition-shan.md` into one canonical LBE ICP definition.

**Background:** the full analysis behind each decision is in `icp-definition-comparison.md`. Section references like "§2.1" point to that file.
- **Part A** of that file covers conflicts and differences between the two definitions. Decisions D1–D13 resolve them.
- **Part B** covers inference gaps: context that neither definition writes down. Decisions D14–D21 close them.

**How to use this:** each decision needs an owner to choose. The "If undecided" column gives a working default, not a recommendation for one author's version over the other's.

---

## 1. Resolving conflicts and differences (Part A)

| # | Decision | Context | Options | If undecided |
| --- | --- | --- | --- | --- |
| D1 | Waivers | Helen's file flags a required waiver for the AE to check. Shan's excludes the business unless the waiver is the only gap and CARR ≥ $1m. The same axe-throwing venue is "verify" under one and excluded under the other. (§2.1) | (a) Flag for verification (Helen) · (b) Exclude forced waivers, with the $1m exception (Shan) | (b), and fix the bucket issue in §4.2.1 |
| D2 | Ticketing partner source | Helen's file takes the ticketing partner from Airscale first. Shan's confirms it from the live booking journey and overrides Airscale when they disagree. (§2.2) | (a) Airscale first (Helen) · (b) Live booking journey first (Shan) | (b); it's evidence-based and doesn't conflict with CARR research |
| D3 | Online booking requirement | Shan's file excludes businesses that only take enquiries, Strategic Opportunities included. Helen's has no such rule, so a large enquiry-only business can still be a Strategic Opportunity. (§2.3) | (a) Not required · (b) Required for every bucket | (b) |
| D4 | Immersive scope | Helen's assessed immersive type is built around food and drink with a narrative. Shan's covers any timed narrative, game-show or interactive format, with food and drink optional. (§2.4) | (a) F&B-led (Helen) · (b) Any timed narrative/interactive format (Shan) | (b), plus a rule to tell standard shows, exhibitions and classes apart from immersive experiences |
| D5 | Excluded businesses in output | Both files say excluded businesses never appear in the output. A line added to the end of Helen's file asks for them to be shown with reasons. (§2.5, §4.1) | (a) Not shown (current main text in both files) · (b) A separate log with a one-line reason each | (b) as a **separate** exclusion log, keeping the AE list clean; reword the "no further work" rule to allow one line per exclusion |
| D6 | Festivals / music | Only Helen's file excludes festivals and music-related businesses. It doesn't say why, which step applies it, or whether karaoke and music bingo count. (§3.2, §4.1) | (a) Exclude at the gate, with a defined scope · (b) Don't add | If kept: define it as "festivals, concerts and music-event promoters" at Step 1, and state whether karaoke and music-led social formats are in or out |
| D7 | Outbound priority layer | Shan's file adds sales priorities (P1 Quick Win to P4 Below CARR Floor), separate from the qualification bucket. Helen's has none. (§3.1) | (a) Keep P1–P4 · (b) Leave it out of the ICP and keep it in a sales-process doc | Keep, but treat it as a separate step after qualification |
| D8 | CARR floor for ASSESS types | Helen's file has no minimum CARR for assessed types. Shan's sets a $20k floor and a $50k–$200k sweet spot, but doesn't say whether businesses below the floor are excluded or kept as P4. (§3.1, §4.2.2) | (a) None · (b) $20k floor, with the sub-floor routing defined | (b), and say clearly whether sub-floor rows are excluded or shown as P4 |
| D9 | Golf simulators | Only Shan's file has a rule: socially led simulators only, and at most two per 25-account batch. A per-batch quota doesn't fit a one-business-at-a-time process. (§3.1, §4.2.3) | (a) No rule · (b) Socially led only | (b), as a gate/taxonomy rule; drop the per-batch quota or move it to batch instructions |
| D10 | Native app dependency | Shan's file checks whether booking depends on a proprietary app and says it "materially reduces" priority, but never says to which priority. (§3.1, §4.2.4) | (a) Ignore · (b) Lower priority | If kept, say which priority it leads to |
| D11 | Primary LBE Segment | Shan's file adds an output column with three segments (lane/bay, private room, timed immersive) that aren't defined and don't map onto the taxonomy. (§4.2.5) | Define a mapping from taxonomy type to segment | Needed if the column is kept |
| D12 | Ismelka's List | Shan's file adds a column marking matches against Ismelka's Fever account list. The list isn't provided. (§3.1) | Keep the column only if that list is provided with the definition | — |
| D13 | Shared fixes | Small issues in both files: Airscale CARR is excluded by the data policy but then used in the divergence check; the $350k threshold is written as both "exceeds" and "≥"; classes and workshops aren't covered. (§4.3) | Allow Airscale CARR for the divergence check only; pick "≥" or ">" for $350k; decide on classes and workshops | Apply in the canonical version |

---

## 2. Closing inference gaps (Part B)

| # | Gap | Context | What to add to the canonical definition |
| --- | --- | --- | --- |
| D14 | Category scheme | Only the types are defined; sub-verticals like "Competitive Socialising" have no definition of their own. Shan's segment column adds a second, overlapping grouping. (§5.1) | Pick **one** top-level grouping (the shared sub-verticals or the three segments), write a one-paragraph definition for each sub-vertical, and add a rule for businesses that fit no listed type |
| D15 | Example businesses | About 35 brand names carry most of the category definitions, with no explanation. The agent has to rely on what it already knows about each brand, and some names are ambiguous. (§5.2) | For each example: a one-line reason ("why this is an example"), its booking model, and its status (Easol customer / prospect / other). Drop or clarify unclear names |
| D16 | Existing customers | Nothing says what to do when a business in the input is already an Easol customer. It would be assessed as a new prospect. (§5.3) | A rule for businesses that are already Easol customers, plus a source for the customer list |
| D17 | Easol product terms | The shape-of-supply gaps (S1–S8) use Easol terms such as variant, Extras and resource that are never defined. The agent can't reason about cases the list doesn't cover. (§5.4) | A short glossary of Easol product concepts (variant, Extras, resource, inventory, package) and how each kind of booking is modelled |
| D18 | Missing inputs | The definitions refer to data that isn't provided: Airscale field definitions, Ismelka's list, a "150 companies" target, a 25-account batch size, and the product gaps for each skipped type. (§5.5) | Attach or link the Airscale field list and Ismelka's list, or remove the rules that depend on them. Define batch size and the "150" target, or remove them. Write the gap list for each SKIP type |
| D19 | Sales signals | Shan's P1 rules depend on warm routes, buying signals and who makes the buying decision. None of these can be seen on a public website, and no data source is given. (§5.6) | Name a data source for warm routes and buying signals, or mark those fields as AE-completed and not agent-inferred |
| D20 | Terms and reasons | CARR, TTV and AE aren't spelled out. The 2.3% rate, the thresholds and the festivals rule have no stated reason, and there's no currency-conversion source. (§5.7) | Spell out CARR, TTV and AE; explain the 2.3% rate, each threshold and the festivals/music rule; set a currency-conversion source |
| D21 | Tools and output | The process assumes a real browser, paid revenue sources and knowledge of ticketing platforms, and gives no output format or template. (§5.8) | State the tools the agent needs (browser, revenue sources), list the known ticketing platforms by role, and give an output template |

---

## 3. Suggested next steps

1. Answer D1–D13 to remove the conflicts.
2. Fill in D14–D21 so the definition doesn't depend on outside knowledge. D14 and D15 matter most, because the taxonomy and its examples drive every categorisation.
3. Build the canonical file from **Shan's structure**, since it already includes almost every section in Helen's file. Apply the answers, keep Helen's festival/music rule and exclusion-log rule if they're approved, and fix the internal issues in §4 of the analysis.
4. Update `support-assets/LBE_EXPERIENCE_INDEX_ICP_SUMMARY.md` to match. It currently points to the deleted `current_lbe_icp_rulebook.md`.
