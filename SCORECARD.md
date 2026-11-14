# Mars RAD learning cycles

The system was asked to learn what drives the radiation dose measured by the Curiosity rover on the surface of Mars. It worked through sixteen cycles. Each cycle wrote down its question and its pass rule before touching the data. It assembled a full Mars year, about forty-three thousand real dose measurements across four seasons.

It learned four things worth knowing. First, dose at the surface falls during solar proton events, in every season. Second, solar activity pushes dose in opposite directions depending on the season. Third, in dust season the monthly average of solar activity matters where the daily value does not. Fourth, two bumps in the dose, in February and in May to June of 2024, line up with solar-wind disturbances arriving at Mars.

Two of those arrivals were flagged from the dose record first, and both were then found in independent spacecraft data on those dates. No catalog of observed arrivals covers Mars in 2024.

What it could not do is establish certainty. The fit improved season by season, but the system does not yet claim to trust any single relationship. And the size of the bumps at Mars is still unexplained.

What it needs from people is short and specific: dust data that has not been released, solar-wind measurements at Mars that will come from a future mission, a better filter on the existing spacecraft data, and a model that works hour by hour.

_Rendered from the briefing record. Items marked internal in the ledger (how the framework works, the state of the record) stay in `ledger.json` and are not shown here._

Record quality: full ledger. Sixteen cycles and one operator audit, each with a commit reference. The code of cycles one to nine is in the operator's working repository at the referenced commits; the code of cycles ten to sixteen is not, so their results stand as accepted and not certified until someone reruns them. Anyone may.

**Standing.** Certified 0. Accepted 8. Refuted 3. Open gaps 5. An open gap is an input or question nobody has settled; it is not a finding and has no standing.

## Findings

| id | kind | standing | basis | cycles |
|---|---|---|---|---|
| F1 | learned | **accepted** | learned through the gate and repeated in three seasons | 1, 2, 5 |
| F2 | learned | **accepted** | admitted under a rule written down before the data | 2 |
| F3 | learned | **accepted** | predicted in advance, both directions confirmed | 4 |
| F4 | learned | **accepted** | admitted under a rule written down before the data | 5 |
| F5 | learned | **accepted** | every registered prediction confirmed | 14 |
| F6 | retracted | **refuted** | the earlier benchmark's sign did not hold in the sixteen-cycle run: negative in all three seasons | 2, 5 |
| F7 | ruled_out | **refuted** | failed its registered test; predicted sign wrong | 6 |
| F8 | ruled_out | **refuted** | failed its registered test | 9, 10 |
| F9 | discovery | **accepted** | both arrivals present in MAVEN plasma and magnetometer data on the published dates | 12, 13, 15 |
| F10 | correction | **accepted** | correction recorded in the ledger | 7, 8 |
| F12 | correction | **accepted** | measured under a registered restatement | 16 |

## Cycles, in order

| cycle | dated | by | kind | written first | verdict |
|---|---|---|---|---|---|
| 1 | 2026-07-18 |  |  | yes | not_admitted |
| 2 | 2026-07-18 |  |  | yes | admitted |
| 3 | 2026-07-18 |  |  | yes | admitted |
| 4 | 2026-07-18 |  |  | yes | confirmed |
| 5 | 2026-07-18 |  |  | yes | mixed |
| 6 | 2026-07-18 |  |  | yes | refuted |
| 7 | 2026-07-18 |  |  | yes | unavailable |
| 8 | 2026-07-18 |  |  | yes | corrected |
| 9 | 2026-07-18 |  |  | yes | not_admitted |
| 10 | 2026-08-08 |  |  | yes | not_admitted |
| 11 | 2026-08-08 |  |  | yes | unavailable |
| 12 | 2026-08-08 |  |  | yes | mixed |
| 13 | 2026-08-08 |  |  | yes | mixed |
| 14 | 2026-08-08 |  |  | yes | learned |
| 15 | 2026-08-08 |  |  | yes | classified |
| 16 | 2026-08-08 |  |  | yes | withdrawn |

## Gaps, in the order that would settle things fastest

| priority | gap | status | closes with | who could act | signal expected | resolution by |
|---|---|---|---|---|---|---|
| 1 | The two bumps in dust season, February and May to June 2024 | immovable | dust-opacity maps for Mars Year 37, or the rover optical-depth record extended past sol 3953; solar wind measured at Mars (ESCAPADE, about 2028); a research-grade filter for MAVEN's upstream solar wind | someone who can reach the record keepers; the ESCAPADE team; an outreach note is drafted and not sent; a heliophysics collaborator |  |  |
| 3 | A prediction waiting on a mission that has not flown | proposed | ESCAPADE science data | the ESCAPADE team |  |  |
| 4 | Event terms cannot be learned at daily grain without masking | in cycle | a model that works hour by hour | the modelling team |  |  |
| 5 | Growing over-prediction in the aphelion season | in cycle | an hourly-grain model | the modelling team |  |  |
| 6 | Growing over-prediction near perihelion | in cycle | an hourly-grain model | the modelling team |  |  |

## Corrections, retractions, ruled out

- **F6** (retracted): An earlier benchmark from June had proton events raising dose at perihelion. The sixteen-cycle run found the opposite: the sign is negative in all three seasons.
- **F7** (ruled_out): Surface pressure does not stand in for dust shielding. It showed no relationship and the predicted sign was wrong.
- **F8** (ruled_out): Daily solar-wind level, and crude automatic arrival detectors, are too weak to explain the bumps.
- **F10** (correction): Cycle seven said nothing further could be tested. That was wrong: the MAVEN archive covers the 2024 window. Cycle eight corrected it.
- **F12** (correction): A suspected contamination of the calibration period was measured at five thousandths of a microgray per day and withdrawn.

_Generated by DEBRIEF tools/render.py from ledger.json; protocol 0.1.0._
