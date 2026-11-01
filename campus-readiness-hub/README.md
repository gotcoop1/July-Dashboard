# TSC Campus Readiness Hub

A facilities & campus-readiness management app for Thompson Station Church:
request portal (problems, event setups, resets, support requests), automatic
post-event resets, verification workflow, room standards, Sunday readiness,
inspections, a unified Planning Center calendar, preventive maintenance, and
reports.

## Where the team actually uses it

The **live, working app** is the Claude Artifact, shared from its Share menu:

> https://claude.ai/artifact/W8qz5sx6aFKoF4BUkRhbbt

The app's shared database, sign-in, photo storage, and Planning Center
connection are provided by the Claude runtime. **This file in GitHub is the
source code / backup and version history** — opening `index.html` directly
from GitHub (or GitHub Pages) shows the interface but cannot save data,
sign people in, or load Planning Center, because that runtime isn't present.
To run it as a standalone multi-user web app, the data layer has to move to a
backend (e.g. Supabase or Firebase) with authentication and row-level
security.

## Brand colors

All colors are CSS variables at the top of `index.html` in the `:root` block
(and the two dark-theme blocks below it). To adjust branding, edit those
hex values in all three blocks. Current values follow the TSC Branding Guide
(Jan 2025):

| Token | Light | Meaning |
|-------|-------|---------|
| `--accent` | `#F36C42` | TSC Orange — primary actions, highlights |
| `--ink-2` | `#4F5659` | TSC Gray |
| `--c-ministry` | `#3F8EA3` | from TSC Blue `#72A8B8` |
| `--line` / `--bg` | `#DED7CC` / `#F4F1EC` | TSC Cream grounding neutral |

Type: **Montserrat** (primary brand typeface).

## Setup

1. Open the artifact link, go to **Setup** and assign the facilities director,
   approvers, category owners, and support-request owners.
2. Add campus rooms under **Rooms** (standard layout, photo, owner, "required
   for Sunday").
3. Share the link from the artifact's **Share** menu — staff/volunteers as
   *Contributor*, trusted leads as *Editor*.
