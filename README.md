# Daily Board

A simple tracker for things you need to do every day (crafting cooldowns, auction reposts, scav runs, workouts) and one-time tasks, grouped by character or area. Daily tasks uncheck themselves at the reset time.

## How to open it

Download `index.html` and double-click it. It opens in your web browser. No install needed.

Your checkmarks and groups are saved in that browser, on that computer.

## How the code is organized

Everything is in `index.html`, in three parts:

1. **`<style>`** (CSS): how it looks. Colors, fonts, spacing.
2. **The HTML in `<body>`**: the fixed parts of the page, like the header.
3. **`<script>`** (JavaScript): what it does. This part has numbered sections:
   1. Settings: the reset hour
   2. Data: what a group and a task look like
   3. Reset logic: decides whether a task counts as done
   4. Actions: add, check, delete
   5. Drawing the page
   6. Start

## Changing the reset time

In the script, find `const RESET_HOUR = 0;` and change `0` to any hour from 0 to 23 (for example, `15` for 3 PM).
