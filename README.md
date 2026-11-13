# Joe's Pizza

A browser game about running a pizza counter. Joe handed you the keys: read the order tickets, build the pies, bake them to golden, and serve them before customers walk out. Cover the rent every night or the shop closes.

## Play

Open `index.html` in any modern browser. There is no build step and nothing to install. It also works as-is on GitHub Pages.

## How it works

1. **Read the ticket.** Customers clip orders to the rail. Each ticket lists sauce, cheese and toppings, plus a patience bar.
2. **Build it.** Stretch dough, then add red sauce, mozzarella and the toppings on the ticket. Extra or missing toppings mean no sale.
3. **Bake it.** Put the pie in the oven and pull it while the needle is in the green. Pale or dark pies still sell but earn no tip. Raw or burnt pies get sent back.
4. **Serve it.** Tap the pie on the pass, then tap the ticket.

Each shift runs from 11 AM to 9 PM (two minutes of real time). Rent comes out at closing and goes up each day. New toppings unlock on days 2, 3 and 4, and customers get pickier and more frequent.

Between days you can spend your cash on upgrades: a hotter oven, a stone deck, a third oven deck, a jukebox (more patience), pre-sauced dough, a tip jar, and a neon sign (rating boost).

You lose if you cannot cover rent, or if your rating drops below one star.

### Keyboard

| Key | Action |
| --- | --- |
| D | Stretch dough |
| S | Red sauce |
| C | Mozzarella |
| 1 to 8 | Toppings |
| B | Into the oven |
| X | Bin the pie on the counter |
| P or Esc | Pause |

## Tuning

The balance numbers live near the top of the script in `index.html`: `DAY_LEN`, `rentFor()`, `bakeSpeed()`, `spawnGap()`, `makeOrder()` (patience and order size), `priceOf()`, and the `UPGRADES` list.
