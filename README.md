# DEBRIEF-space-mars

A DEBRIEF mission record (protocol https://github.com/Nervous-Machine/DEBRIEF): sixteen pre-registered learning cycles
on the radiation dose measured by the Curiosity rover's RAD instrument at Gale Crater, Mars, run in July and August
2026 over a full Mars year of about forty-three thousand dose measurements. The ledger is `ledger/mars.json`;
everything else is rendered from it.

**Briefing video:** https://youtu.be/OekEgqZeIfw. The record told out loud: what was learned, what is open, and what
is being asked for.

**Standing.** Certified 0. Accepted 8. Refuted 3. Open gaps 5. Every cycle wrote
its question and pass rule down before touching the data, and each finding carries the rule it passed. Nothing is
certified: no relationship has earned certainty yet. The open asks are below.

**Record quality: full ledger.** Sixteen cycles and one operator audit, each with a commit reference. The code of cycles one to nine is in the operator's working repository at the referenced commits; the code of cycles ten to sixteen is not, so their results stand as accepted and not certified until the cycles run again.

## What is in the record

- **Learned, and accepted under a rule written first:** dose at the surface falls during solar proton events, in every
  season; solar activity pushes dose in opposite directions depending on the season; in dust season the monthly average
  of solar activity is what matters; a recovery pattern after proton events was predicted in advance and confirmed.
- **Refuted:** an earlier June benchmark in which proton events raised dose at perihelion; surface pressure as a stand-in
  for dust; the daily-average solar-wind level as a driver.
- **Two solar-wind arrivals at Mars in 2024,** February 16 to 17 and June 13, first flagged from the dose record and then
  found in MAVEN plasma and magnetometer data on those dates. No catalog of observed arrivals covers Mars in 2024.
- **Open gaps,** in `ASKS.md`, each with the kind of contribution that would close it: growing over-prediction in two
  seasons, two dust-season bumps that no public data source explains, event terms that cannot be learned at daily grain,
  and a prediction waiting on a mission that has not flown.

## Where contributions land

Two kinds of contribution move this record, and both are credited by name on every cycle that follows from them.

- **A public dataset.** Any dose, plasma, dust or atmospheric series at Mars that bears on an open gap or a
  low-certainty relationship, offered with the **Data contribution** form. The data must be public at an endpoint
  you link; nothing is uploaded here. The cycle records the link, the provenance and your terms. The keeper then
  runs learning cycles on it against the outstanding gaps, and each cycle and each finding it produces carries your
  name under `credits`.
- **A hypothesis.** One falsifiable claim about what drives the dose, with the signals that would validate or refute
  it, offered with the **Hypothesis** form. Your answers are hashed and pinned to you. If the signals are public, the
  keeper runs a learning cycle against them under your registered rule, citing you. If the measurement does not exist
  yet, the hypothesis waits in the ledger as an open gap in your name until someone makes it. All certainty and
  certification later gained on it is yours.

**Checking a finding.** Anyone can confirm or refute a finding against the public RAD data under its registered rule
and report it with the **Rerun report** form. That is recorded as independent confirmation and strengthens
`accepted`; a miss is recorded as a miss. The learning cycles themselves run through the keeper's kernel, so
`certified` is earned when the registered cycle has run on the contributed data or hypothesis, not by a rerun alone.

Every contribution is one dated cycle in the ledger under the contributor's own name, listed in `CITATION.cff` and
in each release. Rules and templates: https://github.com/Nervous-Machine/DEBRIEF/blob/main/CONTRIBUTING.md.

## Layout

```
ledger/mars.json      the ledger (protocol 0.1.0)
SCORECARD.md          findings, cycles, gaps, anomalies (generated)
ASKS.md               open gaps and what closes each (generated)
cycles/               contributed cycles, one file each
CITATION.cff          how to cite; contributors of record
LICENSE               Apache-2.0 (code); LICENSE-CONTENT: CC-BY-4.0 (ledger text)
```

## Sources

Curiosity RAD dose (PDS); MAVEN plasma and magnetometer data (PDS PPI); OMNI2 (NASA SPDF); REMS pressure (PDS); the
operator's sixteen-cycle run ledger of 2026-07-18 to 2026-08-08, with a commit reference per cycle.

## Words

This record never calls a relationship certified until it has earned certainty under a settled rule. It records what
was asked, what rule was written first, what passed, what was refuted, and what is still open.
