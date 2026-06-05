# honest evals

most public eval numbers are marketing. here's what I look at instead.

## red flags

- single-seed numbers
- pass@1 with temperature > 0 and no error bars
- benchmarks that fit the model's training set
- holistic comparisons with no per-category breakdown

## what I actually run

- a small private set of tasks I wrote myself
- 5 seeds, 3 temperatures, stratified by category
- compare *delta* across model versions, not absolutes
- track refusals and silent-degrades separately

## the rule

if I can't reproduce a published number on my own hardware in an hour, I don't trust it.

> the goal isn't a leaderboard. it's a decision: do I switch to this model in production?
