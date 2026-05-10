# Tennis Pivot Tracker

Tennis Pivot Tracker is a lightweight match-charting tool for coaches who want clearer post-match conversations without turning every point into a full video-analysis project.

It focuses on the moment a point changes: the serve, return, shot choice, pressure situation, or opponent quality that shaped the outcome. The goal is practical coaching clarity: one pattern, one action, and a better next session.

## Why a coach might use it

- Track matches live from a phone or tablet with a compact four-tap point flow.
- Separate coachable errors from opponent quality.
- Keep score, serve context, pressure tags, and pivot codes in one place.
- Review the match through simple summaries instead of raw point noise.
- Export match data for later review or sharing across devices.

## What it captures

The app uses a player-centered MPTS 2.0 flow:

1. **Momentum** — did the player take control, give up control, lose to quality, or play a routine point?
2. **Shot or phase** — serve, return, forehand, backhand, transition, or net.
3. **Detail** — a focused code such as direction, depth, decision, double fault, ace, or forced error.
4. **Outcome** — whether the player won or lost the point.

The tracker also records automatic context such as:

- Current score, games, sets, and match status
- Server and first/second serve usage
- Break points, game points, set points, match points, deuce, and advantage
- Big points marked manually by the coach

## Coach-facing outputs

### Record

Enter each point through a guided flow while the live score updates automatically.

### Sheet

Review a chronological score sheet with point codes and pressure context.

### Stats

See practical summaries, including:

- Total and big-point results
- Lucky wins and quality losses
- Top shot leak
- Serve and return splits
- Break-point and pressure-point records
- Pivot-code breakdown by points won and lost

### AI Coach

Optionally connect a Gemini API key stored only in the browser. When used, anonymized match stats are sent directly from the browser to Gemini to generate concise live-match cues or a fuller set/match review.

AI support is optional; the tracker works without it.

### Guide

Use the built-in guide to keep point coding consistent across matches and coaching staff.

### Matches

Create, revisit, delete, import, and export match files as JSON.

## Match formats

New matches can be configured by:

- Match length: one set, best of 3, or best of 5
- Deciding-set rule: normal, 7-point tie-break at 6-6, or 10-point tie-break at 6-6
- Game scoring: regular deuce/advantage or golden point/no-ad
- First server: player or opponent

## Getting started

No installation or build step is required.

1. Open `index.html` in a modern browser.
2. Go to **Matches**.
3. Tap **+ New Match**.
4. Enter the player, opponent, date, match format, scoring format, and first server.
5. Use the **Record** tab to chart points.
6. Review the **Sheet**, **Stats**, and optional **AI Coach** tabs during or after the match.

## Data and privacy

- Match data is stored in the browser using `localStorage`.
- Data stays on the device unless you export it or use the optional AI Coach feature.
- Exported match files are JSON and can be imported back into the app.
- Gemini API keys, if entered, are stored only in the browser.
- AI Coach sends anonymized match statistics directly from the browser to Gemini when a summary is requested.

## Coaching philosophy

This is not a full symmetric match-charting system and it is not designed to replace a coach's judgment. It is intentionally selective: capture the most actionable point pivot, then use the pattern to guide the next conversation or training block.

The recommended review rule is simple:

> One pattern. One action.

## Repository structure

- `index.html` — the complete app: HTML, CSS, and JavaScript
- `README.md` — project overview and usage notes
- `LICENSE` — MIT license

## License

This project is licensed under the MIT License.
