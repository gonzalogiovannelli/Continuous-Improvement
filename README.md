# Continuous improvement on a food production line

DMAIC on a breaded-food line (fish, chicken, vegetable and cheese products) at a food
manufacturer, 2016 to 2018. The company is not named; the production data is real.

## The problem, as it was given

I was hired to plan an expansion: set up a second line, buy a third one and triple the
workforce, to go from about 6 tonnes a day to 18-20. Five days in, I asked to write a
different report instead, because the target looked reachable with what was already
installed.

## Measure and analyse

Three weeks, from 1 to 23 December 2016:

- Three months of production sheets
- Security camera footage, to compare recorded stops with real ones: real stops exceeded
  recorded ones by 24%
- A Pareto of downtime: rest breaks, product changeovers, oil temperature and the forming
  machine
- A methods-and-times study per station, and an energy balance of the boilers

The problem was redefined: the plant did not need another line, it needed the one it had
to work.

## Improve: four levers, chained

| Lever | Effect | Cost |
|---|---|---|
| Reorganise rest breaks, 7 to 6 operators per shift | Running time from 826 to about 1,070 min a day | 0 |
| Redesign the moulds: 5 pieces per stroke instead of 3 | Flow from 8.06 to 13.44 kg/min, with the old machine | ~USD 100 |
| A recirculation pump: only 32% of the boilers' heat reached the fryer | The fryer can cook the new flow, without a new boiler | ~USD 500 |
| Produce in raw-material campaigns: all chicken, then all fish, then vegetable, then cheese | Each avoided raw-material change saves 1.5 h of deep cleaning | 0 |

None of them works alone: more flow without running time is not produced, more running
time without flow hits the forming machine, and more flow without heat is not cooked.

## Control

Production was tracked on paper and in personal spreadsheets. I set up an online
production record, with its first two KPIs: without one version of the data there is no
Pareto, no KPI, and no way to tell whether an improvement worked.

## Result

| | Before (Dec 2016) | After (Jan 2018) |
|---|---|---|
| Daily output | 6,113 kg on average | about 15,000 kg |
| Line operators, two shifts | 14 | 12 |
| Output per person per day | 0.44 t | 1.25 t |

About USD 600 of changes, instead of the new lines that had been planned.

`Visuals/Before-After.png` covers September 2016 to May 2017, the first months after the
changes. The 15 tonnes is the figure for January 2018.

## In this repo

| File | What it is |
|---|---|
| [`Documentation/Findings_Summary.md`](Documentation/Findings_Summary.md) | The bottlenecks found in the analysis |
| [`Documentation/Process_Flow.md`](Documentation/Process_Flow.md) | The line, step by step |
| [`Documentation/Fryer_Calculation.md`](Documentation/Fryer_Calculation.md) | The heat-transfer calculation behind the 32% |
| [`Visuals/Pareto.PNG`](Visuals/Pareto.PNG) | Pareto of downtime causes |
| [`Visuals/Workforce Stops.PNG`](Visuals/Workforce%20Stops.PNG) | Stops caused by rest breaks |
| [`Visuals/Before-After.png`](Visuals/Before-After.png) | Production and stop time, before and after |
| [`Visuals/Before_After_Comparison.xlsx`](Visuals/Before_After_Comparison.xlsx) | The data behind that chart |
| [`Visuals/Fryer_Calculations.xlsx`](Visuals/Fryer_Calculations.xlsx) | The fryer calculation |
