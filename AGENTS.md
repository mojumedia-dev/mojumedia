# mojumedia — agent standards

Before any substantive change to this repo, read `/c/Users/adaml/.claude/projects/C--Users-adaml/PROCESS.md`. It governs the six-phase lifecycle and the eight quality dimensions that every ship in this repo must satisfy.

## What's in this repo

- **`index.html`** — the Mojumedia marketing site (public). Deployed at mojumedia.com (or wherever Vercel points).
- **Personal deliverables Adam authored + drops here** — WGU interview prep, EverForged proposals, other career + client-facing docs he wants versioned. These are not customer-facing; they're Adam's working files.

Branch conventions:
- `main` — site-only.
- `mojumedia` (currently active) — everything: site + personal docs.

## Repo-specific rules

- **This is a static site** — no build step, HTML/CSS/JS only. Testing = open in a browser.
- **11-bot MojuCrew lineup lives here** in `index.html`. Bot descriptions are shipped copy — don't fabricate features (see `feedback_never_fabricate_facts`).
- **Pricing pills + signup/pricing CTAs were intentionally removed** (commit 344cc8d) — model is "call us to activate," not self-serve. Don't add them back without asking.
- **No em dashes in copy** — universal Adam rule.
- **Personal docs (WGU prep, EverForged proposals, career-tracking)** — commit under Adam's name, no client-facing footer.

## Test rig

None yet — it's a static site. Verify visually:

```bash
python -m http.server 8080
# Open http://localhost:8080 in a browser + mobile emulator
```

For any customer-facing HTML change, before committing:
- Screenshot at 375px width (mobile-first per `feedback_mobile_first`).
- Screenshot at 1440px width.
- Verify no console errors.

## Related

- `/c/Users/adaml/.claude/projects/C--Users-adaml/PROCESS.md` — the Mojumedia standard
- `../mojucrew-platform/` — the actual MojuCrew product these bots describe
