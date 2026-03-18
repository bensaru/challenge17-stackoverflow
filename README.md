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
- **Submission:** Use [JSFiddle](https://jsfiddle.net/) only. **Fork** the [starter template](https://jsfiddle.net/eh0xqk9y/) (or copy & paste it). Do **not** modify the template’s HTML or its existing CSS. Only **add** your CSS (rules that color items). Submit the link to your fork. The code in your answer must match the fiddle.
- **Deadline:** April 13, 2026.
- Your entry must not be written by AI.

## How to submit

1. **Use the template as-is:** Open the [starter template](https://jsfiddle.net/eh0xqk9y/), fork it (or copy & paste into a new fiddle). Do **not** change the template’s HTML or its existing CSS — only **add** CSS rules that color the items (e.g. `background: red` / `background: lightblue`). Submissions that alter the template are invalid.
2. In the CSS panel, paste the template’s CSS (unchanged), then append your selection rules — or use the additive CSS from `submission-only.css` in this repo.
3. Add a short description per selection if you like.
4. Submit the **full runnable code** link: `https://jsfiddle.net/...`
5. Optionally: browser(s) your solution works in; selections you didn’t solve (and your attempt).

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

---

**Submission CSS (additive only)**  
This repo includes `submission-only.css`: CSS that implements all 10 selections and is written to be **added** to the [template](https://jsfiddle.net/eh0xqk9y/) without changing the template’s HTML or existing CSS. Fork the template, then paste the template’s CSS and append the contents of `submission-only.css` (or paste `submission-only.css` after the template’s CSS in the fiddle). Same behavior and features as the full demo; valid for “How to submit”.

---

**Have fun selecting with CSS!**

For feedback on the challenge, see the Meta post.
