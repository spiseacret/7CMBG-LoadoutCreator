# 7CMBG Loadout Creator agent instructions

## Pathway tracking and naming

Pathway is the standard work tracker for 7CMBG work across repositories, agents, and chats, regardless of checkout location. This applies to requested development, specifications, investigations, and maintenance; a read-only lookup alone does not require a new card.

- Before substantive work, inspect the appropriate board and reuse a matching card or create one. Record the problem, agreed scope, acceptance criteria, relevant issues, validation, and blockers. Avoid duplicates.
- Use Pathway's actual generated card code as the work identifier. Never invent, predict, or renumber a card code or assume every board uses CF.
- PR and issue titles include `[<CARD-CODE>]` before the summary. Preserve required repository prefixes first: `[DOCS] [CF-48] Standardize Pathway workflow` for the Discord bot; `docs: [CF-48] Standardize Pathway workflow` for a semver-prefixed repository; otherwise `[CF-47] Simplify profile hover preview`.
- New branches use the board's generated branch name when compatible with repository rules; otherwise use `<type>/<lowercase-card-code>-<short-slug>`, for example `fix/cf-47-profile-hover-preview`. Include the code in commit subjects after any required conventional prefix. Preserve existing issue/PR numbers. Do not rename an already-open PR's branch merely to retrofit naming.
- Link the card from every related PR and issue body; link those PRs/issues back from the card. If GitHub integration is not configured on the board, use explicit clickable links and report the limitation rather than claiming native integration.
- Cross-repository work may share a clearly identified coordination card, with every participating repo/PR linked. Independent tasks use separate cards on the appropriate board. Do not create redundant GitHub issues solely to mirror cards.
- Frontend board: https://pathway.lazycub.studio/b/7cmbg-frontend
- HQ board: https://pathway.lazycub.studio/b/7cmbg-hq
- Discord bot board: https://pathway.lazycub.studio/b/7cmbg-discord-bot (generated prefix CB). Bot-only work uses this board; cross-repository CF-48 remains this rollout's coordination card.
- Discover other board mappings from live project context; do not invent a board or silently place unrelated bot work on the frontend board.
- Follow established board status conventions. Otherwise use To do before work; In Progress for implementation/draft review; Testing for validation; Done after acceptance; Released only after verified deployment. Record merge/deploy state separately.
- Include card code/URL, related PR/issue links, validation, and next action in handoffs and checkpoints so another chat can resume. If Pathway is unavailable, report the tracking gap and continue independent authorized work without fabricating a card or code.
- Tracking and naming do not expand task scope or authorize merging, deployment, production changes, unrelated messages, or access to restricted repositories. Preserve repository branch targets and approval boundaries.

