# Skills Index — Spindrift Marketing System

Last updated: 2026-01-30

## Installed Skills

### Custom Slash Commands (Built for Spindrift)

| Skill | Division | Trigger | Chains With |
|-------|----------|---------|-------------|
| `/wip` | Operations | Session start | All — reads /projects/active/ |
| `/brief [topic]` | Content | New content needed | content-strategy → `/brief` → copywriting → `/critique` |
| `/analytics [period]` | Analytics | Weekly + ad hoc | `/analytics` → `/diagnose` → `/weekly-review` |
| `/competitor [name]` | Strategy | New competitor activity | `/competitor` → competitor-alternatives → `/diagnose` |
| `/weekly-review` | Strategy + Ops | Weekly (Friday/Monday) | `/analytics` + all projects → diagnosis → next week plan |
| `/critique [file]` | Creative | Draft content ready | copywriting → `/critique` → copy-editing → publish |
| `/diagnose [challenge]` | Strategy | Strategic challenge arises | `/competitor` + `/analytics` → `/diagnose` → action plan |
| `/repurpose [file] [format]` | Content | Hero content published | `/brief` → create → `/repurpose` → distribute |

### Installed from marketingskills Library

| Skill | Division | Trigger | Chains With | Installed |
|-------|----------|---------|-------------|-----------|
| content-strategy | Content | Quarterly planning, new pillar needed | → `/brief` → copywriting → `/critique` | 2026-01-30 |
| copywriting | Creative | Any external copy needed | content-strategy → copywriting → `/critique` → copy-editing | 2026-01-30 |
| copy-editing | Creative | Draft ready for polish | copywriting → `/critique` → copy-editing → publish | 2026-01-30 |
| competitor-alternatives | Strategy + Content | SEO competitive pages needed | `/competitor` → competitor-alternatives → page-cro | 2026-01-30 |
| social-content | Content | Social calendar production | content-strategy → `/brief` → social-content → `/repurpose` | 2026-01-30 |
| email-sequence | Growth + Content | New email flow needed | copywriting → email-sequence → `/critique` | 2026-01-30 |
| marketing-psychology | Strategy | Campaign planning, CRO work | marketing-psychology → copywriting, paid-ads, page-cro | 2026-01-30 |
| paid-ads | Growth | Campaign creation/optimization | marketing-psychology → paid-ads → `/analytics` | 2026-01-30 |
| launch-strategy | Strategy + Growth | New flavor or product launch | launch-strategy → email-sequence + social-content + paid-ads | 2026-01-30 |
| marketing-ideas | Strategy | Brainstorming, planning | marketing-ideas → `/diagnose` → action plan | 2026-01-30 |
| pricing-strategy | Strategy | Pricing review, competitive response | `/competitor` → pricing-strategy → `/diagnose` | 2026-01-30 |
| page-cro | Growth | Website conversion optimization | marketing-psychology → page-cro → ab-test-setup | 2026-01-30 |
| ab-test-setup | Analytics | Experiment design | page-cro / paid-ads → ab-test-setup → `/analytics` | 2026-01-30 |
| referral-program | Growth | Referral program design/optimization | email-sequence → referral-program → `/analytics` | 2026-01-30 |

---

## Deferred Skills

| Skill | Reason | Trigger Condition | Source |
|-------|--------|-------------------|--------|
| programmatic-seo | Needs SEO infrastructure and content at scale | When Spindrift has 50+ indexed pages and SEO is a priority channel | marketingskills |
| schema-markup | Needs technical implementation on website | When website redesign or SEO audit identifies schema gaps | marketingskills |
| seo-audit | Needs website crawl access and analytics | When organic traffic optimization becomes a priority | marketingskills |
| analytics-tracking | Needs platform access for implementation | When tracking gaps are identified in analytics workflows | marketingskills |
| signup-flow-cro | DTC subscription flow — secondary priority | When DTC subscription conversion becomes a top-3 priority | marketingskills |
| onboarding-cro | DTC post-purchase experience | When subscription churn exceeds 15% monthly | marketingskills |
| free-tool-strategy | SaaS-oriented, limited CPG application | When Spindrift launches a digital product or interactive tool | marketingskills |
| form-cro | Limited web form usage for CPG brand | When lead capture forms become a significant conversion path | marketingskills |

---

## Skipped Skills

| Skill | Reason |
|-------|--------|
| popup-cro | Not aligned with premium brand experience — popups conflict with Spindrift's warm, non-intrusive voice |
| paywall-upgrade-cro | SaaS-specific — no paywall in CPG business model |
| product-marketing-context | Already created manually as `.claude/product-marketing-context.md` — no need for the guided setup skill |

---

## Skill Chains (Key Workflows)

### Content Production Pipeline
```
content-strategy → /brief [topic] → copywriting → /critique [draft] → copy-editing → /repurpose [final] [format]
```

### Campaign Launch Pipeline
```
launch-strategy → email-sequence + social-content + paid-ads → /analytics [post-launch]
```

### Competitive Intelligence Loop
```
/competitor [name] → competitor-alternatives → /diagnose [strategic response] → content-strategy update
```

### Conversion Optimization Cycle
```
marketing-psychology → page-cro → ab-test-setup → /analytics → iterate
```

### Strategic Review Loop
```
/analytics [weekly] → /weekly-review → /diagnose [crux challenge] → coherent actions → execute
```

---

## Maintenance Notes

- **Weekly:** Check marketingskills repo for updates to installed skills. Merge improvements, preserve brand customizations.
- **Monthly:** Review deferred skills — has any trigger condition been met?
- **Quarterly:** Full audit — prune unused installed skills (30+ days no use), promote deferred skills where appropriate.
