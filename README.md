# Daybook

A personal dashboard: live clock, task list, scratch notes, quick links, and a
view of my GitHub repositories.

Source: `dashboard/index.html`

## Published page

The dashboard runs as a private Claude artifact:
https://claude.ai/code/artifact/d2e6ce35-c036-4cbc-a103-42f1626ee910

Tasks, notes and links persist through the artifact `db` capability, so they
follow the page across devices and sessions. Opened as a plain file outside
that runtime, the page falls back to `localStorage` and says so.

## Repository panel

The repository list is a snapshot captured on 6 September 2026 — names,
visibility and last-push timestamps. Relative ages ("9m ago", "55d ago")
recompute in the browser, so they stay correct; the underlying list only
changes when the page is republished.
