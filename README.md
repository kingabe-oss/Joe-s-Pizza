# Joe's Pizza: The Friday Shift

A hands-on companion game for the **Business 101: How Joe's Pizza costs a product to make a profit** deck for manufacturing supervisors. Players run one catering order on Joe's line, then see what the shift really earned compared with Joe's standard cost.

## Play

Open `index.html` in a modern browser. There is no build step and nothing to install. It also works as-is on GitHub Pages.

## The setup (straight from the deck)

| | Joe's standard |
| --- | --- |
| Selling price | $12 per pizza |
| Ingredients (BOM) | Dough $1.00, sauce $0.50, cheese $2.00, pepperoni $1.00 = **$4.50** |
| Labor | $20/hour at a run rate of 20 pizzas/hour = **$1.00** |
| Overhead | Oven and shop, $30/hour = **$1.50** a pizza at 20/hour |
| **Standard cost** | **$7.00** |
| Gross profit | $5.00 |
| Other business costs | $3.00 per pizza equivalent |
| Operating profit | $2.00 |

The order is 20 pepperoni pizzas, starting at 4:00 PM. At standard, that's $240 of revenue, $140 to make, $100 of gross profit and $40 of operating profit.

## How a shift works

1. **The promise.** The caterer asks "When will it be ready?" The player picks a planning run rate: Joe's standard 20/hr, 15, 12, or (from shift 2 on) the rate they actually demonstrated last time. Joe schedules and pays labor to match the promise.
2. **The routing.** Players work the five routing steps: prepare dough, add toppings, bake, cut, box.
   - Toppings are poured by holding a key or button. Letting go in the green is one BOM portion. Pouring heavy costs real money.
   - Pizzas pulled from the oven too early must be reworked. Burnt ones are scrapped.
3. **The debrief.** When the order is boxed, a three-step debrief walks the player to the lesson instead of handing them a dashboard:
   - **Predict.** "Joe's standard pizza costs $7.00 to make. What did one of yours cost?" The player commits to a guess on a slider before seeing the answer. Their pizza is then shown next to Joe's $7 standard, split into ingredients, labor and overhead, with their guess marked. It also says whether the extra came mostly from ingredients or from time (labor and overhead, paid by the hour).
   - **Find the leaks.** Everything between Joe's standard operating profit and theirs, biggest first. Each leak is tagged Time, Promise or Material and tied to something they did: "Burnt at 4:12 PM", "your longest stretch without boxing a pizza was 11 min", "most of the heavy portions were cheese". A closing line says what share of the leak was on the clock.
   - **Pick one fix.** A run-rate slider and switches for honest promise, zero scrap and exact portions show live what each does to cost per pizza and profit on the order. The player picks the one fix they think is worth the most and locks it in. Then the game reveals what each fix was actually worth, ranked. Their pick becomes the goal for the next shift, and the next debrief opens by checking whether they hit it.
   - **See the full numbers** opens the detailed report: profit bars against standard, cost per pizza, the variance bridge, 8-hour capacity, and shift history with goals.

Being late costs overtime at $30/hr plus a 5% discount for every 15 minutes late, up to 25%. Finishing well ahead of a cautious promise still pays for the scheduled hours.

## Using it with the deck

- **Before slide 22 ("Now break the assumption"):** have people play shift 1 promising from 20/hr. Most will run well under 20, find themselves late, and see the slide 29 chain in their own numbers.
- **After slide 28 ("A promise needs a run rate the kitchen will own"):** play shift 2 from their demonstrated rate and compare the two rows in the shift history.

## Controls

| Key | Step |
| --- | --- |
| D | Stretch dough |
| Hold S / C / P | Pour sauce / cheese / pepperoni |
| O | Into the oven |
| 1, 2, 3 | Pull from that oven deck |
| K | Cut |
| B | Box |
| Esc | Pause |

Mouse and touch work too.

## Tuning

The deck's numbers and the pace of play are constants at the top of the script in `index.html`. `SEC_PER_MIN` sets how fast the kitchen clock runs. At 2 real seconds per kitchen minute, the 20/hr standard means a pizza every 6 seconds, which takes practice to hit. Raise it to make the standard easier to reach.
