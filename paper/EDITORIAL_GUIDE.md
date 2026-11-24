# Editorial brief — Alpöge mathematical monograph

**Status:** Governing editorial constitution and continuity protocol, revised 21 November 2026  
**Text examined:** `From_Multiplicity_to_the_Critical_Line.tex` (1,538 source lines), compared with `structural_reductions_lean_rh.tex` (367 source lines). Line references below point to the 1,538-line draft as inspected; they will change after edits.

## The voice to use, consistently

Write as **a patient working mathematician teaching another interested human being**: knowledgeable, measured, curious, precise, and unselfconscious. The reader should feel that the author is following a mathematical thought, not performing an act of exposition. Good sentences identify an object, explain its behavior, derive a consequence, and tell the reader why that consequence matters. They do not repeatedly announce that mathematics is beautiful or that the book is teaching insight.

Favor the restrained, direct style of the earlier *Structural Reductions* paper, combined with the readable development of the seven-page sample. Use natural paragraph-to-paragraph transitions; let the mathematical problem itself determine the pacing. **No faux-authorial personality, no motivational monologue, no cleverness for its own sake.** Never imitate a named mathematician's idiosyncratic prose.

## Concrete AI-writing mannerisms found in the longer manuscript

| Pattern | Existing manuscript evidence (LaTeX source line) | Revision decision |
|---|---|---|
| **1. Aphoristic throat-clearing** | L80, “A mathematical proof has at least two lives.” The paragraph then develops this contrived parallel for several sentences. | Delete. Introduce the mathematical purpose and the exact source-status in ordinary prose. |
| **2. Invented slogans instead of explanation** | L82, “The correct unit of exposition is therefore not a file, a theorem name, or even a mathematical subject. It is a *difficulty overcome*.” | Describe what the chapter will actually explain. Avoid announcing a proprietary philosophy of mathematical writing. |
| **3. Rhetorical self-questioning** | L84, “We shall return repeatedly to five questions.” Followed by five staged questions. | Ask a question only when the next calculation genuinely answers it. Usually state the problem directly. |
| **4. Over-clever titles / anthropomorphism** | L493, “The prime sum that can hear a zero”; L872, “Divisibility is the shadow of a norm inequality”; L1347, “Why automorphic forms have Galois shadows”; L117, “The line as a boundary, not a destination.” | Retitle by mathematical content: “A weighted prime sum and its Mellin transform”; “Divisibility and archimedean bounds”; “Automorphic and Galois representations”; “Zero-freeness and functional-equation symmetry.” |
| **5. Forced antithesis: ‘not X, but Y’** | L245, “The point is not that the character … It is that…”; L350, “It is this imbalance, not merely the act of differentiation…”; L479, “These are not decorations attached to the central idea…” | State the positive mathematical claim. Use contrast only when it prevents a specific mathematical misunderstanding. |
| **6. Narrating the writing process** | L481, “Where the next chapters must go”; L486, “What has actually been established so far?”; L1508, “The economy of a good explanation”; L1516, “An invitation to the underlying mathematics.” | Remove from the main mathematical narrative. Keep one concise scope note and, if needed, an end-of-chapter statement of exact remaining hypotheses. |
| **7. Inflated emphasis** | L312, “An elementary inequality with enormous reach”; L364, “The striking identity”; L968, “The striking detail”; L1297, “This is perhaps the most satisfying small calculation”; L1407, “The two arithmetic branches meet here.” | Let the displayed equation and its consequence produce interest. Describe an identity as striking only if the next sentences make clear *what mathematical obstruction it removes*. |
| **8. Faux depth, often with vague nouns** | L1442, “The central question is not whether any one of those tools is powerful”; L1518, “The spectacular geometry enters only because such an inequality seems unavailable…” | Replace with named hypotheses, estimates, and consequences. Terms such as *machinery*, *bridge*, *engine*, *payoff*, and *architecture* are not replacements for mathematics. |
| **9. A textbook of signposts rather than a coherent essay** | L386, “We now turn from…”; L481–489, explicit description of the chapters to come; L1222, “We have now introduced all the main ingredients…” | Transition through a mathematical dependency instead: “The previous estimate depends on an archimedean norm bound. We next obtain one from…” |
| **10. Repeated defensive epistemic disclaimers in the body** | L414, L481–489, L647, L1006, L1216, L1341 revisit what is unproved, often at length. | **Keep the cautions, change their location.** Put verification status once in front matter, precise conditional hypotheses in theorem statements, and focused notes where a proof gap actually affects a claim. Do not disguise uncertainty, but do not interrupt each paragraph to apologize for it. |
| **11. Generic analogies that are not yet mathematical reductions** | L473–479 posits abstract gain $G(m)$ and cost $C(m)$, then admits no exact definitions; L414 presents a polynomial gcd picture that cannot, without more, stand in for representation subtraction. | Use an analogy only if the relevant map of objects, invariant, and limitations is concrete. Otherwise cut and replace it with the actual source-defined quantities. |
| **12. Announcing beauty instead of allowing discovery** | L80, L1297, L1516 and other reflective passages comment on how illuminating the material is. | Show why a normalization cancels, why disjoint characters permit a subtraction, or why the ramp transform has a simple pole structure. The reader will supply the appreciation. |

## What to preserve and expand

1. **Mathematics first.** Start sections with a concrete task, a definition, an example, or a specific obstruction—not a description of the book's intentions.
2. **Continuity.** Each construction should answer a problem established in the preceding pages. Follow the objects and dependencies, not the Lean directory names.
3. **Proof discipline.** Prove elementary and accessible implications in full. State deeper imported results with exact hypotheses, source links, and verification status; do not call a suggestive model a proof of the corresponding source theorem.
4. **Exposition over transcript.** Ignore notation-management, typeclass scaffolding, and proof-assistant bookkeeping unless mathematically decisive. Retain the numerical exponents, ranges, and nonvanishing conditions that make the argument work.
5. **Illustrations as mathematical arguments.** Draw a figure only when it makes a transformation, cancellation, scope restriction, or dependency visually comprehensible. Captions should say what is represented and what is *not* asserted. Avoid generic flowcharts and decorative images.
6. **Alpöge's own voice.** Insert brief, exact, page-referenced quotations from `remark.pdf` *where the quoted remark illuminates the construction under discussion*—not as epigraphs or mood-setters. Explain the mathematics after the quote, and check the account against the Lean statements. Quote sparingly, with attribution and source page.
7. **Unforced style.** Permit variation in sentence length. Favor plain verbs (“implies,” “forces,” “factors,” “reflects,” “bounds”) over grand adjectives. A well-chosen informal sentence is welcome; an attention-grabbing phrase every other paragraph is not.
8. **Page cap.** Aim for 150–180 pages; 200 hard ceiling including references. Count pages after the mathematics is written. Do not expand or compress merely to meet an allocation.

## Example: revision of the opening voice

**Current:** “A mathematical proof has at least two lives. There is the life in which every inference is justified … There is also the life in which a mathematician understands why the argument had any chance of working.” (L80)

**Proposed:** “Alpöge's Lean archive gives an unusually detailed formal record of an argument concerning the Riemann Hypothesis. Its size makes a line-by-line exposition impractical. The more useful task is to identify the constructions on which the proposed proof depends and explain how their conclusions are used. We begin with the last deduction, because it fixes the exact analytic statement the arithmetic arguments must establish.”

The revision is not trying to be memorable. It provides location, purpose, and mathematical direction.

## Example: revision of a mathematical transition

**Current title:** “The prime sum that can hear a zero” (L493). The following section introduces the ramp only after remarks about architectural motivation.

**Proposed title:** “A smoothed prime sum and its Mellin transform.”

**Proposed lead:** “For a Dirichlet character $\chi$, consider the weighted sum
$$R_\chi(y)=\sum_{n\le y}\Lambda(n)\chi(n)\left(\frac{y}{n}-1\right).$$
The weight vanishes at $n=y$, but its more important feature is its Mellin transform:
$$\int_1^\infty \left(\frac{y}{n}-1\right)_+ y^{-s-1}\,dy=\frac{n^{-s}}{s(s-1)},\qquad \Re(s)>1.$$
Consequently the transform of $R_\chi$ is $-L'(s,\chi)/(s(s-1)L(s,\chi))$ in the half-plane of absolute convergence. The zeros of $L$ appear as poles of this expression. This provides the analytic reason to estimate $R_\chi$: sufficiently strong control of the weighted prime sum excludes zeros in a larger half-plane.”

This is the desired rhythm: object → computation → mathematical consequence → reason to care.

## Non-negotiable editorial test

After any page, the reader should be able to state **what mathematical fact was established or explained, what it assumes, and why it matters at that point in the argument**. If a page is dominated by commentary about significance, complexity, cleverness, the writing process, or the book's “journey,” rewrite it.

**Use this file as the governing style brief for all future revisions to the monograph.**

## Addendum — the human and historical dimension (21 November 2026)

The intended reader includes a mathematically curious non-specialist who wants to understand what it would mean to live through the resolution of the Riemann Hypothesis. The manuscript must therefore do more than reconstruct a chain of definitions and deductions: it must make the stakes, difficulties, surprises, and choices of the working mathematician intelligible. A measured sense of occasion belongs in the book, especially in its opening and at genuine turning points.

**Historical accuracy is essential.** Alpöge has announced a claimed proof and published an enormous Lean formalization. Until the claimed proof and its assumptions have been independently checked, do not write that RH has definitively been proved or that the mathematical community has accepted the result. Convey the real excitement of a possibly historic moment without turning a claim into an established fact. If independent verification later changes its status, update this account against contemporary sources.

**Warmth without performance.** The author's voice is a patient mathematician who enjoys teaching. Modest, situational humor and a little lightness are welcome—especially when they arise from an unexpected cancellation, a familiar argument failing at precisely the needed boundary, or a shrewd construction—rather than from jokes, metaphors, aphorisms, rhetorical questions, or self-conscious attempts to be memorable. The narration should feel like one person helping another think, not an AI trying to sound engaging.

**Human scale.** Explain what a mathematician would have tried, why an apparently natural approach does not suffice, what the new construction preserves or gains, and what obstacle remains. A simple numerical example or a genuinely explanatory illustration is often better than an emotional adjective. Refer to Alpöge as the author of the particular argument being unpacked, not merely as an abstract name attached to a result.

**Authorial source and quotation.** Quote Alpöge's `remark.pdf` sparingly and accurately where his words reveal motivation, an unexpected difficulty, or the provenance of a construction. Attribute each quotation to its page and follow it with the relevant derivation or source-defined theorem. Use the historical voice of the author, not invented interior thoughts or scenes.

**The emotional arc must be earned.** Interest should arise from grasping mathematical necessity and ingenuity. The goal is for a non-specialist to feel the significance of the work while a mathematician can recognize a sound, traceable argument. Never exchange precision for a dramatic climax.

**A working style test.** Read each section aloud. If it sounds like a trailer for a mathematical breakthrough, reduce the rhetoric. If it sounds like a catalog of formal lemmas, restore the motivating problem and one concrete example. If its warmth survives only through exaggeration, remove the exaggeration.

## Addendum — context continuity and mathematical quality control (21 November 2026)

These rules are **operational requirements**, not optional advice. A long mathematical manuscript cannot depend on what the author happens to remember from an earlier conversation. The working files must carry the decisions, mathematics, and checks needed to resume faithfully. The purpose is to keep the prose enjoyable **because it is mathematically lucid**, rather than allowing fluency to hide omissions.

### The authoritative record

Maintain four persistent records, kept alongside the chapter sources and revised whenever the text changes:

| Record | Minimum content | What it prevents |
|---|---|---|
| **This editorial constitution** (`EDITORIAL_VOICE_AND_REVISION_NOTES.md`) | Approved voice, rejected mannerisms, intended reader, quotation policy, illustration criteria, opening model, page ceiling, and revision history | A gradual return to AI catchphrases, manufactured gravity, or textbook-like formality |
| **Mathematical dependency map** (`MATHEMATICAL_DEPENDENCIES.md`) | Every central statement in ordinary mathematical notation; complete hypotheses and scope; what it proves; prior results used; where it is introduced and used in the book | Misstating a conditional result as unconditional; reversing implications; treating a suggestive analogy as a theorem |
| **Source and verification ledger** (`SOURCE_VERIFICATION_LEDGER.md`) | Exact repository commit, file path, declaration name; references to `remark.pdf` by page; status of source inspection, independent derivation, and external verification; outstanding questions | Confusing Lean names with proved claims; invented motivation or citations; quietly promoting unverified dependencies |
| **Chapter briefs and versioned manuscript** (`chapters/` plus `CHAPTER_BRIEFS.md`) | Chapter purpose, mathematical starting point, results established, notation introduced, deferred hypotheses, figure and quote inventory, dependencies on earlier chapters, and unresolved editorial issues | Repetition, inconsistent notation, unexplained concepts, discontinuous voice, or contradictory chapters |

**Source of truth:** Consult these files and the exact source passages before extending or rewriting the manuscript. Conversational summaries and memory are navigation aids, **never replacements for the underlying text**. Do not claim a file, passage, or proof has been examined unless it has actually been reopened and inspected.

### Claims must remain stable as the argument travels

For each substantial mathematical assertion, record the following before presenting it as a theorem or an implication:

1. **Exact mathematical statement.** Preserve its quantifiers, field or group, normalization, ranges of parameters, local/global conditions, exceptional cases, and the meaning of every relevant constant or exponent. A weaker, more readable formulation is acceptable only when the weakening is explained or obvious.
2. **Dependency and status.** Distinguish (a) elementary or classical facts proved in the chapter, (b) deductions justified by identified Lean declarations, (c) deep results whose Lean statements have been inspected but whose proofs have **not** been independently audited, and (d) heuristic explanations or analogies. Compilation, absence of `sorry`, formal source inspection, and independent verification are distinct matters.
3. **Direction of implication.** Write down what the result supplies to the next chapter and what it **does not** supply. A result about a primitive character does not automatically cover every character; an estimate on a special family or a sparse window is not automatically a uniform estimate.
4. **Normalization check.** Verify arithmetic factors, signs, gamma factors, Mellin kernels, conductors, powers, and asymptotic scales from the source or a worked derivation. Numerical constants such as `401`, `1/52`, or `3/2` must not be assigned an informal significance merely because they stand out in a declaration.
5. **Provenance.** Link the exact declaration and, for interpretive statements attributed to Alpöge, the exact page of his remark. Never ascribe an intention or discovery sequence that the source does not document.

The recurring danger is **mathematical drift**: a careful, conditional statement in one chapter becomes a clean-sounding but stronger assertion several chapters later. A polished sentence is not evidence of a valid implication. The source and dependency records must be consulted again at every such transition.

### Chapter production and review protocol

Write in working units of approximately **10–20 pages**, but design the book as one continuous mathematical explanation. This is a practical unit of review, **not** a mandate to hit a page quota. Each chapter follows this sequence:

1. **Locate the mathematical problem.** Decide what genuine obstacle the chapter resolves and why that obstacle is present in the preceding argument. Start from mathematics rather than from Lean filenames or a motivational speech.
2. **Inspect sources before drafting.** Read the relevant Lean statements, follow the necessary dependencies, and check Alpöge's corresponding remarks. If the source-to-source connection is uncertain, say so and investigate it before narrating the connection as fact.
3. **Write the explanation.** Introduce objects at the moment they become necessary. Develop an example, calculation, or figure wherever it reduces conceptual load. Write complete proofs of accessible steps; isolate deeper imported results accurately rather than silently supplying imagined proofs.
4. **Mathematical review — separate from prose review.** Audit each equation, theorem hypothesis, dependency, and implication against the ledger. Check whether the preceding chapter really establishes what the current one uses. Record unresolved points as unresolved; do not repair them with a plausible story.
5. **Editorial review.** Compare pages against the approved *Structural Reductions* style and the preferred opening. Remove aphorisms, repeated antitheses, forced hooks, anthropomorphic headings, filler signposting, and rehearsed declarations of beauty. Preserve natural warmth and a little well-earned humor.
6. **Typesetting and visual review.** Compile the LaTeX, inspect the rendered pages, check figure labels and captions, and verify bibliography and page-specific quotations. The math must read correctly both in source and on the page.
7. **Commit a chapter checkpoint.** Update dependency map, verification ledger, chapter brief, manuscript, and revision notes **together**. State explicitly what the next chapter may assume and which claims remain unreviewed.

When revising an earlier chapter, **propagate the change forward**: check downstream quotations, equation numbers, terminology, hypotheses, diagrams, and conclusions. A local edit can invalidate an explanation fifty pages later.

### How to resume after context loss or a new conversation

Before writing new prose:

1. Reopen **this** editorial guide, the current manuscript, the dependency map, the source ledger, and the relevant chapter brief; do not rely on a conversation recap alone.
2. Verify which manuscript revision and pinned Lean commit are being used. Recheck the exact Lean declarations needed for the next section.
3. Read the **last several pages of the preceding chapter** and a short approved passage from *Structural Reductions* or the accepted opening. Match the established mathematical notation, argumentative pace, and human voice.
4. Identify the last fully reviewed mathematical step and the first unresolved dependency. Continue from that point, not from a convenient thematic summary.
5. If a required source cannot be reopened, **mark the limitation instead of reconstructing its contents from memory**.

A continuity checkpoint must be usable by another careful mathematician (or a fresh session) without relying on hidden context. If it is not, the checkpoint is incomplete.

### The reader, the opening, and the sense of occasion

The likely reader is interested in a potentially momentous mathematical event but has not spent a career on automorphic forms. Do not confuse **accessible** with **oversimplified**: preserve the mathematical reason for each step while omitting formal minutiae that do not advance comprehension. When a new idea is difficult, patiently build toward it; do not substitute a metaphor and move on.

The opening may acknowledge Riemann's 1859 conjecture and the remarkable public announcement by Alpöge, with precise dates and verification status. Convey excitement **about the possibility of a historic result**, not retrospective certainty that the problem has been settled. Introduce Alpöge as a working mathematician through his documented words and mathematical choices. Never invent scenes, emotions, or private motivations.

Retain the approved opening paragraph substantially as written:

> Alpöge's Lean archive gives an unusually detailed formal record of an argument concerning the Riemann Hypothesis. Its size makes a line-by-line exposition impractical. The more useful task is to identify the constructions on which the proposed proof depends and explain how their conclusions are used. We begin with the last deduction, because it fixes the exact analytic statement the arithmetic arguments must establish.

**The prose should be a pleasure to read without calling attention to itself.** A small, accurate observation, a dry aside arising from a calculation, or a brief expression of wonder is welcome; performative cleverness is not. Let the reader see why mathematicians would care and how the author's particular choices solve particular difficulties. Illustrations should clarify a mathematical relationship, not merely make the pages look lively.

### Release gate for a chapter or completed manuscript

Do not label a chapter **mathematically reviewed** until all its central statements have traceable sources or self-contained proofs; all stated hypotheses have been checked; cross-chapter uses are consistent; and every unresolved dependency is recorded. Do not label a monograph a **verified proof of RH** without independent verification of the required formal arguments and assumptions. Those standards cannot be waived for fluency, historical drama, or the 200-page ceiling.

**Page target:** Prefer 110–130 pages, including concise appendices, illustrations and references; expand toward 150 only for indispensable mathematical clarity, with a hard ceiling of 200. Never pad to fill the quota. Reduce duplication, routine lemmas, and code-level bookkeeping first. Preserve the central mathematical transitions at whatever length accurate explanation requires. If the argument cannot be faithfully explained within the ceiling, narrow the stated scope rather than silently omit an essential step.

### Quick final-page test

For each page, ask: **What mathematical fact is the reader now able to understand? Which hypotheses support it? Why is it needed here?** Then ask whether the page sounds like the same patient mathematician who wrote the approved opening. If any of these answers is unclear, revise before extending the manuscript.



## Main text, concise appendices, and illustration standard (revised 21 November 2026)

**Completeness does not mean reproducing the proof archive.** The main text must make every indispensable transition intelligible: the mathematical problem addressed, the needed statement with honest hypotheses, and how that statement feeds the next step. When a technical subject is relevant but a complete treatment would bury the argument, introduce its purpose and conclusion in the main body and refer to a **brief, explicitly numbered appendix note**. Do not use appendices as a way to hide the central reasoning.

Each appendix note should be concise (ordinarily half a page to two pages), state the relevant fact and assumptions, explain why it is true or why it is difficult when possible, and cite precise Lean declaration(s) or published references. Explicitly say when the deep proof is cited rather than reproduced. Cross-reference the appendix from the main text and the main chapter from the appendix; maintain stable labels so future revisions do not strand references.

**Preferred total length: 110–130 pages**, including appendices and references, counting from the current 74-page baseline. Allow additional pages only when they advance comprehension, with 150 pages an exceptional soft limit and 200 a hard maximum.

**Increase the number of mathematical illustrations.** Aim for roughly 10–16 purposeful figures across the complete book: localization of a derivative kernel, positive weighted residues, finite Fourier projection, several small source spaces nearly filling a larger target, slope transfer, three exact arithmetic cancellations, theta chains and seesaw, arithmetic windows, and the overall deduction. A figure must clarify a relationship that prose alone makes difficult. Each should be introduced in the text, used in the explanation, and captioned precisely; schematic simplifications must not be mistaken for proved identities.

Continue using the agreed human voice: a patient research mathematician with warmth, occasional natural humor, and genuine wonder. The writing should make the reader enjoy the mathematics, never perform enjoyment on the reader's behalf. Cite and quote Alpöge's remarks sparingly and accurately, where his words illuminate the construction or the historical moment.

## Manuscript versioning and damage-prevention protocol (added in v1.1.0)

- **v1.0.0** is the immutable, exact PDF/LaTeX snapshot of the previously delivered 73-page revised edition. Its version number is assigned retrospectively; that PDF did not print a version number.
- **v1.1.0** is the 74-page *editorial warmth* edition. The title page, second-page source note, PDF metadata, and page footers display the revision. Neither edition replaces or overwrites the other.
- Update the minor version for changes to exposition, illustrations, organization, or mathematical framing that do not change a statement or proof; update the major version if the mathematical content or proof claims are materially changed. Use patch versions for spelling and layout corrections only.
- For each release, preserve the previous PDF and TeX, record both SHA-256 hashes, provide a source diff and change log, and check all labelled statements, displayed equations, proof environments, Lean source references, and bibliography entries. Compile the PDF and examine the resulting pages.
- A *passed source-preservation check* means only that the mathematical text was unchanged relative to the previous edition. It does **not** imply that the underlying mathematics or claimed RH proof has been independently verified. Any subsequent correction to a mathematical claim must be named explicitly in the version history and reviewed in the dependent chapters.
- Before editing again, consult the most recent `VERSION_HISTORY.md`, `SOURCE_DIFF.patch`, `MATH_INVARIANTS.txt`, and original source ledger. Do not assume a newer manuscript is necessarily better.
