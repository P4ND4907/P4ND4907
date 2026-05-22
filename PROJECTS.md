# P4ND4907 Program Catalog

This catalog organizes the current workspace and the three Perplexity research directions into named programs. It is meant to make GitHub easier to scan, maintain, and improve.

## Source Research Pulled In

- Perplexity link 1: automated blogs/SaaS/web pages for money-making experiments.
- Perplexity link 2: crypto day-trading analyst tooling and market-decision support.
- Perplexity link 3: audit dashboard for financial data architecture.
- Local extraction: Henry engine-sound diagnostics and AudioTuner gaming audio suite from `perplexity_task_extraction.md`.

## Money Automation Lab

| Clean Name | Current Repo/Folder | Purpose | Next Cleanup |
| --- | --- | --- | --- |
| Revenue Forge | [`revenue-forge`](https://github.com/P4ND4907/revenue-forge) | Private dashboard for organizing auto blog, SaaS, lead-generation, and money-project launch ideas from the Perplexity source. | Add brief/export generation and connect useful ideas to existing product repos. |
| InboxPilot AI | `inboxpilot-ai` | AI email operations SaaS for Gmail classification, bills, events, subscriptions, and cleanup review. | Keep as flagship SaaS; add demo screenshots and pricing notes. |
| FlipFlow Hub | `flipflow-hub` | Deal sourcing, flipping, lead generation, listing optimization, and payout tracking. | Add setup guide and money-flow examples. |
| Fiverr Sniper AI | `fiverr-sniper-ai` | Local freelance lead review, job selection, planning, delivery, and payout tracking. | Keep private-first; document extension import flow. |
| Fiverr Sniper Importer | `fiverr-sniper-ai-importer` | Browser extension for collecting freelance coding leads. | Link it clearly from Fiverr Sniper AI. |
| Storage Flip Assistant | `storage-flip-assistant` | Tracker for storage auction items, costs, listings, sales, and profit. | Add screenshots and sample CSV export. |
| YardNow | `yardnow` | Closed-beta route-service product with customers, workers, bookings, and proof photos. | Keep as real service product; avoid mixing with prototypes. |

## Trading Systems Lab

| Clean Name | Current Repo/Folder | Purpose | Next Cleanup |
| --- | --- | --- | --- |
| Crypto Daytrader Analyst | [`crypto-daytrader-analyst`](https://github.com/P4ND4907/crypto-daytrader-analyst) | Private, paper-only crypto market analyst dashboard for bias, setups, invalidation, risk rules, and scenarios. | Add trade journal and optional market-data adapters behind paper-only defaults. |
| Kalshi Scout | `kalshi-scout` | FastAPI + React paper-trading dashboard for Kalshi-style prediction markets. | Preserve safety defaults; add audit/risk dashboard docs. |
| Pandora Trading | `TRADING` | Electron + FastAPI desktop trading HUD with bot controls, market data, AI chat, and backtesting. | Rename in GitHub later to `pandora-trading` after branch cleanup. |
| Kalshi Scout Live | `Autobot-latest-main` | Live Kalshi assistant with signed API access and strict risk caps. | Merge the useful parts back into `kalshi-scout` or archive duplicate. |
| Autobot Experiments | `Autobot`, `Autobot-improved` | Older/duplicate Kalshi Scout variants. | Do not feature publicly; archive after confirming no unique code. |
| Trading Logic | `Trading-Logic` | Empty placeholder repo. | Either delete/archive or turn into shared strategy library. |

## Financial Data Architecture

| Clean Name | Current Repo/Folder | Purpose | Next Cleanup |
| --- | --- | --- | --- |
| Financial Audit Dashboard | [`financial-audit-dashboard`](https://github.com/P4ND4907/financial-audit-dashboard) | Starter audit dashboard from the Perplexity audit-dashboard research: trace data sources, transforms, model signals, controls, and review evidence. | Add importable flow definitions and weekly review export. |
| Feedback Automation System | `feedback-automation-system` | Turns raw feedback into prioritized tasks with AI clustering and approval gates. | Can supply the task-review workflow for financial audits. |
| Pandora Build Cache | `pandora-desktop` | Build-cache and task-graph system for multiple toolchains. | Keep as infrastructure; do not mix with trading logic. |

## Audio Intelligence Lab

| Clean Name | Current Repo/Folder | Purpose | Next Cleanup |
| --- | --- | --- | --- |
| AudioTuner Local | [`audiotuner-local`](https://github.com/P4ND4907/audiotuner-local) | Local reconstruction of the gaming audio suite: EQ studio, mic analysis simulator, hearing model, and Equalizer APO export. | Published; add screenshots and profile import/export next. |
| AutoEQ Helper | `autoeq` | Automatic Equalizer APO profile switching from headset/game JSON profiles. | Add examples for popular games/headsets. |
| Gaming Buddy | `gaming-buddy` | Windows helper for gaming audio and lightweight game-aware tuning. | Decide whether this becomes the desktop shell for AudioTuner. |
| Footstep Test | `footstep-test` | Small experiment around footsteps/audio tests. | Merge into AudioTuner or archive. |
| Henry Diagnostics | local research extraction | Web MVP concept for engine sound upload/recording with mocked diagnostic confidence scores. | Create repo only if you want this product line. |

## Game And Creative Tools

| Clean Name | Current Repo/Folder | Purpose | Next Cleanup |
| --- | --- | --- | --- |
| BotLab Tiles | `botlab-tiles-app` | Planner, learning-session, expansion unlock, and payment foundation. | Keep separate from general games. |
| Rift Runners | `rift-runners` | Game project. | Add README screenshots and controls. |
| Tower Defense | `tower-defense` | HTML5 tower defense game. | Keep as simple playable demo. |
| Pong Engine | `pong-engine` | Small engine/game experiment. | Decide whether to archive or combine with game utilities. |
| Quest Cache | `quest-cache` | Vite starter currently underdocumented. | Rename or document actual purpose. |

## Local Utility And Personal Tools

| Clean Name | Current Repo/Folder | Purpose | Next Cleanup |
| --- | --- | --- | --- |
| Vector Control Hub | `Vector` | Local-first dashboard for an Anki / DDL Vector robot through WirePod. | Keep as polished local tool. |
| Northbound Operator | `northbound-operator-site` | Alaska-focused opportunity studio site. | Use as public portfolio/company shell. |
| Pandora Site | `pandora-site` | Site for Pandora. | Link to `pandora-desktop`. |
| Closet Mate | `closet-mate` | Closet/fashion helper. | Add README or archive. |
| Fit Check | `FIT-CHECK` | Outfit/fit checker. | Consider lowercase rename to `fit-check`. |
| First Koinos Dapp | `first-dapp-panda` | Koinos token balance checker. | Keep as blockchain learning/demo repo. |
| Koinos Messenger Beta | `koinos-contract-messaging-dapp` | Thread-first public packet messaging beta. | Keep separate from first dapp. |
| Micro-Skills | `micro-skills-mobile` | Expo/React Native short learning app. | Add screenshots and app-store path. |

## Naming Rules Going Forward

- Use lowercase kebab-case for repository names.
- Keep one flagship repo per product; archive duplicates instead of letting names drift.
- Put research notes in `docs/research/`.
- Put launch and money tasks in `docs/business/`.
- Put status updates in `docs/updates/YYYY-MM-DD-project-update.md`.
- Keep destructive or real-money behavior disabled by default.

## Recommended GitHub Renames

These should be done after confirming branches and remotes:

| Current | Recommended | Reason |
| --- | --- | --- |
| `TRADING` | `pandora-trading` | Clearer, lowercase, product-specific. |
| `FIT-CHECK` | `fit-check` | Lowercase GitHub convention. |
| `Autobot-latest-main` | merge/archive | Duplicate Kalshi line. |
| `Autobot` | archive | Duplicate Kalshi line. |
| `Autobot-improved` | archive | Duplicate Kalshi line. |
| `Trading-Logic` | `trading-logic` or archive | Empty placeholder. |
