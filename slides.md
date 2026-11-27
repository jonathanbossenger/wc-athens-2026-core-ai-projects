# WordCamp Athens 2026 Talk Slides

https://athens.wordcamp.org/2026/

## WordPress 🤝 AI: A Tour of the Core AI Projects

A tour of the WordPress Core AI team's building blocks: the Abilities API, the MCP Adapter, the AI Client, and the AI Experiments plugin.

### Slides

1. Title
   - WordPress 🤝 AI: A tour of the Core AI projects
   - Jonathan Bossenger · Developer Advocate, Automattic
2. Intro: Hi, I'm Jonathan
   - Developer Advocate at Automattic
   - Based in Cape Town, South Africa
   - AI experimenter
   - https://jonathanbossenger.com/
   - (image: slide-02-intro.jpg)
3. The WordPress Core AI team
   - Formed in May 2025
   - Accelerates and coordinates AI projects across the WordPress ecosystem
   - Core team reps from across the WordPress ecosystem
   - https://make.wordpress.org/ai/
4. Open building blocks
   - Make WordPress AI-ready without forcing a single vendor or model into Core
   - 01 Abilities API: describe what WordPress can do
   - 02 MCP Adapter: expose content and actions to external agents
   - 03 AI Client: call AI providers in a standard way
   - 04 AI Experiments: try AI features in WordPress today
   - https://make.wordpress.org/ai/2025/07/17/ai-building-blocks/
5. Shipping since 6.9, more to 7.3
   - Updates have shipped since WordPress 6.9, and more is on the roadmap toward WordPress 7.3
   - https://make.wordpress.org/ai/2026/10/28/wordpress-for-the-agentic-web/

#### Section 1: Abilities API

6. Section divider: 01 / 04 Abilities API, the foundation for AI
7. Developers and robots like structure
   - Every AI feature needs a solid foundation to build on
   - (image: slide-05-foundation-for-ai.jpg)
8. 20+ years of WordPress APIs
   - (image: slide-06-wordpress-apis-diagram.png)
9. Register once, use everywhere
   - One registry for extenders, AI and automations
   - 20 years of open source, now with structured inputs and outputs
   - Accessible via PHP, JavaScript and the REST API
   - Part of WordPress Core since WordPress 6.9
10. Next: native Abilities
    - A baseline set of Abilities for common site management workflows
    - A few foundational Abilities may land in WordPress 7.2
    - A useful native set is targeted for WordPress 7.3
11. One registry, many consumers
    - (image: slide-08-abilities-api-diagram.png)
12. Learn the Abilities API
    - https://github.com/WordPress/abilities-api
    - https://make.wordpress.org/core/2025/11/10/abilities-api-in-wordpress-6-9/
    - https://developer.wordpress.org/news/2025/11/introducing-the-wordpress-abilities-api/

#### Section 2: MCP Adapter

13. Section divider: 02 / 04 MCP Adapter, Abilities become tools and resources
14. Abilities → tools & resources
    - Giving AI agents context since 2025
    - (image: slide-10-abilities-tools-resources.jpg)
15. The WordPress MCP Adapter
    - Automatically adapts Abilities into MCP tools
    - Works with any AI agent application: chat, IDE and more
    - HTTP (web) and STDIO (local) transports
    - Not in Core (yet): install it as a Composer package or the MCP Adapter plugin
16. On the road to Core
    - 7.2: rapid iteration on reliability, security and usability
    - 7.3: a proposal to bring MCP into Core (direct merge, or bundled so it can evolve independently)
17. One adapter, any agent
    - (image: slide-12-mcp-adapter-diagram.png)
18. Learn the MCP Adapter
    - https://modelcontextprotocol.io/
    - https://github.com/WordPress/mcp-adapter
    - https://wordpress.org/plugins/mcp-adapter/
    - https://developer.wordpress.org/news/2026/02/from-abilities-to-ai-agents-introducing-the-wordpress-mcp-adapter/
19. WordPress for the agentic web
    - The goal: connecting an agent to your site should take one sign-in
    - Flow: an agent recognises your site → it sends you an authorization link → you sign in → done
    - https://make.wordpress.org/ai/2026/10/28/wordpress-for-the-agentic-web/
20. Four workstreams
    - MCP Adapter: agents talk to WordPress over MCP
    - Abilities: what agents can do on your site
    - OAuth: authorize agents without sharing Application Passwords
    - End-to-end UX: discover, request access, perform tasks, manage or revoke
    - Foundations in 7.2, targeting 7.3
    - Get involved in #core-ai on Make WordPress Slack

#### Section 3: AI Client

21. Section divider: 03 / 04 AI Client, making WordPress AI aware
22. Making WordPress AI aware
    - One standard way for Core and plugins to talk to any AI provider
    - (image: slide-14-making-wordpress-ai-aware.jpg)
23. The WordPress AI Client
    - Registers AI providers for use inside WordPress
    - Fully extendable to work with any external AI provider
    - Anthropic, OpenAI and Google Gemini by default, plus community providers
    - Foundations shipped in WordPress 7.0, with the new Connectors page
24. LLM agnostic
    - (image: slide-16-ai-client-diagram.png)
25. Learn the AI Client
    - https://make.wordpress.org/core/2026/03/24/introducing-the-ai-client-in-wordpress-7-0/
    - https://github.com/WordPress/php-ai-client
    - https://developer.wordpress.org/news/2026/05/how-to-build-an-image-generation-plugin-with-the-wordpress-ai-client/

#### Section 4: AI Experiments

26. Section divider: 04 / 04 AI Experiments, AI features you can try today
27. The AI Experiments plugin
    - AI-powered features in your admin and editor. Nothing is on by default
    - Stats: 1 stable feature, 26 experiments
    - https://wordpress.org/plugins/ai/
    - (image: slide-18-ai-experiments.jpg)
28. What's inside
    - Stable: image generation and editing. Everything else is an experiment you switch on
    - Editor writing tools
    - Editorial notes & updates
    - Content & media
    - Comments
    - Agentic web
    - Site owner controls
29. Live demo: Let's try it together
30. Try it yourself
    - Install the plugin and connect your AI provider
    - https://wordpress.org/plugins/ai/

#### Wrap-up and bonus

31. Recap: the Core AI building blocks
    - 01 Abilities API: https://github.com/WordPress/abilities-api
    - 02 MCP Adapter: https://github.com/WordPress/mcp-adapter
    - 03 AI Client: https://github.com/WordPress/php-ai-client
    - 04 AI Experiments: https://wordpress.org/plugins/ai/
32. Want more?
    - wp-bench: benchmark models for WordPress development (https://github.com/WordPress/wp-bench)
    - agent-skills: expert WordPress knowledge for AI coding assistants (https://github.com/WordPress/agent-skills)
    - (image: slide-21-want-more.jpg)
33. A recent wp-bench run
    - Latest three models from OpenAI, Anthropic and Google · 350 tests each
    - 1 Claude Opus 5.5 (Anthropic) 90.6%
    - 2 Gemini 4 Argon (Google) 90.0%
    - 3 GPT-6.1 Sol (OpenAI) 88.0%
    - 4 GPT-6 Astra (OpenAI) 87.7%
    - 5 Gemini 3.8 Flash (Google) 85.1%
    - 6 Gemini 3.7 Flash (Google) 84.9%
    - 6 Claude Sonnet 5.5 (Anthropic) 84.9%
    - 8 Claude Haiku 5.5 (Anthropic) 82.3%
    - 9 GPT-6 Luna (OpenAI) 77.7%
    - https://wp-ai-benchmarks.space.fast/
34. agent-skills
    - Expert-level WordPress knowledge for AI coding assistants
    - `npx skills add WordPress/agent-skills --list`
    - `npx skills add WordPress/agent-skills --skill wp-abilities-api`
    - Skills: wp-abilities-api, wp-block-development, wp-block-themes, wp-plugin-development, wp-rest-api, wp-interactivity-api, wp-performance, wp-phpstan, wp-playground, wp-wpcli-and-ops, + more
    - https://github.com/WordPress/agent-skills
35. Any questions?
36. Thank you.
    - jonathanbossenger@gmail.com
    - https://jonathanbossenger.com/
