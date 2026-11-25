# unity-ai-integration

AI tools built around a Unity 6 space tower-defense / twin-stick shooter (indie game in development, source private):

- **LLM Balance Analyst** — an agent that reads playtest telemetry, finds balance problems and proposes tuning changes, with evals that verify every number it reports.
- **Ship AI companion** — an in-game AI that streams advice to the player from live game state, using tool calling through a secure backend proxy.
- **Agentic development workflow** — how the game itself is developed with an AI coding agent: context files, tested PRs, CI and human review.

> 🚧 Work in progress — started November 2026.

## Repository layout

| Folder | What | Stack |
|---|---|---|
| [`balance-analyst/`](balance-analyst/) | Telemetry → balance report + tuning proposals, with evals | Node.js, TypeScript, Claude API (tool use) |
| [`ship-ai-backend/`](ship-ai-backend/) | Proxy between the game and the LLM: keys, streaming, rate & cost limits | Node.js, TypeScript, Express |
| [`unity-client/`](unity-client/) | Reusable Unity package: AI client, streaming UI, game state → context | Unity 6, C# |
| [`docs/`](docs/) | Agentic workflow write-up, examples, architecture | Markdown |

## Author

**Adrian Muntean** — Senior Unity / C# developer (12+ years: games, mobile, VR / Meta Quest, Node.js backends).

## License

MIT — see [LICENSE](LICENSE).
