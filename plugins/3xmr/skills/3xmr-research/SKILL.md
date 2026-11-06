---
name: 3xmr-research
description: Use when the user wants to research a market or trading idea with 3XMR, or asks what 3XMR can do. Starts every session by asking the 3XMR server who the user is and what it offers.
---

# Working with 3XMR

1. Call the 3XMR `whoami` tool first. If the user is not signed in or their
   invitation is still pending, say so plainly and point them to
   https://lab.3xmr.com/join/. Do not retry in a loop.
2. Call `guide` next and follow the workflow it returns. The server's own
   descriptions are the source of truth for which tools and data exist; do not
   promise features the server does not list.
3. Keep work private unless the user explicitly chooses to share it.
4. Report results with their evidence: data sources, time ranges, costs and
   what would prove the idea wrong. A test result is not a recommendation to
   trade, and no 3XMR tool places orders.
