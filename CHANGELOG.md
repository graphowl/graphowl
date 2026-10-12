# Changelog

Dated notes on what changes in GraphOWL. Newest first. There is no packaged release yet: the demo runs build `0.1.0`, and a note is added here whenever the demo or the website changes in a way a visitor can see.

Changes made before the first entry below were not recorded publicly.

## Unreleased

- Nothing recorded yet.

## 2026-10-12 — Public demo and website open (early access)

- Website live at <https://graphowl.app>.
- Live demo at <https://demo.graphowl.app>, protected by a shared password available on request (<connect@graphowl.app>).
- The demo workspace is **Northfield Dairy Cooperative**, a synthetic dairy cooperative: farms, milk lots, quality tests, production batches and retail sales. GraphOWL scans the source database, proposes an ontology from its tables and keys, and loads a bounded sample of rows as instances of the approved classes. In the demo, the proposal is approved automatically by the demo's built-in user so that the workspace opens populated; this is not a real review.
- The source database is read through a read-only database role.
- Known limits: single-node deployment on a small host; one shared login; the demo database is reset between sessions.
