---
name: 3xmr-research
description: Use when the user wants to research a market or trading idea with 3XMR, or asks what 3XMR can do. Starts every session by checking the user's account and entitled capabilities on the 3XMR server.
---

# Working with 3XMR Research

1. Call `whoami` first to confirm account identity, live capabilities, and
   entitled datasets. If the user is not signed in or has no approved access,
   say so plainly and point them to https://lab.3xmr.com/join/. Do not retry
   in a loop or invent observations.
2. Call `guide` next and follow the workflow it returns. Treat the server's
   own descriptions as the source of truth for which tools and data are live;
   never promise undeployed compute or unavailable venues/dates.
3. Keep research private by default. Only share findings when the user
   explicitly chooses an opt-in sharing action.
4. Distinguish drafted strategy plans from executed experiments. Report
   findings with full provenance: venue, pair, UTC window, event vs ingest
   clocks, units, missingness, costs, and what would falsify the idea. A
   historical result is not a trade signal or profit guarantee, and no 3XMR
   tool places orders.
