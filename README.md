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

A run is **three Fridays**. Each Friday is a catering order for 10 pepperoni pizzas, starting at 4:00 PM. At standard, that's $120 of revenue, $70 to make, $50 of gross profit and $20 of operating profit, and about a minute of play. A full run with debriefs takes around 15 minutes.

## How a shift works

0. **A practice pizza.** Before the first shift, players make one pizza with no clock and no cost. A coach bar walks them through each routing step and highlights the control to use. That way shift 1 measures the process, not how fast someone learns the keys. It can be skipped or repeated.
1. **The promise.** The caterer asks "When will it be ready?" The player picks a planning run rate: Joe's standard 20/hr, 15, 12, or (from shift 2 on) the rate they actually demonstrated last time. Joe schedules and pays labor to match the promise.
2. **The routing.** Players work the five routing steps: prepare dough, add toppings, bake, cut, box.
   - Toppings are poured by holding a key or button. Letting go in the green is one BOM portion. Pouring heavy costs real money.
   - Pizzas pulled from the oven too early must be reworked. Burnt ones are scrapped.
3. **The debrief.** When the order is boxed, a four-step debrief walks the player to the lesson instead of handing them a dashboard:
   - **Predict.** "Joe's standard pizza costs $7.00 to make. What did one of yours cost?" The player commits to a guess on a slider before seeing the answer. Their pizza is then shown next to Joe's $7 standard, split into ingredients, labor and overhead, with their guess marked. It also says whether the extra came mostly from ingredients or from time (labor and overhead, paid by the hour).
   - **Find the leaks.** Everything between Joe's standard operating profit and theirs, biggest first. Each leak is tagged Time, Promise or Material and tied to something they did: "Burnt at 4:12 PM", "your longest stretch without boxing a pizza was 11 min", "most of the heavy portions were cheese". A closing line says what share of the leak was on the clock.
   - **Payday.** Joe's money carries over between Fridays: $100 in savings, $150 saved toward a $200 new oven, and a bank loan available up to $150 at 5% interest per Friday. Joe's plan is built on standard: each Friday's standard profit, 10 pizzas × $2 = $20, goes into the new-oven fund.
     - **If a Friday delivers less than the $20 plan, the gap is one decision.** Gap = plan - what the Friday delivered. A Friday that lost $6.61 is $26.61 short: $6.61 of unpaid bills plus the $20 deposit. Payday reconciles the gap line by line against the leaks from the previous step, plus any pizzas not delivered and loan interest. The rows always add up to the total shown. The player covers it as on slide 14: use savings (less cash for the next bad night), borrow (debt and interest grow), or take it from the oven plan (the oven is delayed). Unpaid bills must be real cash, so the oven option can only use money already in the fund plus the deposit Joe skips. If nothing can cover the gap, Joe can't make payroll and the run ends. This is slide 16, "Every unnecessary dollar of cost has to come from somewhere," made literal.
     - The cash always balances: what the Friday delivered + savings used + borrowing = bills paid + what actually goes into the oven fund.
     - **Above plan:** the extra pays down any loan, then goes into the oven fund. At $200, Joe buys the oven and the kitchen gets a fourth oven deck.

     A profitable but slow Friday doesn't create a cash gap in real accounting; the extra cost comes out of profit. What it does short is Joe's investment plan, so that's where the decision sits.
   - **Pick one fix.** A run-rate slider and switches for honest promise, zero scrap and exact portions show live what each does to cost per pizza and profit on the order. The player picks the one fix they think is worth the most and locks it in. Then the game reveals what each fix was actually worth, ranked. Their pick becomes the goal for the next shift, and the next debrief opens by checking whether they hit it.
   - **See the full numbers** opens the detailed report: profit bars against standard, cost per pizza, the variance bridge, 8-hour capacity, and shift history with goals.

Being late costs overtime at $30/hr plus a 5% discount for every 15 minutes late, up to 25%. Finishing well ahead of a cautious promise still pays for the scheduled hours.

These dollar amounts are scaled to a 10-pizza order. The deck's example uses a $10,000 oven fund for a full night with five people.

4. **The close-out.** After Friday 3, or earlier if Joe can't make payroll, the run ends with the deck's closing ideas, filled in from the player's own run:
   - **"One last time: did Joe make $12?"** Their last Friday's $12 broken into cost to make, gross profit, other costs and operating profit, against Joe's standard.
   - **Your Fridays.** Promised rate, demonstrated rate, promise kept or missed, cost per pizza, profit, and Joe's savings, loan and oven fund after each Friday, plus a line on how their run rate and cost moved.
   - **Joe's Pizza is a small factory.** The slide 32 translation table (recipe = BOM, steps = routing, pizzas per hour = run rate, and so on), with the player's numbers in a third column.
   - **A factory is a much bigger pizza shop.** A calculator for a product from their own line: standard rate, demonstrated rate, crew, labor rate, overhead and shift length give labor and overhead per unit, capacity given up per shift, and the cost of the gap per shift, week and year. It opens with example numbers marked as examples.
   - The deck's last line: **"Revenue is earned by the customer. Profit is protected by execution."**

The promise screen frames each Friday: Friday 1 starts from Joe's 20/hr plan, Friday 2 asks which number to trust after seeing the real one, and Friday 3 asks the player to prove the improvement.

## Using it with the deck

- **Before slide 22 ("Now break the assumption"):** play Friday 1. Most people promise from 20/hr, run well under it, and see the slide 29 chain in their own numbers.
- **After slide 28 ("A promise needs a run rate the kitchen will own"):** play Fridays 2 and 3, planning from what they demonstrated and working on their chosen fix.
- **With slides 31 to 36:** walk through the close-out together. The calculator works well with a real product from the room.

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
