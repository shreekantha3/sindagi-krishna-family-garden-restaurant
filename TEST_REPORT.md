# TEST REPORT — Krishna Family Garden Restaurant
> Date: 2026-09-10 | Tester: Senior Engg | Segment: Food

## Build
- [x] `npm run build` PASS (vite 5.4.21, 4 modules, 0 warnings)
- dist sizes: 12.16 kB HTML / 12.06 kB CSS / 1.20 kB JS — well under perf budget (<200KB JS, <1.5MB total)

## Static checks (all PASS)
- [x] tel:+919980111618 present (hero + mobile Call Now + contact)
- [x] Google Maps URL present (Directions + reviews + contact)
- [x] JSON-LD Restaurant schema present
- [x] H1 contains business name, semantic sections, skip link
- [x] No lorem ipsum, no invented hours/prices (call-CTA fallback)
- [x] Images have alt / placeholders labeled, lazy-ready
- [x] aria-expanded on nav toggle, keyboard reachable CTAs

## Pending (requires preview + device lab before Deployed)
- [ ] Lighthouse CI mobile+desktop (target 90/95/95/95)
- [ ] Playwright 12-case E2E + axe (0 serious) + linkinator
- [ ] Screenshots 360/768/1440 attached to PR
- [ ] GitHub Pages deploy verify (200 + base path assets)

## Verdict: BUILT + STATIC QA PASS → ready for full QA + separate repo deploy

## Maps embed + README (2026-09-15)
- [x] Google Maps iframe embed added to #visit panel (lazy-loaded, `output=embed`, query fused from page's own Maps URL)
- [x] Per-site README.md added (live link, owner update guide)
