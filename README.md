# The Accurate Selection — CSS Selectors Challenge (Temani Afif)

Community-authored challenge. **Temani Afif** is an expert web developer and one of the most active users in the CSS tag. He’s the creator of css-loaders.com, css-generators.com, css-tip.com, css-pattern.com, and more.

You’re given an array of **100 numbered boxes** (1–100). By default, boxes **15–28** are red and the rest are **light blue**.

## The challenge

Solve **10 selections** with increasing difficulty using **CSS only**. A `<select>` has 10 options; for each option, your CSS must color the **corresponding items** (e.g. red). Any approach is fine as long as the right items are colored when that option is selected.

**Example** — “Color the first item in red”:

```css
select:has(option[value="0"]:checked) ~ .container > div:nth-child(1) {
  background: red;
}
```

## The 10 selections

| # | Selection |
|---|-----------|
| 1 | The last item |
| 2 | The first 10 items |
| 3 | All items except the first and last one |
| 4 | The items with a **prime number** |
| 5 | The items **without "5"** in their number |
| 6 | The items whose **sum of digits = 8** |
| 7 | The **first item of each row** |
| 8 | The **items of the second row** |
| 9 | The **first half** of the items (e.g. 56 items → first 28) |
| 10 | The items that form a **checkerboard** (e.g. even positions red in one array, odd in another) |

## Rules

- **Only CSS.** Do not change the existing HTML/CSS structure (container, items, padding, margin, size). Only add/change rules that **color** items.
- Must work in **at least one** major browser (Chrome, Firefox, Edge, Safari).
- Must work for **any number of items from 1 to 100** (template has 100; tests may use a random count).
- **Container width is variable** (e.g. `50%`, `756px`); number of items per row is not fixed.
- **Submission:** Use [JSFiddle](https://jsfiddle.net/) only. Fork the [starter template](https://jsfiddle.net/eh0xqk9y/), add your CSS, and submit the link. The code in your answer must match the fiddle.
- **Deadline:** April 13, 2026.
- Your entry must not be written by AI.

## How to submit

1. Add your CSS (and a short description per selection if you like).
2. Include the **full runnable code** link: `https://jsfiddle.net/...`
3. Optionally: browser(s) your solution works in; selections you didn’t solve (and your attempt).

**Example:**

```text
Here is my full CSS code:

/* selection #1 */
select:has(option[value="0"]:checked) ~ .container > div:last-child { background: red; }
...

And here is the full runnable code: [your jsfiddle link]

My solution only works in Chrome V145+ and Firefox V147+
I was unable to solve selections #7 and #10
```

## How to win

- **Winner:** Anyone who solves **all** 10 selections.
- If no one solves all, the person with the **most** solved selections wins.
- Among winners, **special mention** for the **smallest** code (by number of properties and selector length, not character count).

---

**Have fun selecting with CSS!**

For feedback on the challenge, see the Meta post.
