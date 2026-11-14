# DEBRIEF-space-mars

A DEBRIEF mission record (protocol https://github.com/Nervous-Machine/DEBRIEF): sixteen pre-registered learning cycles
on the radiation dose measured by the Curiosity rover's RAD instrument at Gale Crater, Mars, run in July and August
2026 over a full Mars year of about forty-three thousand dose measurements. The ledger is `ledger/mars.json`;
everything else is rendered from it.

**Briefing video:** https://youtu.be/OekEgqZeIfw. The record told out loud: what was learned, what is open, and what
is being asked for.

**Standing.** Certified 0. Accepted 8. Refuted 3. Open gaps 5. Every cycle wrote
its question and pass rule down before touching the data, and each finding carries the rule it passed. Nothing is
certified: no relationship has earned certainty yet, and nothing has been rerun by anyone outside the operator. Both
are open asks below.

**Record quality: full ledger.** Sixteen cycles and one operator audit, each with a commit reference. The code of cycles one to nine is in the operator's working repository at the referenced commits; the code of cycles ten to sixteen is not, so their results stand as accepted and not certified until someone reruns them. Anyone may.

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

- **A rerun.** The strongest contribution is a rerun of the cycles from the public RAD data (PDS) under the registered
  rules, on your own machine, reported with the **Rerun report** issue form. Cycles ten to sixteen are the ones nobody
  has rerun; a pass makes them certified, a miss is recorded as a miss, and either enters the ledger under your name.
- **Data.** Any dose, plasma or dust series at Mars for 2024 that bears on an open gap, offered with the **Data
  contribution** form. The data need not be uploaded; the cycle records where it lives, its provenance and your terms.
- **A refutation.** If a finding does not hold under its own rule, say so through the Rerun report. Refuted is a
  standing in this protocol, not a failure of the record.

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
