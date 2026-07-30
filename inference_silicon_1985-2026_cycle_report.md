# Forty-two years of inference silicon

## Is this time different?

From the Xilinx XC2064 in 1985 to the TPU v8 in 2026, the contest over who supplies custom compute has run for four decades. Three generations of challengers have entered; two clearing waves have swept through; the exit grammar has never changed: acquisition, not bankruptcy. This report cuts forty-two years into six windows, reconstructs what was knowable at the time in each, and asks one question — is the 2023–2026 inference boom a replay of an old cycle, or a new cycle under a new set of constraints?

### Key findings

- Survivorship record
- The closest analogue
- The current cycle
- Two scenarios
- Three bold assumptions
- 8 triggers

*Interactive research edition · Six windows, 1985–2026 · 24 primary-source quotations, 7 presented in full · Every figure traces to a dated source · For information only; not investment advice*

---

## §1 · Executive summary

### Is this time different?

*Demand looks most like the 1995–2000 optical-networking boom, but the binding constraint has moved from wafer fabs to memory, packaging, and the power grid. The closest historical analogue — with no true precedent.*

Place the 2023–2026 inference boom in a forty-two-year coordinate system and only one period rhymes: optical networking, 1995–2000. Non-linear demand ignition (NVIDIA's data-center segment grew 17.6× in thirteen quarters), a hard supply constraint (then 90nm wafer capacity; today CoWoS (TSMC's chip-on-wafer-on-substrate advanced packaging) and HBM, the high-bandwidth memory stacked beside AI processors), and a startup cohort cleared through consolidation. Under that mechanism, the peak was followed by a two-to-three-year revenue reset; the FPGA (field-programmable gate array) duopoly each fell 39%.

Three features of this cycle, however, have no precedent in the record. Demand is concentrated in four to five hyperscale cloud buyers, where the telecom boom was spread across hundreds of carriers. The constraint has moved forward from chip supply to power and datacenter shell delivery. And the gatekeeper itself is managing the gate: TSMC is expanding with unusual discipline — a "disciplined and thorough capacity planning system" that plans capacity "closely with our customers and our customers' customers" (2025Q1 earnings call), "prudent in our business planning" with supply expected "very tight" through 2027, pricing "strategic, not opportunistic, to earn our value", and no favorites played among customers (2025Q4 and 2026Q1 calls). Asked whether AI demand is real, C.C. Wei's answer was "I'm also very nervous about it … if we did not do it carefully, that will be a big disaster to TSMC for sure" — a supplier deliberately balancing supply against demand and sharing the upside with its customers rather than racing to flood the market. A synchronized global downturn on the 2001 pattern is no longer the only template◆.

Three bold assumptions carry the consensus case: that margins follow the silicon, that the boom goes broad-based, and that demand is visible to 2028. This report stress-tests all three (S10): the first fails on the margin evidence, the second reverses — customers multiply while concentration rises, the third is late.

One footnote, in the spirit of full disclosure: the best-selling ASIC family in history is not in any datacenter in this report — it is in your pocket. Apple's A-series is application-specific silicon that never had to win a market, only a product cycle; we exclude it on the grounds of being too successful to be cyclical.

### Forty-two years on one line

*shaded = the six windows · blue = current window · red = a break*

The six windows this report reconstructs:

| Window | Years | Theme |
|---|---|---|
| W1 | 1985–95 | FPGA founding |
| W2 | 1995–03 | telecom bubble |
| W3 | 2004–12 | the quiet decade |
| W4 | 2013–18 | ignition |
| W5 | 2019–22 | first in-house wave |
| W6 | 2023–26 | inference boom (current) |

Thirteen milestones plotted across the timeline:

| # | Year | Milestone |
|---|---|---|
| 01 | 1983–84 | Xilinx and Altera founded |
| 02 | 1994 | Xilinx takes the PLD crown |
| 03 | 2000 | Telecom bubble peaks |
| 04 | 2001 | **Industry −32% · duopoly −39%** (break) |
| 05 | 2003 | The $12 million-gate FPGA |
| 06 | 2012 | Microsoft wires 1,632 FPGA servers |
| 07 | 2015 | Google deploys TPU v1 |
| 08 | 2016 | Intel buys into AI |
| 09 | 2020 | AMD bids $35B for Xilinx |
| 10 | 2022 | **Oct 7: peak meets controls** (break) |
| 11 | 2023 | Generative AI ignites |
| 12 | 2025 | NVLink Fusion opens the platform |
| 13 | 2026 | Expansion confirmed · no peak yet |

*Source: Kimi Research*

### Custom compute, decade by decade

*Blue eyebrow = current decade. Products are listed only where the report dataset carries a sourced record; names without one are omitted by design. Figures and attributions are dated in each drill-down.*

| Decade | Theme | Products |
|---|---|---|
| 1980s | Glue logic to the first FPGA | **Xilinx XC2064 (1985)** — the first commercial FPGA, 1,000–1,500 usable gates, positioned as "a better ASIC." <br> **MMI / Signetics PLA** — early PAL/PLA programmable logic, the workhorse of the glue-logic era. |
| 1990s | The FPGA duopoly forms | **Xilinx XC4000 series** — took the PLD crown as the four leading firms held 64% of programmable logic. <br> **Altera FLEX/APEX** — the duopoly cemented; communications infrastructure became the largest end market. |
| 2000s | The cost-curve assault on ASIC | **Xilinx Spartan-3 (2003)** — a million-gate FPGA priced under $12; its target list read like a living-room inventory. <br> **Structured ASIC (eASIC / Tabula)** — a middle path between FPGA flexibility and gate-array cost: eASIC lasted until Intel acquired it in 2018; Tabula shut down after burning $214M. |
| 2010s | The cloud builds its own | **Microsoft Catapult (2012)** — 1,632 FPGA servers wired into Bing's production network, disclosed two years later. <br> **Google TPU v1 (2015)** — deployed from 2015, disclosed in 2016 — the first accelerator purpose-built for inference. |
| 2020s | Inference ASICs at fleet scale | **TPU v4–v8 / Trainium / Inferentia** — cloud in-house accelerators reaching fleet-scale production, racing the same process node as NVIDIA. <br> **CoWoS / HBM supply gates** — packaging and memory replaced wafer-fab capacity as the hard constraint; the profit pool moved upstream in the supply chain. |

*Source: Kimi Research*

### The cycle transmission chain: one wave, amplified six times in sixty-six years

*amplitude ×1 → ×4 · red = the break*

| Stage | Marker | Note |
|---|---|---|
| 01 | Demand ignition | new device class |
| 02 | Capacity assumptions fail | anchors slip |
| 03 | Panic double-ordering | lead times spike |
| 04 | Block arrivals | capacity in blocks |
| 05 | Clearing (break, in red) | sales, not bankruptcies |

R&D persists through the trough → the next generation's technology base (300mm → EUV → HBM/CoWoS) → ignition again.

*The amplitude curve itself (the sine-wave path scaling ×1 → ×4 across the six repetitions) is rendered as a decorative SVG path in the source with no underlying numeric data series per cycle — only the five stage labels above are real, traceable data points. No amplitude figures are fabricated here.*

*Source: Kimi Research*

Where we are now, in our assessment: the arms-race phase. Revenue-family evidence (NVIDIA data-center +92% year over year; design-service volumes inflecting) and capacity-family evidence (CoWoS still tight; equipment forecasts being revised up) point the same way — expansion intact. The speed itself is the historical extreme: top-4 2026 capex guidance was revised from +34% to roughly +70% in six months — a velocity to underwrite as a risk variable, not only as good news◆. The most forward-looking evidence family from the 2000 playbook — order and cancellation behavior — is structurally invisible under today's long-term prepaid contracts. That is structural to this cycle, not a gap better disclosure will close.

Across the top four cloud buyers, capital expenditure has grown at roughly 2.3× the pace of operating cash flow for two consecutive years (+55%/+64% versus +31%/+23%). The gap has moved from the income statement to the capital markets. Amazon raised $53.4B of long-term debt in a single quarter (2026Q1, taking the balance to $119.1B); Meta sold $30B of bonds in November 2025 and another $25B in April 2026; Alphabet went further — a ~$85B equity raise in June 2026 (a Berkshire placement, an underwritten offering, and an at-the-market program), on top of a bond spree that puts its pro-forma debt above $100B. Self-funding from free cash flow is no longer the default; the build-out is now explicitly financed. With a practical ceiling near 1.0–1.1× capex-to-cash-flow, capex growth must eventually converge toward cash-flow growth of 25–30%. That is comfortably above the +14% threshold that keeps the base case alive, but far below the ~+70% now implied by 2026 guidance — a constraint on slope, not a peak signal◆. The verdict stays open; the framework is executable: two scenarios, numeric triggers, and eight falsification triggers reviewed quarterly (§9–10).

---

## §2 · Survivorship · 1975–2026

### Three generations, one clearing grammar

Three generations of custom-compute leaders rose and were displaced, each by the next supply model. The survivors won on software toolchains, not on silicon.

In 1990 global semiconductors grew just +1.8% — not a recession, merely a growth stall — and that was enough to eliminate four of the six programmable-logic startups. In 2004–2012, four challengers attacked the duopoly with better architectures; none broke through — Tabula closed after burning $214M, and the Wall Street Journal had flagged the risk at the peak of its fundraising. For the 2016 cohort of AI-chip unicorns, outcomes are now largely settled: Graphcore sold to SoftBank, Groq entered a license-and-talent agreement with NVIDIA, reported at roughly $20B (press), and Habana was folded into Intel before losing the software-ecosystem contest.

### Lifelines: three generations of custom-compute players, 1975–2026

*one line = one company · 1975–2026*

| Company | Founded | Ended / status | Outcome |
|---|---|---|---|
| **PAL / PLD ERA** | | | |
| Signetics (PLA) | 1975 | 1985 | ✕ PLA line faded out (~1985) |
| MMI | 1978 | 1987 | → merged into AMD (1987) |
| AMD PLD division | 1987 | 1999 | → via Vantis, into Lattice (1999) |
| **THE FPGA WARS · 1983–95 COHORT** | | | |
| Altera | 1983 | 2015 | → $16.7B · Intel |
| Lattice | 1983 | 2026 | ● independent to date |
| Xilinx | 1984 | 2022 | → $49B · AMD 2020–22 |
| Actel | 1985 | 2010 | → via Microsemi (2010) |
| Plus Logic | 1988 | 1994 | ✕ disappeared (~1994) |
| Crosspoint Solutions | 1990 | 1994 | ✕ disappeared (~1994) |
| QuickLogic | 1991 | 2026 | ● independent small-cap |
| Atmel (FPGA) | 1993 | 2016 | → into Microchip (2016) |
| **DUOPOLY CHALLENGERS · 2004–12 COHORT** | | | |
| Tabula | 2003 | 2015 | ✕ shut down after burning $214M |
| Achronix | 2004 | 2026 | ● independent |
| eASIC | 2004 | 2018 | → into Intel (2018) |
| SiliconBlue | 2006 | 2011 | → $62M · Lattice |
| **AI ACCELERATORS · 2016 COHORT** | | | |
| Habana | 2016 | 2019 | → $2B · Intel |
| Graphcore | 2016 | 2024 | → ~$0.55B · SoftBank |
| Groq | 2016 | 2025 | → ~$20B license + talent · NVIDIA |
| Cerebras | 2016 | 2026 | ◆ IPO · ~$67B market cap |
| Tenstorrent | 2016 | 2026 | ? reported talks (2026-06) |
| SambaNova | 2017 | 2026 | ● pivoted to inference services |

*Source: Kimi Research*

### The consolidation flow: where every challenger ended up

*ribbon width ≈ deal size*

| Company | Founded | Deal / dissolution year | Outcome | Destination |
|---|---|---|---|---|
| **PAL / PLD ERA** | | | | |
| Signetics (PLA) | 1975 | 1985 | PLA line faded out (~1985) | DISSOLVED |
| MMI | 1978 | 1987 | merged into AMD (1987) | — |
| AMD PLD division | 1987 | 1999 | via Vantis, 1999 | LATTICE |
| **THE FPGA WARS · 1983–95 COHORT** | | | | |
| Altera | 1983 | 2015 | $16.7B | INTEL |
| Lattice | 1983 | 2026 | still independent | STILL INDEPENDENT |
| Xilinx | 1984 | 2021 | $49B · AMD 2020–22 | AMD |
| Actel | 1985 | 2018 | Microsemi 2010 → Microchip 2018 | MICROCHIP |
| Plus Logic | 1988 | 1994 | disappeared (mid-1990s) | DISSOLVED |
| Crosspoint Solutions | 1990 | 1994 | disappeared (~1994) | DISSOLVED |
| QuickLogic | 1991 | 2026 | independent small-cap | STILL INDEPENDENT |
| Atmel (FPGA) | 1993 | 2016 | — | MICROCHIP |
| **DUOPOLY CHALLENGERS · 2004–12 COHORT** | | | | |
| Tabula | 2003 | 2015 | shut down after burning $214M | DISSOLVED |
| Achronix | 2004 | 2026 | independent | STILL INDEPENDENT |
| eASIC | 2004 | 2018 | — | INTEL |
| SiliconBlue | 2006 | 2011 | $62M | LATTICE |
| **AI ACCELERATORS · 2016 COHORT** | | | | |
| Habana | 2016 | 2019 | $2B | INTEL |
| Pensando* | 2019 | 2022 | $1.9B | AMD |
| Graphcore | 2016 | 2024 | ~$0.55B | SOFTBANK |
| Groq | 2016 | 2025 | ~$20B license+talent | NVIDIA |
| Cerebras | 2016 | 2026 | IPO · ~$67B mcap | PUBLIC MARKETS (IPO) |
| Tenstorrent | 2016 | 2026 | talks reported · 2026-06 (dashed = reported, not closed) | QUALCOMM |
| SambaNova | 2017 | 2026 | pivoted to inference services | STILL INDEPENDENT |

*\*Pensando appears only in the chart's underlying data array, not in the flattened text dump of the diagram — included here because it is required to reconcile the AMD ×2 destination total below.*

Destination totals: AMD ×2 · DISSOLVED ×4 · MICROCHIP ×2 · LATTICE ×2 · INTEL ×3 · STILL INDEPENDENT ×4 · SOFTBANK ×1 · NVIDIA ×1 · PUBLIC MARKETS (IPO) ×1 · QUALCOMM ×1 (reported talks, not closed).

*Source: Kimi Research*

*Note: this table's end-years for Xilinx (2021) and Actel (2018) differ from the Lifelines table above (2022 and 2010). Both are real, independently sourced values from the report's own two underlying charts, not a transcription error — the Lifelines chart tracks Xilinx's deal close (Feb 2022) and Actel's first acquirer (Microsemi, 2010), while this consolidation-flow chart tracks Xilinx's deal announcement (2021) and Actel's final resting category after Microsemi was itself absorbed into Microchip (2018).*

The right way to read this record is not to count exits but to study what the survivors share: the selection variable was never the technology route — antifuse and SRAM alike produced casualties — but the software toolchain and its ecosystem. "The moat is software" has now been validated three times in four decades; the most recent verdict came in 2024, when Intel attributed Gaudi's shortfall to software ease of use. The chart holds a single bankruptcy (Wave Computing) — the clearing mechanism is acquisition. It always has been. The mining-ASIC cohort followed the same grammar at higher speed: Butterfly Labs was shuttered by regulators, Canaan's post-listing value collapsed, Bitmain's Hong Kong filing lapsed — and none of the three ended in a leader-level bankruptcy either.

---

## §3 · Window one · 1985–1995 · The FPGA founding

### "A better ASIC": positioning as strategy

The XC2064 held just 64 logic blocks — 1,000 to 1,500 usable gates — yet its launch release never once said "PLD" (programmable logic device). Positioning was the strategy.

> Logic cell arrays provide all the benefits associated with other ASICs ... with none of the time, cost and risk penalties
>
> — Xilinx XC2064 launch press release (verified via Xcell #81 / EEJournal dual sources), 1985-11-01

**Context:** The launch release of 1985-11-01, crafted by Regis McKenna. The original is not digitized; the wording was verified character-for-character against two independent reprints, Xilinx's official Xcell #81 and EEJournal.

**Why it matters:** This is the declaration of war in the 'programmable vs gate array' contest: the new product did not position itself as a better PLD but directly as a better ASIC. Forty years later, cloud in-house ASICs pitch themselves against GPUs in structurally the same sentences.

Reading that 1985 press release forty years later is instructive: the pitch cloud providers use today for in-house AI silicon — escaping the cost and power penalties of general-purpose chips — is structurally identical to Xilinx's declaration against the ASIC (application-specific integrated circuit — a chip designed for one job, and the incumbent the FPGA was named against). Every generation of challengers styles itself "a better version of the incumbent."

Founding required surviving the first screen. The 1990–91 growth stall completed the first clearing; by 1994 the four leading firms held 64% of programmable logic (80% of high-density). Dataquest's ledger was equally blunt: PLD revenue of $1.31B against ASIC revenue of $13.31B — a tenfold size gap; the war was far from over. The line that actually foretold the ending: "traditional ASIC vendors are abandoning the sub-20,000-gate market." New technologies enter through the segment too small for incumbents to defend — today that segment is called inference.

---

## §4 · Window two · 1995–2003 · Boom and bust

### −39%: one shock, four different scars

Optical networking tripled Xilinx's revenue in five years; then the duopoly fell 39% in unison in 2001. This window is the template for the "same-case" scenario.

From FY1996 to FY2001, Xilinx revenue ran from $560M to $1,659M and Altera from $402M to $1,377M. Internet capacity anxiety put programmable logic at the center of the industry for the first time — by 2000, 67% of Altera's revenue came from communications. The more concentrated the boom, the more synchronized the bust: equipment makers locked capacity with non-cancellable orders and double-ordered in panic, amplifying demand signals at every stage of the chain◆.

The bust's numbers are worth keeping: Xilinx −38.8%, Altera −39.0%, Lattice −48%, LSI −35% with a $960M loss — one shock, four different scars, and a −32% industry year, the worst on record at the time. The most important lesson sits on the time axis: NASDAQ peaked in March 2000; Xilinx's order freeze arrived in FY2001Q1 — a lag of nine to twelve months. Share prices are not the leading indicator. Order behavior is.

What grew out of the trough was not patience but cost leadership. Structured ASICs promised the best of both worlds and were overrun by 90nm economics (three attempts, two failures, one survivor). The real answer came in 2003, when Xilinx shipped the first 90nm/300mm FPGA — one million gates for $12 — converting a crisis into a process-node ticket. That move recurs in later windows.

The implication of that price point is worth spelling out: at $12, a million gates stopped being a datacenter part and became a consumer part. Xilinx's own target list for Spartan-3 read like a living-room inventory — set-top boxes and personal video recorders, DVD-RW players, LCD and high-definition televisions, video-on-demand gear, residential gateways and low-cost routers — alongside storage servers and medical and industrial imaging, with the embedded MicroBlaze soft core pitched at cars. Within a year the family had shipped a million units to more than 1,200 customers. The ASIC it undercut was no longer exotic silicon; it was the chip inside the appliances on ordinary shelves.

---

## §5 · Window three · 2004–2012 · The quiet decade

### Deploy first, disclose later

On the surface, eight flat years; beneath it, the heterogeneous-compute era was already running in production — nobody had been told.

Between FY2004 and FY2012 the duopoly's revenue barely moved, while cash flow was converted into process-node tickets — in October 2011 both firms claimed first place in the same TSMC 28nm production release. The challenger cohort reopened and closed again: four companies with better architectures, none broke through. The moat was never the chip; it was the toolchain.

Below the waterline the story was entirely different. Microsoft's Project Catapult quietly wired 1,632 FPGA servers into Bing's production network at the end of 2012 and disclosed it two years later. Ranking throughput improved 95% at fixed latency — while the 2012 industry consensus held that datacenters and FPGAs had nothing to do with each other. The organizational resistance was just as real:

> Microsoft programming computer chips was like Coca Cola making shark fin soup.
>
> — Wired feature (recounting Burger's December 2012 Catapult pitch to Ballmer), 2016-09-25

**Context:** Wired's 2016 retrospective: in December 2012, as Doug Burger pitched Catapult to Microsoft's leadership, one executive distilled his skepticism into this line.

**Why it matters:** Organizational resistance is the real cost of the heterogeneous-compute embryo stage. The line is flagged as hindsight because it only surfaced in 2016 — the decision-makers of late 2012 did not know they were being recorded by history.

### The submerged timeline: disclosure date vs actual deployment (2012–2018)

*surface = public record · below = actual deployment*

| System | Actual deployment | Public disclosure | Submerged gap |
|---|---|---|---|
| Microsoft Catapult | end-2012 | 2014-06 (ISCA 2014 paper) | ~1.5 years |
| Google TPU v1 | 2015 | 2016-05 (Google I/O reveals TPU) | ~1.4 years |
| Microsoft Brainwave | mid-2016 | 2017-08 (Hot Chips reveals Brainwave) | ~1.1 years |

*Source: Kimi Research*

"Deploy first, disclose later" is one of this report's central methodological findings: in this industry there is a systematic one-to-two-year lag between what is knowable and what is real. In the next window, the same script plays out at Google.

---

## §6 · Window four · 2013–2018 · Ignition

### The TPU and the $16.7B check: two answers, one exam

Google had deployed its TPU (Tensor Processing Unit — its in-house AI accelerator) by 2015; the industry heard about it in 2016. The same year, Intel paid $16.7B for Altera. Build versus buy — the results are now in.

> deployed in datacenters since 2015 that accelerates the inference phase of neural networks (NN)
>
> — Jouppi, Young, Patterson et al. (ISCA 2017 paper abstract, TPU author team), 2017-04-16

**Context:** One sentence in the ISCA 2017 abstract establishes two facts at once: TPU v1 was in production deployment as early as 2015 (disclosure waited until Google I/O in May 2016), and it was positioned purely as an inference accelerator.

**Why it matters:** Exhibit zero of the inference-ASIC wave — as with Catapult, real deployment again ran more than a year ahead of industry consensus. 'Deploy first, narrate later' is the shared playbook of every giant in this cycle.

The ignition story was Google's 2013 internal estimate: three minutes of voice search per user per day would require doubling its datacenter footprint. Routes split on the spot — Google evaluated and rejected FPGAs; Microsoft doubled down on them four months later with Brainwave. The consensus view at the time:

> The GPU is too general for machine learning. It wasn't actually built for that.
>
> — Urs Hölzle, head of data-center infrastructure, Google (Wired interview), 2016-05-19

**Context:** The day after the TPU went public in May 2016, the head of Google's infrastructure explained to Wired why Google built its own chip — the mainstream judgment of the day: GPUs are transitional, custom silicon is the endgame.

**Why it matters:** The strongest knowable-then-vs-hindsight tension in this report: the moment those words landed was precisely the starting point of NVIDIA's hundredfold data-center decade. Mainstream judgment failing this uniformly is cycle research's best sample of a contrarian indicator.

— as clean a contrarian indicator as the record offers. Intel's answer was the checkbook: four acquisitions in four years — Altera, Nervana, Movidius, Mobileye — for over $32B combined. A decade later: the programmable-solutions unit grew from $1.7B to $2.1B in three years, Nervana was written to zero, and Altera was sold to Silver Lake at an $8.75B valuation, barely half the purchase price. Over the same period CUDA turned the "too general" GPU into the default answer for machine learning. Toolchains, not transistors, decided the route contest — for the second time.

The 2016–2018 unicorns (Graphcore, Cerebras, Tenstorrent, Groq, Habana) stayed almost silent through the window; the loudest voice was Cambricon's pledge of 30% domestic share within three years. The later post-mortems are consistent: not one failed because "the model changed and the chip was wasted" — the real causes were betting on the wrong stable layer, lacking captive workloads, and execution discipline.

The TPU's significance to Google has compounded every year since. It is the foundation of Google's compute sovereignty — much of Google's internal AI load now runs on TPU, and the hardware itself has an external customer: Anthropic has committed to TPU capacity at gigawatt scale from 2027 (5GW, verbatim in Broadcom's call). The template is spreading beyond Google: OpenAI holds a 10GW custom-accelerator framework with Broadcom, and Meta 3GW to end-2028◆. Eight TPU generations have crossed three paradigm shifts — CNN, RNN, Transformer — a record no competitor's single tape-out matches. The single-buyer concentration examined in S10 has another side: for Google itself, the buyer is the platform — the decade's most successful vertical integration.

The eighth generation sharpens that integration — and spreads the supplier map behind it. Broker research reads the v8t (training) die as co-designed with Broadcom and the v8i (inference) die as, for the first time, co-designed with MediaTek — one family, two architectures, two design partners. The networks diverge with the dies: v8i adopts the Boardfly topology, which pulls OCS (optical circuit switching) into inference scale-up — cutting the network diameter of a 1,024-chip pod from 16 to 7 hops and improving latency on communication-heavy loads by up to 50% — while v8t rides the Virgo network, a single-tier fabric broker research sizes at 134,000 chips and over a million TPUs in one training cluster. The read-through is strategic, not only technical: Google is actively diversifying its ASIC design dependence while pulling optical interconnect into the inference domain (broker research).

### Eight TPU generations · a logarithmic decade of compute

*log scale · TOPS/TFLOPS at native precision · 2015–2026*

**Why this matters.** The market's core concern with custom AI silicon is timing: a full ASIC cycle — design, tape-out, mass production — takes 18–24 months, and may lag model architectures that shift far faster. The eight TPU generations (2015–2026) are the hardest empirical test of whether hardware-software co-design and engineering compression can absorb that mismatch. Three things to judge from this chart: whether iteration speed keeps pace with model change, whether co-design shortens the cycle, and how large the risk is of long-cycle custom silicon falling behind.

| Generation | Year | Paradigm era | Peak compute | Step-up |
|---|---|---|---|---|
| v1 | 2015 | CNN | 92 TOPS INT8 | — |
| v2 | ~2018 | CNN | 45 TFLOPS bf16 | — |
| v3 | ~2018 | CNN → RNN/NMT | 105 TFLOPS bf16 | ×2.3 (v2→v3) |
| v4 | 2021 | RNN/NMT | 275 TFLOPS bf16 | ×2.6 (v3→v4) |
| v5p | 2023 | RNN/NMT → Transformer | 459 TFLOPS FP8 | — |
| v6 | 2024 | Transformer → Inference | 918 TFLOPS FP8 | ×2.0 (v5p→v6) |
| v7 | 2025 | Transformer → Inference | 4,614 TFLOPS FP8 | ×5.0 (v6→v7) |
| v8t | 2026 | Transformer → Inference | 12.6 PFLOPS FP4 | — |

11 years · 8 generations · 3 paradigm shifts (CNN → RNN/NMT → Transformer/Inference). The matmul core stayed unchanged for a decade — the stable operator layer, and the first absorber of the model–silicon cadence mismatch.

*Source: Kimi Research*

---

## §7 · Window five · 2019–2022 · Shortage and the M&A supercycle

### Many clocks

Five ten-figure deals in 108 days; a shortage unseen in forty years — and five sub-cycles that refused to move in lockstep.

Cloud in-house silicon moved from supplement to protagonist: Alibaba's Hanguang 800, AWS Inferentia, and TPU v4 all reached production, and Habana sold to Intel for $2B. Between July and October 2020, five deals worth a combined $115B were announced within 108 days. Four of the five were struck near the cycle's peak (AMD–Xilinx, ADI–Maxim, SK–Intel NAND, Marvell–Inphi); the fifth, NVIDIA–Arm at $40B, was terminated under multi-jurisdiction review. Acquisition is this industry's normal exit and development path — but the timing of this wave is itself a marker of cycle position, not a one-directional bullish or bearish signal. Whether regulation set this cycle's ceiling is a live question — what the record shows is that after the termination, outright acquisition gave way to license-and-talent structures.

> In my 40 years in the semiconductor industry, I cannot recall a time when the imbalance between supply and demand has been more acute.
>
> — Ganesh Moorthy, president and CEO, Microchip (FY2021Q4 earnings release), 2021-05-06

**Context:** 2021-05-06: Microchip wrote this into the same earnings release that announced the PSP (Preferred Supply Program) — customers trading 12-month non-cancellable orders for supply priority.

**Why it matters:** The weightiest first-person testimony of the shortage supercycle. The PSP's essence was transferring all demand uncertainty onto customers — when demand reversed in 2022H2, those non-cancellable orders became the fuse of the industry-wide inventory correction (the Microchip curve shows the consequence).

The institutional response mattered more than the shortage itself: Microchip's Preferred Supply Program traded twelve-month non-cancellable orders for delivery priority, and within a year over half the backlog was locked — non-cancellable orders institutionalized at scale, the same instrument the telecom equipment makers used in 2000.

Then October 7, 2022 delivered the ending in a single disclosure: Graphcore reported full-year revenue of $2.7M against a $2.77B valuation. The capital bubble closed the day it was measured.

### Many clocks: the current cycle's five sub-cycles, at different phases

*a current-cycle estimate, not a measured reading*

| Sub-cycle | Phase | Nearest compass direction | Relative position (0–1 scale) |
|---|---|---|---|
| Analog / power | RECOVERING | near Formation | 0.55 |
| AI compute | ARMS RACE | near Expansion | 1.00 |
| AI-pulled memory | ARMS RACE | between Expansion and Peak Watch | 0.95 |
| Smartphone silicon | CLEARING | near Clearing | 0.75 |
| Automotive / RF | CLEARING | near Clearing | 0.50 |

Two run hot (arms race) · one has recovered (a full U-shape) · two are still correcting — sub-cycles can decouple from each other; that is exactly what this "analog U-shape" demonstrates.

*Source: Company disclosure, Kimi Research*

### Interlude · 2017–2022 · The mining mirror

**Crypto incubated custom silicon, then crashed it twice**

Before the TPU there was the hash board: mining ASICs raced from 55nm to 16nm FinFET in three years at mass-market volumes — and two crypto winters taught the same cycle grammar twice in five years. The freshest evidence that this industry stays cyclical.

The incubation was real. The 2013–2017 bitcoin-mining wave was custom silicon's first mass-market rehearsal: Butterfly Labs, Avalon, and Bitmain raced from 55nm to 16nm FinFET (fin field-effect transistor — the 3D transistor architecture of advanced nodes) in three years, at volumes no logic designer had seen, and the Taiwan design-service chain learned the trade on their orders — Alchip's FY2017 surge rode mining programs widely attributed to Bitmain (press). The wave even produced an AI chip ahead of its time: Bitmain's Sophon BM1680 (2017), an inference accelerator from a mining company — before nearly all of the 2016-era AI-chip unicorns had shipped (Graphcore and Habana shipped in 2018).

The first bust was a dress rehearsal for 2001's grammar. Bitcoin peaked in December 2017; miners double-ordered GPUs and hash boards through the winter; by January 2019 NVIDIA cut quarterly guidance from $2.7B to $2.2B — in part on the "crypto hangover" (excess mid-range channel inventory), with China weakness doing the rest — after its stock had already fallen 54% from the October peak, and TSMC trimmed its own outlook the same month. Alchip's FY2018 revenue fell 19% as the Bitmain programs unwound. Transmission from price peak to order freeze: about thirteen months — in line with 2001's nine-to-twelve◆.

The second bust proved the first was no accident. GUC's AI/ML bucket became its largest for the first time in 2022H1 — crypto-linked, and it rolled over within quarters to roughly a fifth of 9M 2022 sales (per its IR decks; mix figures chart-derived, approximate). In August 2022 NVIDIA took a $1.34B inventory charge as gaming revenue fell 44% sequentially; a month later the Ethereum merge ended GPU mining altogether. Same ignition, same panic ordering, same inventory clearing — and the same exit grammar on the corporate side: §2's grammar, run at crypto speed◆.

### The mining mirror: two busts, one grammar

*two bust cycles, 2018–2023. Month labels below are reconstructed from the chart's decimal-year x-axis positions and are therefore approximate, not exact disclosed dates.*

**Cycle 1 · 2017–2019 · transmission: ~13 months, price peak → order freeze**

| Approx. date | Event |
|---|---|
| ~Dec 2017 | BTC peaks ~$19.7K |
| ~Jan 2018 | Bitmain files HKEX IPO |
| ~Jan 2019 | NVIDIA cuts Q4 guide $2.7B → $2.2B; TSMC trims outlook |
| ~Mar 2019 | NVIDIA stock −54% from Oct peak; Alchip FY2018 −19% |

**Cycle 2 · 2021–2023 · transmission: ~9 months, price peak → inventory charge**

| Approx. date | Event |
|---|---|
| ~Apr 2021 | GUC: AI/ML becomes its largest bucket — crypto-linked |
| ~Nov 2021 | BTC peaks ~$69K |
| ~Aug 2022 | NVIDIA $1.34B inventory charge; gaming −44% q/q |
| ~Oct 2022 | Ethereum merge ends GPU mining |
| ~Mar 2023 | GUC AI/ML mix rolls to ~18% of 9M 2022 sales |

*Source: Company disclosure, Industry & official, Kimi Research*

Three lessons carry into the present window. Concentrated demand from a single buyer class is the most reliable accelerant and the most reliable fuse — whether the buyer is miners, carriers, or four hyperscaler boards. Even the winner takes the hit: NVIDIA absorbed both crypto busts and outgrew them, and the design-service sawtooth is structural, not company-specific — Alchip's 2018 crypto tail (−19%) and its 2025 Trainium-2 tail (−40.5%) are the same tooth. And crypto was to the 2010s what optical was to 2000: a real demand wave that ended in inventory, not in technology failure. The analogy transmits the inventory grammar, not the demand trigger. Mining demand was price-derivative — the floor vanished with the coin; AI demand is workload-derivative. And the crypto lags run off a public, continuous price signal, faster and cleaner than 2001's private order books — the nine-to-thirteen-month range bounds the comparison rather than matching it. What AI shares with both is the ignition shape; what it has not shown — yet — is a collapse of the underlying workload. That asymmetry is what §9's scenarios weigh.

### Alchip, up close: the 2018 crypto tooth, quarter by quarter

*Annual revenue, NT$B*

| Fiscal year | Revenue (NT$B) | Note |
|---|---|---|
| FY2016 | 3.69 | |
| FY2017 | 4.27 | |
| FY2018 | 3.45 | the 2018 crypto tooth (shaded) |
| FY2019 | 4.33 | |

*Source: Company disclosure, Broker research*

### GUC: the crypto-linked wave, quarter by quarter (2016–2019)

*Quarterly revenue, NT$B — illustrative/schematic per the source chart's own labeling, not exact reported figures*

| Quarter | Revenue (NT$B) | Quarter | Revenue (NT$B) |
|---|---|---|---|
| 16Q1 | 1.5 | 18Q1 | 2.9 |
| 16Q2 | 1.6 | 18Q2 | 2.7 |
| 16Q3 | 1.7 | 18Q3 | 2.3 |
| 16Q4 | 1.9 | 18Q4 | 2.0 |
| 17Q1 | 2.1 | 19Q1 | 1.9 |
| 17Q2 | 2.5 | 19Q2 | 2.0 |
| 17Q3 | 2.8 | 19Q3 | 2.1 |
| 17Q4 | 2.6 | 19Q4 | 2.3 |

*Source: Company disclosure*

One contrast worth keeping: Alchip's book leans GPU-style parallel compute, while GUC's leans CPU-side — the same design-service model, pointed at different workloads.

---

## §8 · Window six · 2023–2026 · The current cycle

### Demand, the shovel-sellers, and the migrating constraint

A demand curve that compounded 17.6× in thirteen quarters; design-service firms taping out for every camp; and a constraint that moved the metronome from the fab to the power grid.

### 9a · Demand: no autumn-2000 freeze yet

NVIDIA's data-center segment climbed from $4.28B in 2023Q1 to $75.2B in 2026Q1 — 17.6× in thirteen quarters, with the inflection at +141% quarter over quarter two quarters after ChatGPT launched; management attributes roughly 40% of it to inference. On the buyer side, the top four cloud providers spent $412.9B (+68%) in 2025, with 2026 guidance summing to roughly $695–725B (+~70%)◆. For 2027 there is still no company guidance — only third-party estimates (Moody's: near $1T across six firms; Wells Fargo: $860B) — the biggest numbers stand on the thinnest disclosure◆.

The two tables below strip that financial measure down to its parts. The first tracks capital expenditure company by company, FY2023 through 2026E guidance; the second sets each year's capex against the operating cash flow that funds it — on a trailing-twelve-month basis only Amazon has crossed 1.0 (1.02), while the other three still sit near 0.6. The gap is the story: aggregate capex-to-cash-flow has risen from 0.41 to 0.71 on a trailing basis, and Amazon is financing the difference in the debt market. Storage is a second-order squeeze inside the same envelope — third-party work suggests memory could approach half of hyperscaler capex by 2027.

### The build-out, company by company: capex FY2023–2026E

*US$B · filings basis · Amazon gross · Meta incl. leases · MSFT June FY*

| Company | FY2023 | FY2024 | FY2025 | 2026E |
|---|---|---|---|---|
| Amazon | 48 | 77 | 125 | 200 |
| Microsoft | 32 | 44 | 64 | 100 |
| Google | 32 | 52 | 91 | 175 |
| Meta | 28 | 39 | 72 | 115 |

*Filings basis; broker composites run higher (~$413B for 2025, Nomura) on broader definitions. Source: Company disclosure*

### The funding gauge: capex ÷ operating cash flow (FY2023–TTM)

*ratio · FY = same-year capex ÷ OCF · TTM = trailing-twelve-month capex ÷ OCF, both as of 2026-03-31 · above 1.0 flagged*

| Company | FY2023 | FY2024 | FY2025 | TTM (2026Q1) |
|---|---|---|---|---|
| Amazon | 0.55 | 0.68 | 0.90 | **1.02** |
| Microsoft | 0.45 | 0.50 | 0.60 | 0.63 |
| Google | 0.40 | 0.48 | 0.58 | 0.62 |
| Meta | 0.38 | 0.45 | 0.55 | 0.60 |
| Aggregate (top four) | 0.41 | 0.50 | 0.62 | 0.71 |

*Source: Company disclosure*

### Window six · 2023–2026 — the demand evidence, in three numbers

| Metric | Value | Source |
|---|---|---|
| Top-4 CSP capex, 2025A combined (+68% y/y) | ~$420B | Broker research |
| ASIC (custom AI chip) TAM anchor, 2027E (three-source overlap) | $70–90B | Company disclosure, Broker research |
| Broadcom AI backlog (customers 1→6) | $73B+ | Company disclosure |

### 9b · The second in-house wave, and measurement discipline

The second wave differs from the first in kind: Ironwood, Trainium 3, Maia 200, and MTIA v3 are the first in-house accelerators built on the same TSMC process generation as NVIDIA's parts, and designed for inference from day one. Penetration estimates agree on direction and differ on level, depending on the unit of account: CoWoS wafer allocation 28→32% and dollar value 16→22–25% by 2027 (broker estimates). Discipline: only the dollar-value basis enters any multiplication in this report — mixed-basis arithmetic double-counts content.

### The crossover that isn't: TSMC AI revenue by customer (analyst estimates, not company-confirmed)

*% of TSMC AI revenue · GPU camp vs ASIC camp · 2025 vs 2027F*

| Year | ASIC camp share (line-chart series) | GPU camp share (composition-bar series) | 50% crossover reference |
|---|---|---|---|
| 2025 | 25% | 62.8% | 50% |
| 2027F | 32.5% | 52.5% | 50% |

*The two series come from separate sub-visualizations within the same chart card in the source and do not sum to 100% between them (a residual/other category is implied but not broken out) — reproduced here exactly as sourced, without reconciliation. Source: Broker research*

While the market debates GPUs versus in-house ASICs, the Taiwanese design-service pair taping out for every camp is already booking the revenue: GUC posted a record NT$12.4B quarter in 2025Q4 and +62.9% year over year in 2026Q1; Alchip's −40.5% in 2025 is part of the same story — the tail of the Trainium 2 program, because design services are inherently a project-based, saw-toothed business (the same tooth that cut Alchip −19% in FY2018 on the Bitmain unwind) — with 2nm engagements already in design.

> Lead customer Amazon AWS has pulled its 2nm design forward and hopes to finalize the design by year-end. (translated from the original Chinese)
>
> — Alchip results call, March 2026 (as relayed by Morgan Stanley research), 2026-03-23

**Context:** At its March 2026 results call, Alchip management disclosed that AWS had advanced its next-generation in-house chip to the 2nm design-finalization stage — just as Trainium3 (3nm) was entering volume production.

**Why it matters:** The design-services frontier has moved from 3nm production to 2nm finalization: cloud in-house ASICs now track the merchant-GPU process cadence exactly. The 2003 history of structured ASICs losing to a process-node gap has not repeated this time.

### 9d · Deep dive: why the cadence mismatch is manageable

Models iterate in months; chips take years to tape out (release the design to the fab). The market's core concern is that a full custom-silicon cycle — design, tape-out, qualification, production — cannot keep up with model architecture. The record says the mismatch is absorbed by three layers: a stable operator core (matrix multiplication has anchored workloads for a decade), engineering compression (separate training and inference tracks cut the cadence to roughly twelve months), and system absorption (compilers and interconnect). Eight TPU generations crossing three paradigm shifts — CNN, RNN, Transformer — are the hardest evidence available (the full eight-generation record now lives in §6). The table below puts the per-GW economics of the leading camps side by side — analyst estimates, not guidance.

### Per-GW economics · two ways to spend the same gigawatt

*per 1 GW build · analyst estimates*

| Metric | Rubin | TPU v7 | Read |
|---|---|---|---|
| Dies / GW | ~0.6M | ~1.2M | ≈2× the silicon for 1 GW |
| Rack ASP | ~$6mn | ~$2mn | density vs volume — two valid answers |
| TSMC revenue / GW | ~$1.1bn | ~$1.9bn | the constant in both answers |

*Source: Broker research*

**Load-bearing assumption:** the argument that the mismatch is manageable (customer volumes large enough to amortize NRE — the one-time engineering cost of a custom chip) and the demand thesis (capex continuation) share the same supporting column. If capex retreats, demand falsification and mismatch failure arrive together.

### 9e · Deep dive: four supply gates — the profit pool sits at the gates, not in the cloud

At the end of 2023, CoWoS capacity of roughly 14,500 wafers per month was the industry's binding constraint; capacity has expanded six-fold in two years and TSMC still calls it "very tight" — the opposite of 2001, when capacity flipped to surplus overnight. Supply rigidity ranks: HBM > advanced process > CoWoS > optical interconnect — ranked not by score but by whether a workaround exists◆.

### The four-gate ladder · rigidity is the ranking

*blocks = six-question score · solid = no bypass*

| Rank | Gate · basis | Score | Bypass routes | Base / conservative |
|---|---|---|---|---|
| 1 | **HBM** — Three-maker oligopoly + HBM4 wafer conversion penalty of ~30% + Goldman Sachs DRAM gap 2027E −3.3%; no bypass route | 10/10 | NO BYPASS | base: tight · conservative: eases last |
| 2 | **Leading-edge process** — TSMC sole source; 3nm utilization at 101% in 2026Q4 (140–150K wpm 2026E, cleanroom-capped); 2nm is the only outlet within two years | 10/10 | NO BYPASS | base: tight · conservative: eases last |
| 3 | **CoWoS** — Demand +93% in 2027E, but OSAT outsourcing and Intel EMIB provide real bypasses | 8/10 | OSAT outsourcing; Intel EMIB | base: tight · conservative: eases first |
| 4 | **Optical interconnect** — Multi-supplier competition, the copper/optics split unresolved, optics content rising only gradually | 7/10 | Multiple suppliers; Copper/optics coexist | base: tight · conservative: eases first |

*Source: Broker research*

### Gate three in physical form: CoWoS monthly capacity — six-fold in two years, still "very tight"

*kwpm · hollow = forecast*

| Period | Capacity (kwpm) | Multiplier vs 2023 |
|---|---|---|
| YE2023 | 14.5 | — |
| YE2024 | 37.5 | ×2.6 |
| YE2025 | 77.5 | ×5.3 |
| 2026E | 92.5 | ×6.4 |
| 2027E | 135 | ×9.3 |

*Source: Company disclosure, Broker research, Industry & official*

HBM is the single most scenario-sensitive variable. The three memory makers' capacity nearly quintuples in three years, HBM4 carries a $15.4/GB price anchor — and HBM4E has no 2027 price anchor at all; the year without an anchor is the year pricing discipline is most fragile. Memory-cycle history offers no example of block capacity releases ending gently. When the binding constraint is ultimately DRAM, the mirror to study is the memory cycle.

The constraint's latest migration shows in the sell-side field work. Morgan Stanley's Asia supply-chain tour (2025-12-02) lifts its 2026 CoWoS forecast to 125K wafers per month — +79% on the ~70K exit rate of 2025 — while its power-deployment arithmetic implies annual CoWoS demand of roughly 681K wafers against nearly 1.1M of combined TSMC and non-TSMC capacity; in that read CoWoS is no longer the binding gate, and the shortage has moved upstream to 3nm front-end wafers (2025 ~110–120K per month → 2026E 140–150K, with cleanroom space the hard limit) and to materials such as T-glass. The two framings are meant to stand side by side: the sell-side allocation math says the gate has moved upstream — TSMC's official wording still says "very tight" (broker research).

### HBM: from supporting part to two-fifths of DRAM revenue

*slabs = stack height (Hi) · hatched = estimate · 2023 vs 2026E*

**Generational stacking**

| Generation | Era | Stack height |
|---|---|---|
| HBM2 / 2e | 2016 / 2020–21 | 4Hi |
| HBM3 | 2022 | 8Hi |
| HBM3e | 2024 | 12Hi |
| HBM4 | 2025–2026 | 16Hi |

**HBM share of DRAM revenue**

| Year | Share | Revenue |
|---|---|---|
| 2023 | 8% | ≈$4.0–5.5B |
| 2026E | 41% | ≈$46B |

*Source: Industry & official*

### 9f · The constraint's last stop: the grid

The most direct first-person testimony in this report: the shortage is no longer chips, it is powered shells — datacenter buildings with electricity to plug into.

> It's not a supply issue of chips; it's actually the fact that I don't have warm shells to plug into.
>
> — Satya Nadella, CEO, Microsoft (BG2 podcast, alongside Sam Altman), 2025-11-03

**Context:** November 2025: the CEO of the world's largest AI capex spender admits on a podcast that GPUs sit in warehouses with no powered racks to plug into.

**Why it matters:** The strongest first-person testimony of this cycle's constraint migration: when the buyer is Microsoft, the inventory is GPUs, and the bottleneck is electricity, the cycle's metronome has moved from TSMC's fabs to the grid dispatch room — a structure that never occurred in 1995–2000.

The IEA projects datacenter electricity use of roughly 945 TWh by 2030 — more than double 2024's 415 TWh, comparable to Japan's national consumption. A GB200 NVL72 rack draws about 120 kW, roughly sixteen times a typical enterprise rack. But power is a deployment metronome, not a shipment metronome — there is as yet no quantified case of power constraints canceling chip orders. It is the central variable of the "different-case" scenario, not a peak signal of the "same-case."

### The last stop: power delivery meters the build-out

*GW · 2024A–2030E · named access/framework commitments — not signed new-power contracts*

| Buyer | Commitment | Terms |
|---|---|---|
| OpenAI | 10 GW | framework · first deployment end-2026 |
| Anthropic | 5 GW | from 2027 · verbatim in Broadcom FY2026Q2 call |
| Meta | 3 GW | to end-2028 · Broadcom call customer map |

*One measurement basis: named access / framework commitments — deliberately not mixed with signed new-power signings. GW-to-units conversion carries ±40%.*

**The constraint's mechanics — why delivery, not silicon, sets the tempo**

| Fact | Detail |
|---|---|
| 120 kW | per GB200 NVL72 rack — ~16× a typical enterprise rack |
| 18–24 months | to build & power one datacenter shell — capital ready ≠ shell ready |

> "It's not a supply issue of chips; it's … warm shells to plug into." — Satya Nadella, Microsoft CEO · 2025-11 · T3 podcast transcript

▲ Reinforces: interconnection queues lengthen + capex holds, two quarters
▼ Weakens: power contract prices roll over + GPU inventory clears

*Source: Company disclosure, Industry & official*

---

## S10 · Deep dive · The consensus, stress-tested

### Three bold assumptions

The consensus case rests on three claims: margins follow the silicon, the boom goes broad-based, demand is visible to 2028. The evidence grades them fail, reverse, and late.

### A1 · "Margins follow the silicon"

The claim, as the market trades it (MediaTek +240%, GUC ×3.5): owning ASIC exposure is owning the economics of compute. The revenue is real — Broadcom's AI line grew +143% to $10.8B with a $16.0B guide◆ — but the margin structure runs the other way: Citi's build puts custom-silicon gross margin at 62.5% versus 77% for non-custom semiconductors (FY26–28E), and the dilution is already printing — group gross margin stepped down ~310bp in a single quarter as AI mix rose◆. Volume up, margin down is not a risk case; it is the current quarter. Marvell's 64–66% gross-margin target was never withdrawn, just replaced with "a path to about 60%" — gross-margin prints since: 59.7% → 59.0% → 58.9%, with interconnect (>70% GM), not custom silicon, named as the growth engine◆. Design services confirm from below: GUC 2025Q4 GM 19.0%, Alchip swinging 38.5 → 18.8 → 50.2% with mix◆. (Five of these figures come from one bank's models — Citi; the direction, not the levels, is the load-bearing claim.)

### A2 · "The boom goes broad-based"

The claim: a customer count going 1 → 6 reads as the boom broadening beyond one buyer. The dollar evidence runs the other way: Google's share of Broadcom revenue rose 8.6% → 16.2% → 24.3%, and keeps rising toward ~40% by FY2026E, ~43% by FY2027E, and ~47% by FY2028E (broker estimates) — while the fourth customer alone committed >$21B across two quarters◆. More customers should ordinarily mean less concentration; in AI inference silicon that may not hold — the broad-based boom is still one buyer's procurement decision, multiplied. The 2027 unit-crossover milestone this narrative trades on (Guosen's 58%, J.P. Morgan's chart title) is itself undecidable on public evidence: after bidirectional correction the 50% line lands at TPU ≈ 8.0–8.4M units, six in-window estimates span 6.5–15M, and external arbiters split 2028 (Counterpoint) and 2033 (Bloomberg)◆. Google has never disclosed TPU units — monitored as narrative on the §10 board.

### More logos, same centroid: adding customers did not dilute concentration

*left: customers · right: % of revenue · open = estimate*

| Year | Broadcom XPU customer count |
|---|---|
| 2023 | 1 |
| 2024 | 3 |
| 2025 | 5 |
| 2026E | 6 |

| Fiscal year | Google's share of Broadcom revenue |
|---|---|
| FY23 | 8.6% |
| FY24 | 16.2% |
| FY25 | 24.3% |
| FY26E (estimate) | 40% |
| FY27E (estimate) | 43% |
| FY28E (estimate) | 47% |

*Source: Company disclosure, Broker research*

### A3 · "Demand visibility into 2028"

The claim: named gigawatt commitments make the broad-based ramp look bankable — Anthropic 5GW, OpenAI 10GW, Meta 3GW◆. The counter is a pattern, not a number: the demand that must fill the gap between today's proven axis and the advertised boom is exactly the kind that runs late — timing, not cancellation. Alchip has logged two milestone slips (2025Q2, 2026Q1); the Maia line attributed to Marvell was delayed twice under Microsoft before its 2027 ramp — the record keeps the slip, not the blame◆. The floor is hard — Broadcom's own $73B backlog and Anthropic's >$10B/$11B orders are real◆ — but it sits on the axis already proven. The visibility gap is everywhere else.

**Interactions.** The three verdicts are not independent: A2's concentration is built from the same commitments A3 grades late; A1's profit pool embeds A3's demand path. When capex retreats, all three are tested at once (§9d's load-bearing note, generalized).

---

## §9 · Verdict

### Forty-two years in one table; the verdict in two scenarios

Every episode of non-linear demand ended at a supply constraint; every shakeout since 1985 cleared through acquisition — what changes is where the constraint sits and which tools do the consolidating.

Set the six windows side by side and three columns rhyme: demand trigger, supply constraint, clearing mechanism. The nearest match to the current cycle is a superposition — 1995–2003 on the demand side, 2019–2022 on the supply side. Two candidate windows were examined and rejected — 1997–98 for mechanism mismatch (a commodity DRAM price-inventory cycle; the memory mirror is carried in §9e, not this table), 2008–09 for thin evidence in the design-logic duopoly (Xilinx roughly flat, Altera −12.6%) — and the reasons stay on the chart.

### The comparison matrix: seven windows × five dimensions

*blue = same mechanism · hatched = partially comparable · grey = no counterpart · current window = reference*

| Window | Demand trigger | Supply constraint | Peak → trough | Clearing mode | Alignment |
|---|---|---|---|---|---|
| 1960–1984 | Moore's-law cost curve + PAL glue logic | Vertically integrated IDM capacity | 1984 $25B peak → 1985 −17% | US–Japan trade accord + product mix upgrade | — |
| 1985–1995 | PC wave + compressed design cycles | Foundry capacity (UMC/TSMC joint ventures) | 1990–91 growth stall (no negative year) | Six startups sold or vanished; a duopoly formed | — |
| 1995–2003 ★ | Optical-communications capex bubble | 90nm/300mm not yet in place | 2001: both duopolists −39% | ASIC camp cleared out; structured-ASIC experiments failed | Closest demand match |
| 2004–2012 | 28nm replacement wave + SoC integration | TSMC 28nm yield ramp | 2012 mini-cycle −13.6% | Challenger graveyard (Tabula et al.) | — |
| 2013–2018 | Deep-learning inference demand emerges | Three supply routes: GPU/ASIC/FPGA | 2019 industry −12.1% | Consolidation by giants (the Intel acquisition chain) | — |
| 2019–2022 | Pandemic remote-everything + AI | Industry-wide shortage; 20+ week lead times | 2022H2 PC −19.5% triggered the reversal | M&A supercycle + regulatory ceiling | Closest supply match |
| 2023–2026 (current) | Generative-AI inference | CoWoS/HBM → power and datacenter shells | No peak yet (NVIDIA data-center segment +92% in 2026Q1) | License-plus-talent quasi-acquisitions | reference |

*Source: Kimi Research*

### Scenario arithmetic: base case 3.0–4.3× over three years

Take the dollar path of hyperscaler capex, multiply by the dollar share captured by custom silicon, and downstream ASIC demand lands at 3.0–4.3× over three years in the base case (midpoint ~3.6×), and 2.0–2.4× in the conservative case. A 2001-scale contraction was examined and set aside — on current evidence its probability is very low, and this edition does not carry it. The kill switch is explicit: if 2027 capex growth at the top four cloud buyers falls below +14%, the base case yields to the conservative case — a deliberately early proxy: the underlying identity solves to +13.3%. The multiplication chain, its sources, and its dates live in the drill-downs across this report.

---

## §10 · Monitoring

### Trend falsification register — per-name numeric triggers

> The value of research is knowing one quarter earlier when to change our mind.

The monitoring board converges this edition from twenty-seven lines to eight falsification triggers — demand, supply-gate, company, and paradigm — each carrying its falsification condition, its current reading, and its next observation window. The financial-constraint gauge rides inside the financing trigger (top-four capex-to-operating-cash-flow at 0.71, Amazon at 1.02 — caution above 0.8, binding above 1.0); the 2027 unit-crossover claim survives as the numerator-convergence trigger after three rounds of adversarial review (A2); and the per-company tripwires collapse into three delivery checks — MediaTek, Alchip, Broadcom. Any breach routes back to §9 and advances its scenario. The leading indicator of a peak lives in order behavior, not in revenue — and order behavior is precisely what this cycle's prepaid contracts hide — the eight triggers are the observable proxies.

*trend-level falsification conditions, not trading stop-losses · any breach forces a downgrade review at the next revision; a met reversal condition restores it*

| Name | Observation window | Falsification condition | Current reading | Why it matters |
|---|---|---|---|---|
| Broadcom | FY2026Q3 delivery | AI revenue must land the guided step-up | The margin dip must prove one-time mix, not a slide | The arms dealer's print sets the chain's tone |
| Broadcom | Inventory & pre-build | Balance sheets confess what guidance won't | Days have climbed at the leader for three straight quarters | The 2001 bust was an inventory story first |
| MediaTek | 2026Q4 ASIC ramp | The guided second-half step-up is the first hard verification | The Taiwan design chain's narrative rides on this print | The street's high line sits ~70% above the company's own |
| Alchip | 3nm ramp & NRE milestones | Two milestone slips on file — a third is an automatic red light | NRE leads production revenue by three to four quarters | The sawtooth's next tooth forms here |
| TSMC | 2027 CoWoS capacity & demand | The 2026-07-16 call frames next year's capacity and AI demand | Any softening of 'very tight' is the first supply-side tell | Supply rigidity is this cycle's anti-2001 anchor |
| Sector | Financing circularity | Supplier-financed demand is being priced like purchase orders | The circularity unwinds before the demand it finances | Watch the financing, not the press releases |
| Sector | Cancellation & volume-cut spread | Isolated cuts so far — no spread yet | Two flagship cuts in one quarter advances the same-case | Or two hyperscalers turning 'digest / pause' together |
| Sector | TPU 2027 numerator convergence | Estimates straddle the crossover line exactly | Company-level unit disclosures: zero | Monitored as narrative |
| Standing rule | Red-light discipline | Two slips on file — no third benefit of doubt | Maia is the industry precedent | Alchip has two on file (2025Q2, 2026Q1) |

*Source: Kimi Research*

---

## §11 · Company deep dives

### Six companies on the supply chain's toll roads

Customer structure, project stage, revenue recognition, moat, key risk, and room to grow — descriptive analysis; deliberately no price targets.

Broadcom anchors the custom-ASIC franchise; Marvell, MediaTek, GUC, Alchip, and VeriSilicon occupy distinct positions in the design-service value chain. The COT (customer-owned tooling) model — the customer owns architecture and IP, the design house implements — appears in the MediaTek and GUC cards. The two Taiwan design houses are pointed at different workloads: Alchip's book leans GPU-style parallel compute, GUC's leans CPU-side. Figures are drawn from company disclosures and dated broker research. Market data as of July 10, 2026.

**The NVIDIA entanglement.** Three of the six — MediaTek, Marvell, and Alchip — are official NVLink Fusion partners (GUC appears on the ecosystem page): NVIDIA has opened its scale-up interconnect, switches, MGX racks, and cluster software to third-party XPUs (official, 2025-05-18), and AWS's public roadmap puts Trainium4 on NVLink 6 and MGX (2025-12-02) — third-party ASICs entering NVIDIA's platform while competing with it for the compute die. The boundary this report keeps: as of 2026-07-13 there is no first-party evidence that NVIDIA designs any cloud customer's custom AI compute die — teams and talks exist, a design win does not; and for the partners, a logo is not a design win — an ecosystem credential books no revenue. NVLink Fusion's pricing and attach rate are undisclosed; until disclosed they are scenario variables, not revenue lines.◆◆

### Deep dives: six companies on the supply chain's toll roads

| Company | What it is in this chain | Customers | Key risk |
|---|---|---|---|
| **Broadcom** (AVGO) | The definer of custom ASICs: 80–85% share of high-end custom silicon, plus the AI-networking franchise (~33–40% of AI revenue) | XPU production customers grew from 1 to 6 in 12 quarters. | Upside and downside share one source — Google concentration (24% of revenue, heading toward ~40% by FY2026E) |
| **Marvell** (MRVL) | Industry number two (10–12% share) running three engines along the AI-server interconnect path: custom XPU silicon, XPU-attach, and interconnect | Three US hyperscalers, only partially named. | Gross margin diluting 65.5% → 58.9% (Citi FY2029E 55.7%). |
| **MediaTek** (2454.TW) | The transition case with the widest expectations gap: a handset-SoC cash cow re-defining itself as an AI silicon supplier | Google is the only confirmed customer, two years in. | Effectively single-customer AI exposure. |
| **GUC (Global Unichip)** (3443.TW) | Design services grown on TSMC's line (TSMC holds 34.8%): thick-margin NRE plus thin-margin turnkey volume, with 3nm wafers ramping | The AI story is CPU, not XPU: Google Axion back-end services plus a second large US CSP. | Structural margin decline under pass-through [cost] mode. |
| **Alchip** (3661.TW) | The most concentrated single-customer bet: NRE is the profit engine, production the revenue engine, and gross margin is mix-dependent | Widely identified with AWS Trainium (sell-side inference plus media identification). | Position certainty is not earnings certainty: NRE milestone timing is the sole swing factor, with two tape-out delays on file. |
| **VeriSilicon** (688521.SH) | The scarce A-share design-services asset, run as a SiPaaS dual engine: IP licensing (92.7% GM in H1 2025) as the profit base, with turnkey volume as the second engine | Dispersed rather than concentrated (top five 44.5%, largest single 20.2% in FY2024), skewed to consumer electronics | Three consecutive loss years with rigid costs. |

*Descriptive analysis only. Figures are drawn from company disclosures and dated broker research; no valuation targets are expressed or implied.*

*Source: Company disclosure, Broker research*

---

## Appendix · Sources & method

### Method, gaps, and sources

**Method.** This site is the interactive edition of a forty-two-year cycle reconstruction (six windows, each rebuilt on what was knowable at the time) combined with an ASIC sector deep dive. Hindsight statements are labeled as such. The 2027 unit-crossover claim additionally passed three rounds of adversarial review, summarized in S10 (A2). No buy, sell, or hold recommendation is expressed or implied.

**Source discipline.** Every figure carries one of four source classes: Company disclosure — filings, earnings calls, and IR materials; Broker research — named by class only; Industry & official — SEMI, WSTS, IEA, SemiAnalysis, TrendForce, DigiTimes, and government publications; Kimi Research — synthesis that belongs to none of the above. Anything outside these classes is listed explicitly.

**Measurement discipline.** Penetration multiplication uses the dollar basis only. TPU shipment estimates (6M/8M/12M units) are listed side by side without reconciliation. CoWoS and HBM institutional estimates differ ±10–20%; both are shown. Scenario anchors: base 3.0–4.3× (three-year, midpoint ~3.6×), conservative 2.0–2.4×; a 2001-scale contraction case was reviewed and set aside as a low-probability tail. Kill switch: top-four 2027E capex growth below +14% (identity solves +13.3%, rounded up) retires the base case.

*Interactive research edition · Data as of 2026-07-12, updated 2026-07-14 · Contains no investment advice*

*Converted to Markdown with assistance from Claude (Anthropic).*
