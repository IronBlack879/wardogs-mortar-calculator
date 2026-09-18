# War Dogs Range Calculator

A web-based fire-control tool for **War Dogs** mortars and artillery. Paste the coordinates of your position and your target and it instantly returns the exact range (RNG) to dial in.

https://ironblack879.github.io/wardogs-range-calculator/

## Features

- **Instant range** — paste both coordinates and read the value to set on your sight.
- **Format-friendly** — coordinates like `x94.53, y109.03` work as-is; the `x`/`y` labels are ignored automatically.
- **Weapon check** — switch between Mortar and Artillery to see whether the target is in range, too close, or out of range.
- **Height handling** — if your coordinates include a third (height) value, an option lets you pick the correct ground axes.
- **Fully client-side** — every calculation runs in your browser. Nothing is sent anywhere.

## How to use

1. In game center the map on your position.
2. Right-click and select **mark coordinates** to open the chat.
3. Press `Ctrl+A` to select all, then `Ctrl+C` to copy.
4. Paste into the matching field on the page. Repeat for the position you want to fire to.
5. Align your sight on the diamond marker and set the **RNG** to the displayed value.

## How it works

The two points form a right triangle, so the range is the hypotenuse (Pythagoras):

range = 100 × √( (Xtarget − Xyou)² + (Ytarget − Yyou)² )

Δx and Δy are the coordinate differences; squaring them makes direction irrelevant. The ×100 converts coordinate units to meters. Result rounded to the nearest meter.
Écrivez un message…

## Credits

- Method credit to [SwoleBenji](https://www.youtube.com/@SwoleBenji) for the original tutorial that inspired this tool.
- Made by IronBlack.

## I'm hungry

https://fr.tipeee.com/ironblack/
