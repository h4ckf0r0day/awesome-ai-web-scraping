<div align="center">

# Awesome AI Web Scraping

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of tools, libraries, and resources for AI-powered web scraping.

</div>

---

Frameworks, hosted APIs, browser infrastructure, MCP servers, and research for turning the web into clean, structured data for LLMs, RAG pipelines, and agents.

**Scope:** Tools where AI or LLMs play a meaningful role in extraction, navigation, or content understanding. General-purpose scrapers (Scrapy, BeautifulSoup) belong in [awesome-web-scraping](https://github.com/lorien/awesome-web-scraping). Autonomous browser agents belong in [awesome-web-agents](https://github.com/steel-dev/awesome-web-agents).

## Contents

- [Frameworks & Libraries](#frameworks--libraries)
- [Hosted APIs](#hosted-apis)
- [Browser Infrastructure for AI](#browser-infrastructure-for-ai)
- [No-Code AI Scrapers](#no-code-ai-scrapers)
- [MCP Servers for Scraping](#mcp-servers-for-scraping)
- [Web Search APIs for LLMs](#web-search-apis-for-llms)
- [Proxy & Anti-Bot Infrastructure](#proxy--anti-bot-infrastructure)
- [Datasets](#datasets)
- [Benchmarks & Research](#benchmarks--research)
- [Tutorials & Guides](#tutorials--guides)
- [Contributing](#contributing)

## Frameworks & Libraries

Self-hosted, open-source. Most pair a headless browser with an LLM for schema-based or prompt-based extraction.

- [Crawl4AI](https://github.com/unclecode/crawl4ai) - LLM-friendly web crawler with Markdown output and JSON-schema or LLM-based extraction. Python. ![GitHub Repo stars](https://img.shields.io/github/stars/unclecode/crawl4ai?style=social)
- [Scrapling](https://github.com/D4Vinci/Scrapling) - Adaptive Python framework with smart element tracking that relocates elements after site changes. Cloudflare Turnstile bypass, spider framework with pause/resume, and a built-in MCP server. ![GitHub Repo stars](https://img.shields.io/github/stars/D4Vinci/Scrapling?style=social)
- [ScrapeGraphAI](https://github.com/ScrapeGraphAI/Scrapegraph-ai) - Python scraper using LLM + graph pipelines. Describe data in natural language, get typed JSON. Works with OpenAI, Anthropic, Groq, Gemini, Ollama. ![GitHub Repo stars](https://img.shields.io/github/stars/ScrapeGraphAI/Scrapegraph-ai?style=social)
- [llm-scraper](https://github.com/mishushakov/llm-scraper) - TypeScript library for structured extraction with Zod schemas. Supports GPT, Claude, Gemini, Llama, Qwen. ![GitHub Repo stars](https://img.shields.io/github/stars/mishushakov/llm-scraper?style=social)
- [Reader](https://github.com/jina-ai/reader) - Jina AI's URL-to-Markdown converter. Engine behind `r.jina.ai`. ![GitHub Repo stars](https://img.shields.io/github/stars/jina-ai/reader?style=social)
- [Stagehand](https://github.com/browserbase/stagehand) - Browser automation framework with `act`, `extract`, and `observe` primitives over Playwright. ![GitHub Repo stars](https://img.shields.io/github/stars/browserbase/stagehand?style=social)
- [Browser-Use](https://github.com/browser-use/browser-use) - Agent framework commonly used for scraping complex, login-walled sites. ![GitHub Repo stars](https://img.shields.io/github/stars/browser-use/browser-use?style=social)
- [Skyvern](https://github.com/Skyvern-AI/skyvern) - Browser automation for forms, logins, and dynamic content. ![GitHub Repo stars](https://img.shields.io/github/stars/Skyvern-AI/skyvern?style=social)
- [LaVague](https://github.com/lavague-ai/LaVague) - Natural language web automation framework. ![GitHub Repo stars](https://img.shields.io/github/stars/lavague-ai/LaVague?style=social)
- [CyberScraper 2077](https://github.com/itsOwen/CyberScraper-2077) - LLM scraper with Streamlit UI. Supports OpenAI, Gemini, and Ollama. Tor support included. ![GitHub Repo stars](https://img.shields.io/github/stars/itsOwen/CyberScraper-2077?style=social)
- [ScraperAI](https://github.com/scraperai/scraperai) - AI scraper with auto-detection of page types, pagination, and catalog cards. ![GitHub Repo stars](https://img.shields.io/github/stars/scraperai/scraperai?style=social)
- [SpiderCreator](https://github.com/carlosplanchon/spidercreator) - Generates Playwright spiders from natural language prompts. ![GitHub Repo stars](https://img.shields.io/github/stars/carlosplanchon/spidercreator?style=social)
- [PulsarRPA](https://github.com/platonai/pulsarRPA) - AI-powered browser automation and data extraction. ![GitHub Repo stars](https://img.shields.io/github/stars/platonai/pulsarRPA?style=social)

## Hosted APIs

Managed services that turn URLs into LLM-ready Markdown or JSON. JS rendering, proxies, and anti-bot handled internally.

- [Firecrawl](https://firecrawl.dev/) - Scrape, crawl, map, search, agent, and interact endpoints. LLM-ready Markdown. 500 free credits, paid plans from $16/mo.
- [Jina Reader](https://jina.ai/reader/) - Prepend `r.jina.ai/` to any URL for LLM-friendly text. Free tier with no API key required.
- [Diffbot](https://www.diffbot.com/) - Computer vision and NLP extraction with a knowledge graph layer. Paid.
- [Apify](https://apify.com/) - Marketplace of 10,000+ pre-built scrapers ("Actors") plus a runtime for your own. Free tier and paid plans.
- [Bright Data](https://brightdata.com/) - Scraping with 150M+ proxies and pre-built APIs for 120+ sites. Free tier and paid plans.
- [Zyte](https://www.zyte.com/) - Scraping API with AI extraction. Formerly Scrapinghub. Paid.
- [ScrapingBee](https://www.scrapingbee.com/) - JS rendering, AI extraction, Markdown, and Google SERP support. Free trial and paid plans.
- [ZenRows](https://www.zenrows.com/) - Anti-bot focused scraping API with Markdown output. Free trial and paid plans.
- [Oxylabs](https://oxylabs.io/) - Proxies plus a Web Scraper API with adaptive parsing. Paid.
- [Spider](https://spider.cloud/) - Concurrent crawler and scraper API with LLM-ready output. Free tier and paid plans.
- [WebScraping.AI](https://webscraping.ai/) - Scraping API with question-answering and field-extraction endpoints. Free tier and paid plans.
- [Scrapeless](https://www.scrapeless.com/) - Scraping API with anti-bot bypass and structured extraction. Free tier and paid plans.
- [Kadoa](https://www.kadoa.com/) - Self-healing extraction that adapts when sites change. Paid.
- [Expand.ai](https://www.expand.ai/) - Turns any website into a type-safe API. Paid.
- [Reworkd](https://reworkd.ai/) - Agentic AI for no-code structured extraction. Paid.

## Browser Infrastructure for AI

Headless browsers designed for AI agents and scrapers.

- [Steel.dev](https://steel.dev/) - Open-source headless browser API for AI agents. Self-host or use the hosted service. ![GitHub Repo stars](https://img.shields.io/github/stars/steel-dev/steel-browser?style=social)
- [Browserbase](https://www.browserbase.com/) - Hosted headless browser. Powers Stagehand. Paid.
- [Hyperbrowser](https://www.hyperbrowser.ai/) - Browser platform with stealth, scraping, and agent endpoints. Free tier and paid plans.
- [Anchor Browser](https://anchorbrowser.io/) - Browser API with built-in auth and session persistence. Paid.
- [Browserless](https://www.browserless.io/) - Headless Chrome as a service. Free tier and paid plans.
- [Obscura](https://github.com/h4ckf0r0day/obscura) - Rust-based headless browser. CDP-compatible with Puppeteer and Playwright. Built-in stealth and tracker blocking. ![GitHub Repo stars](https://img.shields.io/github/stars/h4ckf0r0day/obscura?style=social)
- [Browserable](https://github.com/browserable/browserable) - Open-source, self-hostable browser automation library. ![GitHub Repo stars](https://img.shields.io/github/stars/browserable/browserable?style=social)
- [Fortress](https://github.com/tiliondev/fortress) - Open-source recompiled Chromium, fingerprint corrected in C++, driven over CDP. Passes CreepJS and sannysoft, clears Cloudflare Turnstile and Anubis.

## No-Code AI Scrapers

Visual or point-and-click tools that use AI to extract data without writing code.

- [Browse AI](https://www.browse.ai/) - Chrome extension and SaaS for AI-assisted scraping with scheduled monitoring.
- [Bardeen.ai](https://bardeen.ai/) - Chrome extension combining AI scraping with automation across 100+ apps.
- [Thunderbit](https://thunderbit.com/) - Two-click Chrome extension with AI "Suggest Fields" for instant extraction.
- [Gumloop](https://www.gumloop.com/) - Visual workflow builder for scraping, LLM calls, and data transforms.
- [Octoparse](https://www.octoparse.com/) - Visual scraper with AI-assisted field detection.
- [ParseHub](https://www.parsehub.com/) - Visual scraper with template-based extraction.

## MCP Servers for Scraping

[Model Context Protocol](https://modelcontextprotocol.io/) servers that expose scraping capabilities to Claude, Cursor, Windsurf, and other LLM clients.

- [Firecrawl MCP](https://github.com/mendableai/firecrawl-mcp-server) - Official MCP wrapper for Firecrawl's scrape, crawl, and extract endpoints. ![GitHub Repo stars](https://img.shields.io/github/stars/mendableai/firecrawl-mcp-server?style=social)
- [Bright Data MCP](https://github.com/brightdata/brightdata-mcp) - Search, scrape, and extract from 60+ sources with anti-bot bypass. 5,000 free requests/month. ![GitHub Repo stars](https://img.shields.io/github/stars/brightdata/brightdata-mcp?style=social)
- [Scrapling MCP](https://scrapling.readthedocs.io/en/latest/ai/mcp-server/) - Built-in MCP server bundled with [Scrapling](https://github.com/D4Vinci/Scrapling). Install with `pip install "scrapling[ai]"`.
- [Fetch](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch) - Anthropic's official fetch MCP server. URL-to-Markdown.
- [Browserbase MCP](https://github.com/browserbase/mcp-server-browserbase) - MCP server exposing Browserbase sessions and Stagehand primitives. ![GitHub Repo stars](https://img.shields.io/github/stars/browserbase/mcp-server-browserbase?style=social)
- [Puppeteer MCP](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/puppeteer) - Browser automation for scraping and interaction.
- [Apify MCP](https://github.com/apify/actors-mcp-server) - Run any Apify Actor as an MCP tool. ![GitHub Repo stars](https://img.shields.io/github/stars/apify/actors-mcp-server?style=social)
- [WebScraping.AI MCP](https://webscraping.ai/docs/mcp) - MCP integration for WebScraping.AI's extraction tools.
- [Tilion](https://github.com/tiliondev/fortress) - MCP server exposing a stealth Chromium so agents reach sites behind Cloudflare, DataDome, and Anubis; fetch, extract, crawl, detect WAF.

## Web Search APIs for LLMs

Search APIs that return structured, LLM-friendly results with full-page content.

- [Exa](https://exa.ai/) - Neural search API. Returns clean content alongside results.
- [Tavily](https://tavily.com/) - Search API optimized for LLMs and RAG.
- [Linkup](https://www.linkup.so/) - Search API with verified sources.
- [Perplexity Sonar](https://docs.perplexity.ai/) - Perplexity's online search and answer API.
- [Serper](https://serper.dev/) - Fast, low-cost Google search API.
- [SerpAPI](https://serpapi.com/) - Search engine results API.
- [Brave Search API](https://brave.com/search/api/) - Independent search index.
- [You.com API](https://api.you.com/) - Web, news, and snippet endpoints.
- [Kagi Search API](https://help.kagi.com/kagi/api/search.html) - Premium, ad-free search results.

## Proxy & Anti-Bot Infrastructure

- [Bright Data](https://brightdata.com/) - 150M+ proxies, Web Unblocker, browser cloud.
- [Oxylabs](https://oxylabs.io/) - Residential, datacenter, and ISP proxies plus Web Unblocker.
- [Decodo (Smartproxy)](https://decodo.com/) - Residential proxies and scraping APIs.
- [NetNut](https://netnut.io/) - ISP and residential proxy network.
- [ZenRows](https://www.zenrows.com/) - Anti-bot proxy and scraping API.
- [ScraperAPI](https://www.scraperapi.com/) - Proxy rotation and CAPTCHA handling.

## Datasets

Pre-scraped web data for RAG, training, or benchmarking.

- [Common Crawl](https://commoncrawl.org/) - The largest public web crawl. Petabytes of pages, monthly updates.
- [FineWeb](https://huggingface.co/datasets/HuggingFaceFW/fineweb) - 15T-token deduplicated web dataset from Hugging Face.
- [RedPajama-Data-v2](https://github.com/togethercomputer/RedPajama-Data) - 30T-token open web dataset.
- [C4](https://huggingface.co/datasets/allenai/c4) - Colossal Clean Crawled Corpus derived from Common Crawl.
- [The Pile](https://pile.eleuther.ai/) - 825 GiB diverse text corpus including web data.

## Benchmarks & Research

- [SWDE](https://www.microsoft.com/en-us/research/publication/from-one-tree-to-a-forest-a-unified-solution-for-structured-web-data-extraction/) - Structured Web Data Extraction benchmark from Microsoft Research.
- [WebSRC](https://x-lance.github.io/WebSRC/) - Dataset for web-based structural reading comprehension.
- [AXE](https://arxiv.org/abs/2406.06237) - Research on DOM pruning for token-efficient LLM extraction.
- [NEXT-EVAL](https://arxiv.org/abs/2503.05036) - Benchmark comparing HTML representations for LLM extraction accuracy.

## Tutorials & Guides

- [Firecrawl Docs](https://docs.firecrawl.dev/) - Guides for RAG ingestion, structured extraction, and agent integration.
- [Crawl4AI Documentation](https://docs.crawl4ai.com/) - Walk-throughs for LLM-based extraction strategies.
- [Jina Reader Quickstart](https://jina.ai/reader/) - One-line URL conversion.
- [LangChain Web Loaders](https://python.langchain.com/docs/integrations/document_loaders/) - Document loaders for web content.
- [LlamaIndex Web Connectors](https://llamahub.ai/) - Web data connectors for LlamaIndex.

## Contributing

Contributions welcome. Open a pull request to add a new tool or resource.

Guidelines:
- Keep entries focused on AI/LLM-powered scraping. Generic scrapers belong elsewhere.
- Follow the format: `- [Name](url) - One-line description.`
- Add the GitHub stars badge for open-source projects.
- Mention pricing in the description if relevant (free tier, paid, etc.).

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related rights to this work.
