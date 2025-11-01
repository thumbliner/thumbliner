thumbliner.com
The website is a knowledge base focused on the project The Curious Outsider; pages and posts are the smallest unit of analysis, and the entire project is treated as a single work spanning epistemology, economics, entrepreneurship, investment practice, consulting, and education.

The site is a Jekyll-generated static site stored in a GitHub repository as Markdown files, themed with Just-the-Docs, and served over HTTPS via Cloudflare. The domain is hosted by Squarespace.

Squarespace Domains
Squarespace Domains are a registrar and management service for domain names, offering purchase, renewal, and DNS settings within the Squarespace dashboard.

Cloudflare
Cloudflare is an edge network and DNS provider that offers global CDN, free SSL/TLS, security, redirects, and static hosting via Cloudflare Pages.

Just-the-Docs
Just-the-Docs is a Jekyll documentation theme featuring sidebar navigation, built-in client-side search, and responsive, reading-first design. A modern, high customizable, responsive Jekyll theme for documentation with built-in search.

Obsidian (.md note-taking platform)
Obsidian is a local-first knowledge base that stores everything as plain Markdown (.md) files inside a folder called a vault. Notes link to each other with [[wikilinks]], show backlinks automatically, and render a graph view of connections. Core features include fast search, tags, embedded files, and robust version control compatibility (e.g., Git). Power users add community plugins for spaced repetition, citation management, kanban, and more—while keeping data portable because it’s all plain text.

Website as an extension of the .md network
The site functions as a public layer on top of the private Markdown vault: selected .md notes are organized, cleaned up, and published as web pages, preserving internal links, hierarchy, and ongoing research threads. This approach keeps a single source of truth in Markdown for personal note-taking and analysis, while the website exposes curated slices—reference pages, research hubs, and evolving essays—so the public output stays in sync with the underlying network of notes.

GitHub is an online platform for hosting code and collaborating on software using Git, pairing core planning, automation, and security tools with a shared workspace. Git provides the distributed version control that records changes to files and enables multiple people to work in parallel. Work lives in a repository—the project’s codebase and its full change history—where contributors create a branch to develop features independently, make a commit to capture a snapshot of their changes with an explanatory message, and coordinate with others. Teams group members with shared permissions and mentions to streamline collaboration, while documentation grows in a Wiki, a versioned knowledge base for longer-form notes and guides. When it’s time to share publicly, Pages serves a static website directly from the repository, ideal for docs, demos, or project homepages.

Jekyll, a static site generator, converts source files into a ready-to-host website by combining Markdown for writing, YAML front matter for metadata (title, layout, tags), and Liquid templates for layouts, includes, loops, and variables, yielding fast HTML/CSS/JS output. Built on Ruby, the system organizes content as posts, pages, and collections, draws structured data from _data files (YAML/JSON/CSV), and enforces consistent design through layouts and includes. Themes supply prepackaged styles with override options, while plugins add sitemaps, RSS feeds, tagging, and multilingual support. A Git-based version control workflow tracks content and configuration; the generated _site/ folder serves as deployable output; deployment on GitHub Pages publishes static files directly from a repository—delivering strong performance and security for blogs, documentation, portfolios, and other content-driven sites.

GitHub Pages is a static site hosting service that publishes web pages directly from a GitHub repository, turning Markdown or HTML into a fast, secure website. You choose a branch or folder as the source, push content, and GitHub builds and serves it over HTTPS at a project, user, or organization URL. Built-in support for Jekyll and community themes makes it easy to style blogs and documentation without complex tooling, while custom domains, automatic SSL, and integration with GitHub Actions enable modern workflows—from linting and testing to deploying on every commit. Common uses include documentation sites, portfolios, product pages, and demos that live alongside the code they describe.

Themes in GitHub Pages are ready-made design packages—usually Jekyll themes—that control your site’s layout, colors, typography, and common components so you can launch polished docs, blogs, or portfolios quickly. You pick a theme in repository settings or reference one with the remote_theme setting, then customize details with _config.yml, Sass variables, and overrides for layouts or includes. GitHub offers an official set in the pages-themes org, and thousands more come from the open-source community, covering styles from minimal docs to bold portfolio designs. Themes pair smoothly with Markdown content, work with automatic builds over HTTPS, and keep presentation separate from content, making sites easy to maintain and evolve.

Gem-based themes — Jekyll themes packaged as Ruby gems and listed in a site’s _config.yml via theme: <name>; they bundle layouts, includes, assets, and Sass so you can update the look by bumping a version without copying files into your repo.

GitHub Pages “Pages Themes” — the official, GitHub-maintained set of lightweight Jekyll themes (e.g., Minimal, Cayman) designed to be easy, stable, and compatible with the GitHub Pages build environment.

Documentation style themes — themes optimized for product or project docs: sidebar navigation, search, versioning cues, code blocks, callouts, and content-first typography (think “docs portal” look and IA).

Wiki style themes — themes that mimic a wiki’s feel: hierarchical or interlinked pages, simple typography, table-of-contents navigation, and lightweight page templates suited to knowledge bases.

Developer-notebook themes: code-centric layouts for demos and notes.
