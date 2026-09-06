# Company Accountant — dashboard

The web view for the Telegram bot that tracks money between Mahmoud, Taha and
Mostafa.

This repo holds one static page. It stores nothing and contains no data: every
number is fetched at runtime from the project's Supabase function, which only
answers requests carrying either

- Telegram Mini App `initData` (signed by Telegram with the bot token), or
- a short-lived per-person token that the bot signs into the `/dashboard` link.

Opening this page without one of those shows nothing.

## Hosting

GitHub Pages, served from `main` / root. Send `/dashboard` in the Telegram
group to get a working link.
