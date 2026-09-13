# TASK

## Current task
Complete and validate the 新人バイトFAQ MVP v1.2 as the first production-ready prototype.

## Objective
Provide a safe, smartphone-first fixed-URL FAQ that reads only registered store data and lets a manager generate schema-compatible store JSON without AI inventing store rules.

## Current phase
Final MVP validation.

## Completed
- Fixed-URL FAQ UI with `?id=<store_id>` routing.
- Store ID and JSON `store_id` consistency validation.
- Safe rendering without `innerHTML`.
- HTTPS-only question form validation.
- Unregistered/invalid store data fails safely instead of being guessed.
- Smartphone-first manager input form.
- Manager form output aligned with `schema.json`.
- GitHub Pages deployment workflow exists.
- AI collaboration protocol aligned with AI TEAM HQ.

## Remaining validation
- Confirm the GitHub Pages deployment is live after the latest `main` commit.
- Confirm the FAQ URL with `?id=marufuku` renders the sample store safely.
- Confirm `manager.html` generates schema-compatible JSON on iPhone Safari.
- Confirm invalid/missing store IDs and invalid store data show safe error/unregistered states.

## Completion criteria
- `schema.json` accepts the generated manager JSON shape.
- Existing FAQ behavior remains intact.
- Safety rules remain intact.
- GitHub Pages deployment succeeds.
- iPhone Safari smoke test passes for both FAQ and manager flows.
- Test results and any remaining limitations are recorded in `TEST_REPORT.md`.

## Non-goals
- No dashboard.
- No AI chat for restaurant staff.
- No payment system.
- No analytics.
- No automatic invention or completion of store-specific rules.
