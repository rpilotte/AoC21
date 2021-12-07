# AoC 2021: Day 7
Excel still works for Day 7

## Explanations:
Day 7 is so simple to solve the day puzzle.

Solver is the key for today.

## How it works
No real programatic possibility as Solver needs to be invoked.

Simple formula leveraging "fuel=distance=ABS(CurrentPosition-DestinationPosition)" to calculate the fuel consumption for Part 1.

For Part 2, the trick is to see that fuel=((distance+1)\*distance)/2, still with distance=ABS(CurrentPosition-DestinationPosition).

Then solver is used for minimizing the sum of all the fuel consumptions.

## Notes
I lost time as I hadn't read the text and tried to provide the location and not the consumption for part 1.
