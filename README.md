# AI agents directory

Which AI agents and crawlers visit websites, who runs them, what they do, the name each one obeys in robots.txt, and what its operator publishes so you can tell the real agent from an impostor. Every entry links to the operator's own documentation and says when it was last checked.

Maintained by [Knocklog](https://knocklog.ai/agents), the analytics for AI agents. Data in [`agents.json`](agents.json) and [`agents.csv`](agents.csv) (schema in [`schema.json`](schema.json)). Last checked: 2026-11-04. 26 agents.

> Em português: [diretório de agentes de IA](https://knocklog.ai/agentes) e o guia [como saber quais agentes de IA visitam o meu site](https://knocklog.ai/guia/como-saber-quais-agentes-de-ia-visitam-meu-site).

## The agents

### Training crawler

| Agent | Operator | robots.txt token | Obeys robots.txt | Docs |
|---|---|---|---|---|
| [GPTBot](https://knocklog.ai/agents/openai-gptbot) | OpenAI | `GPTBot` | yes | [official](https://developers.openai.com/api/docs/bots) |
| [ClaudeBot](https://knocklog.ai/agents/anthropic-claudebot) | Anthropic | `ClaudeBot` | yes | [official](https://support.claude.com/en/articles/8896518-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler) |
| [Google-Extended](https://knocklog.ai/agents/google-extended) | Google | `Google-Extended` | yes | — |
| [Applebot-Extended](https://knocklog.ai/agents/apple-applebot-extended) | Apple | `Applebot-Extended` | yes | [official](https://support.apple.com/en-us/119829) |
| [Meta-ExternalAgent](https://knocklog.ai/agents/meta-externalagent) | Meta | `meta-externalagent` | yes | [official](https://developers.facebook.com/docs/sharing/webmasters/web-crawlers) |
| [CCBot](https://knocklog.ai/agents/commoncrawl-ccbot) | Common Crawl | `CCBot` | unknown | — |
| [Bytespider](https://knocklog.ai/agents/bytedance-bytespider) | ByteDance | `Bytespider` | unknown | — |

### AI search crawler

| Agent | Operator | robots.txt token | Obeys robots.txt | Docs |
|---|---|---|---|---|
| [OAI-SearchBot](https://knocklog.ai/agents/openai-oai-searchbot) | OpenAI | `OAI-SearchBot` | yes | [official](https://developers.openai.com/api/docs/bots) |
| [Claude-SearchBot](https://knocklog.ai/agents/anthropic-claude-searchbot) | Anthropic | `Claude-SearchBot` | yes | [official](https://support.claude.com/en/articles/8896518-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler) |
| [PerplexityBot](https://knocklog.ai/agents/perplexity-perplexitybot) | Perplexity | `PerplexityBot` | yes | [official](https://docs.perplexity.ai/docs/resources/perplexity-crawlers) |
| [Meta-WebIndexer](https://knocklog.ai/agents/meta-webindexer) | Meta | `meta-webindexer` | yes | [official](https://developers.facebook.com/docs/sharing/webmasters/web-crawlers) |
| [Amazonbot](https://knocklog.ai/agents/amazon-amazonbot) | Amazon | `Amazonbot` | unknown | — |
| [PetalBot](https://knocklog.ai/agents/huawei-petalbot) | Huawei | `PetalBot` | unknown | — |

### Assistant fetching for a person

| Agent | Operator | robots.txt token | Obeys robots.txt | Docs |
|---|---|---|---|---|
| [ChatGPT-User](https://knocklog.ai/agents/openai-chatgpt-user) | OpenAI | `ChatGPT-User` | partial | [official](https://developers.openai.com/api/docs/bots) |
| [Claude-User](https://knocklog.ai/agents/anthropic-claude-user) | Anthropic | `Claude-User` | yes | [official](https://support.claude.com/en/articles/8896518-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler) |
| [Perplexity-User](https://knocklog.ai/agents/perplexity-user) | Perplexity | `Perplexity-User` | no | [official](https://docs.perplexity.ai/docs/resources/perplexity-crawlers) |
| [Meta-ExternalFetcher](https://knocklog.ai/agents/meta-externalfetcher) | Meta | `meta-externalfetcher` | no | [official](https://developers.facebook.com/docs/sharing/webmasters/web-crawlers) |
| [DuckAssistBot](https://knocklog.ai/agents/duckduckgo-duckassistbot) | DuckDuckGo | `DuckAssistBot` | unknown | — |
| [MistralAI-User](https://knocklog.ai/agents/mistral-user) | Mistral AI | `MistralAI-User` | unknown | — |

### Agentic browser

| Agent | Operator | robots.txt token | Obeys robots.txt | Docs |
|---|---|---|---|---|
| [ChatGPT agent](https://knocklog.ai/agents/openai-chatgpt-agent) | OpenAI | `—` | unknown | [official](https://help.openai.com/en/articles/11845367-chatgpt-agent-allowlisting) |
| [Google-Agent](https://knocklog.ai/agents/google-agent) | Google | `—` | unknown | [official](https://developers.google.com/crawling/docs/crawlers-fetchers/google-agent) |

### Search engine

| Agent | Operator | robots.txt token | Obeys robots.txt | Docs |
|---|---|---|---|---|
| [Googlebot](https://knocklog.ai/agents/google-googlebot) | Google | `Googlebot` | yes | [official](https://developers.google.com/crawling/ipranges/) |
| [Applebot](https://knocklog.ai/agents/apple-applebot) | Apple | `Applebot` | yes | [official](https://support.apple.com/en-us/119829) |
| [Bingbot](https://knocklog.ai/agents/microsoft-bingbot) | Microsoft | `bingbot` | yes | — |

### Link preview

| Agent | Operator | robots.txt token | Obeys robots.txt | Docs |
|---|---|---|---|---|
| [FacebookExternalHit](https://knocklog.ai/agents/meta-facebookexternalhit) | Meta | `facebookexternalhit` | partial | [official](https://developers.facebook.com/docs/sharing/webmasters/web-crawlers) |

### Ads checker

| Agent | Operator | robots.txt token | Obeys robots.txt | Docs |
|---|---|---|---|---|
| [OAI-AdsBot](https://knocklog.ai/agents/openai-oai-adsbot) | OpenAI | `OAI-AdsBot` | unknown | [official](https://developers.openai.com/api/docs/bots) |

## Using the data

- **robots.txt:** use `robotsTokens`, not the product name. Blocking `GPTBot` keeps OpenAI's training crawler out but not `ChatGPT-User`, which fetches pages when a person asks ChatGPT something.
- **Logs and analytics:** match `userAgentTokens` against the User-Agent header to label requests.
- **Impostors:** anyone can send a User-Agent that says GPTBot. The `published` field lists what the operator publishes (IP range files, reverse-DNS names, Web Bot Auth signature agents) to confirm a request really came from it. An agent with nothing published cannot be confirmed either way.

To see which of these agents visit your own site, whether they are real, and how many visitors and leads AI assistants send you, create a free project at [knocklog.ai](https://knocklog.ai). You can also check any site's readiness for AI agents at [knocklog.ai](https://knocklog.ai) or from Claude and ChatGPT with the Knocklog connector.

## Contributing

Open an issue or a pull request. A new agent or a change needs a link to the operator's official documentation; entries without one are not added.

## License

Data: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Credit "Knocklog AI agents directory" with a link to https://knocklog.ai/agents.
