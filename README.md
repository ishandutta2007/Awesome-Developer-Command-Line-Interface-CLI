# Awesome-Developer-Command-Line-Interface-CLI

# Awesome-Developer-Command-Line-Interface-CLI

**Top Developer Command Line Interface CLI (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Cloud Provider CLIs, API Testing, Terminal Emulators, Autocomplete & Shell Productivity*

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Developer Command Line Interface (CLI)** tools. These tools enable developers to manage cloud infrastructure, test APIs, navigate terminals, and automate workflows from the command line—from official vendor CLIs like AWS CLI and GitHub CLI to open-source terminal emulators and productivity enhancers that give developers complete control over their shell environment.



**Examples** include Snowflake CLI, AWS CLI, Google Cloud SDK (gcloud), Azure CLI, GitHub CLI (gh), Databricks CLI, Stripe CLI, Vercel CLI, Supabase CLI, and Cloudflare Wrangler (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted CLI tooling, terminal emulators, and open developer productivity. **Critical note**: Most vendor CLIs are open source themselves—**GitHub CLI**, **Supabase CLI**, **Stripe CLI**, and **Vercel CLI** all publish their source. The open-source landscape for terminal productivity is exceptionally rich, with **ohmygosh** offering a Warp-inspired interactive shell, **rfig** providing local autocomplete, and **Zhell** delivering GPU-accelerated terminal features.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The Developer Command Line Interface (CLI) and developer tooling market is valued at approximately $1.42B to $5.6B (as part of the broader $30B+ software developer tooling ecosystem) and is projected to expand at a 9.8% to 15% CAGR through 2033. The sector is highly fragmented—characterized by vibrant open-source bottom-up adoption across diverse programming language ecosystems, while major cloud hyperscalers maintain high switching costs and platform-specific lock-in without a single winner-take-all monopoly across the terminal layer.

## SaaS/Hosted Platforms

| Platform / CLI | Company Size (Valuation / Revenue) | Pricing (Starting Paid Tier) | Free Tier Limits | Best For / Key Capabilities |
| :--- | :--- | :--- | :--- | :--- |
| **Azure CLI (`az`)** | Microsoft: ~$3.8T Market Cap / $100B+ Cloud Rev | Free CLI; Pay-as-you-go / Pay-per-resource (e.g., B1s VM from ~$0.0104/hr) | **Azure Free Account**: $200 trial credit (30 days) + 12 months free services (e.g., 750 hrs B1s VM, 5 GB Blob storage) + 55+ always-free services | Azure-centric infrastructure automation and ARM/Bicep template deployments |
| **AWS CLI** | Amazon: ~$2.1T Market Cap / $100B+ AWS Rev | Free CLI; Pay-as-you-go / Pay-per-resource (e.g., t4g.nano from ~$0.0042/hr) | **AWS Free Tier**: 12-month free trial (750 hrs/mo t2.micro/t3.micro, 5 GB S3 storage) + Always-free tier (1M Lambda requests/mo, 25 GB DynamoDB) | Enterprise cloud operations, scripting, and full-spectrum AWS services |
| **Google Cloud SDK (`gcloud`)** | Alphabet: ~$2.0T Market Cap / $40B+ GCP Rev | Free CLI; Pay-as-you-go / Pay-per-resource (e.g., e2-micro from ~$0.0084/hr) | **Google Cloud Free Tier**: $300 trial credit (90 days) + Always-free tier (1 non-preemptible e2-micro VM/mo in US regions, 5 GB Cloud Storage, 2M Cloud Function calls/mo) | GCP resource provisioning, BigQuery management, and Kubernetes engine orchestration |
| **Databricks CLI** | Databricks: $190B Valuation / $7B+ ARR | Free CLI; Serverless / Jobs compute starts at ~$0.10 to $0.15 per DBU (+ underlying cloud VM cost) | **Databricks Free Trial**: 14-day free trial with up to $400 in usage credits; or Community Edition (micro-cluster, personal non-commercial learning only) | Databricks Lakehouse, jobs scheduling, and Unity Catalog automation |
| **Stripe CLI** | Stripe: $159B Valuation / $6.8B+ Rev | Free CLI; Live processing starts at 2.9% + 30¢ per domestic transaction | **Stripe Test Mode**: 100% free indefinitely for simulation, local webhook listener forwarding, fixture generation, and API sandboxing (no monthly subscription or setup fees) | Local webhook testing and payments API development |
| **Cloudflare Wrangler** | Cloudflare: ~$110B Market Cap / $2.17B+ Rev | Free CLI; Workers Paid plan starts at $5.00/month (includes 10M requests + 30M CPU ms; $0.30/million extra requests) | **Workers Free Tier**: 100,000 requests per day (resets daily at UTC midnight), 10ms CPU time per invocation, up to 100 worker scripts | Edge compute deployment, serverless Workers, and KV/D1/R2 management |
| **Snowflake CLI (`snow`)** | Snowflake: ~$108B Market Cap / $4.68B+ Rev | Free CLI; Standard tier starts at $2.00 per capacity credit (AWS US East) + $23/TB/mo storage | **Snowflake Free Trial**: $400 in free usage credits valid for 30 days (whichever expires first; no upfront billing required) | Data warehouse management, Streamlit apps, Snowpark, and SQL automation |
| **GitHub CLI (`gh`)** | Microsoft / GitHub: $7.5B Acq. / Part of $3.8T MSFT | Free CLI; Team plan starts at $4.00/user/month | **GitHub Free Tier**: Unlimited public/private repositories, 2,000 GitHub Actions CI/CD minutes/mo (for private repos), 500 MB GitHub Packages storage | Terminal-native pull requests, issue tracking, and repository workflows |
| **Supabase CLI** | Supabase: $10.5B Valuation / ~$170M ARR | Free CLI; Pro plan starts at $25.00/month (includes 8 GB disk, 100 GB storage, 250 GB egress, $10 compute credits) | **Supabase Free Tier**: Up to 2 active projects (pauses after 1 week inactivity), 500 MB database, 1 GB storage, 50,000 MAUs, 500k edge functions/mo | Local-first Postgres development, migrations, schema typing, and emulated backend |
| **Vercel CLI** | Vercel: $9.3B Valuation / ~$200M+ ARR | Free CLI; Pro plan starts at $20.00/seat/month (includes $20 monthly usage credit, priority build queues) | **Vercel Hobby Tier**: Free for non-commercial use; 100 GB fast data transfer/mo, 1M edge requests/mo, 1M serverless function invocations/mo, 4 CPU-hours | Frontend deployment, preview URLs, domain configuration, and Next.js optimization |

## Open-Source GitHub Projects



- **ohmygosh**

  **Interactive shell in Go with Warp-inspired UI** (open source) — **the most innovative open-source terminal project**, reimagining the shell itself rather than the terminal emulator . **Features**: **Run multiple commands at once**; **connect to running commands** to enable stdin input; **cancel running commands via mouse click**; **copy output via mouse click**; **Vim motions in command prompt**; **Windows not supported** (PTY limitation). **Tech stack**: Go. **Deploy**: Homebrew (`brew tap tsukinoko-kun/tap && brew install tsukinoko-kun/tap/ohmygosh`), Go install, or Docker . **Trade-off**: **Work in progress and experimental**—explicitly "not ready for production use" . **Best for**: developers wanting to explore the future of interactive shells with modern UI features—not for production workflows yet.



- **rfig**

  **Command completion menus and history-based autosuggestions for zsh, Bash, and Fish** (open source) — **the most polished open-source autocomplete tool**, rebuilt from Fig's completion engine without account, AI, or telemetry . **Features**: **Completion menus** with up to 5 rows; **history-based autosuggestions** ranked by usage and directory context; **Vim-style navigation** (`↑`/`↓` for selection, `→` to accept); **local storage**—history and ranking stay on your machine; **Landlock/seccomp sandbox** on Linux for safe help probing; **no account required**. **Tech stack**: Rust (editing layer), ZLE integration for zsh. **Deploy**: macOS and Linux; Windows not supported . **Trade-off**: **Bash/Fish multiline paste returns to native editor**; newer than established tools; requires kernel 6.2+ on Linux for full features . **Best for**: developers wanting Fig-quality autocomplete without cloud dependency—especially privacy-conscious users on macOS or Linux.



- **Zhell**

  **GPU-accelerated terminal for Linux and Windows with command blocks and session persistence** (open source) — **the most feature-rich open-source terminal emulator** for developer workflows . **Features**: **Command blocks**—every command and output is a block with exit code, duration, copy, fold, rerun, share; **SQLite-backed history** with full-text search and secret redaction; **sessions survive** window close, kill, or update via `zhelld` daemon; **command palette**, **copy mode** (Vim keys), **quick select** (label URLs/paths/git hashes); **project mode** detecting Node/Rust/Go/Docker projects; **SSH integration** with shell integration installation on servers; **secret guard** for pasted secrets. **Tech stack**: Rust, SQLite. **Deploy**: Linux and Windows; no telemetry . **Trade-off**: **Newer than established terminals**; macOS not supported; GPU acceleration requires compatible hardware. **Best for**: developers wanting terminal history, session persistence, and command blocks—especially those frustrated by losing context when terminals close.



- **Zap (formerly OpenWarp)**

  **Local-first terminal with first-class AI and agent support** (open source, based on Warp) — **the most AI-forward open-source terminal**, forked from Warp with cloud requirements removed . **Features**: **No mandatory cloud**—no account, login, or Drive sync required; **BYOP AI providers**—any OpenAI-compatible endpoint plus native OpenAI/Anthropic/Gemini/DeepSeek/Ollama; **third-party CLI agents** wired into Blocks (DeepSeek-TUI, Codex CLI, Claude Code, Google Antigravity); **built-in SSH host manager** with tmux integration; **editable system prompts** via minijinja templates; **privacy defaults**—Cloud Agent and telemetry off by default. **Tech stack**: Rust (based on Warp). **Deploy**: Self-hosted desktop . **Trade-off**: **Evolving independently from Warp**—feature parity and stability still developing; forked project with governance questions. **Best for**: developers wanting Warp's UX without cloud dependency, with local AI and agent integration.



### Additional Strong Open-Source Options



- **fq** — Terminal tool for inspecting MP4, PCAP, images, and binary streams with jq-like queries (open source) . **Note**: Specialized binary inspector, not a general CLI. **Best for**: reverse engineers and security analysts.

- **himalaya** — CLI email client for IMAP, JMAP, Maildir, Gmail, and Microsoft (open source) . **Note**: Email management from terminal; not cloud CLI. **Best for**: terminal-centric users wanting email without GUI.

- **atuin** — Magical shell history in SQLite with optional encrypted sync (open source) . **Note**: History search, not a full shell. **Best for**: developers wanting `Ctrl+R` replacement with search and sync.

- **starship** — Minimal, blazing-fast prompt for any shell (open source) . **Note**: Prompt customization, not a CLI tool. **Best for**: developers wanting a fast, informative prompt.



**Frameworks for building custom systems**: Combine **rfig** for autocomplete with **Zhell** for terminal history and **ohmygosh** for experimental shell features—creating a modern terminal stack. **None of these match Warp's polish or vendor CLIs' service coverage**, but for terminal productivity, the open-source options are production-capable.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- CLI tools handling cloud credentials and API keys must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate secret management.

- **The "vendor CLI" vs. "terminal emulator" vs. "shell enhancement" vs. "autocomplete" distinction is critical.** **Snowflake CLI, AWS CLI, gcloud, Azure CLI, gh, Databricks CLI, Stripe CLI, Vercel CLI, Supabase CLI, and Wrangler** are **vendor CLIs**—they manage specific platforms . **Zhell and Zap** are **terminal emulators**—they run your existing shell with enhanced features . **ohmygosh** is a **shell**—it replaces bash/zsh entirely . **rfig** is **autocomplete**—it enhances existing shells . **Choose based on whether you need platform management, terminal UX, or shell behavior changes.**

- **Databricks CLI is in Public Preview** as of v0.205+—command surface and behavior may change . **Do not build critical automation without pinning versions.**

- **Wrangler v4 mutates flags per minor release**—`wrangler deploy` replaced `publish` mid-v3; v2 is obsolete . **Pin Wrangler to a known-good version in `package.json`.**

- **Stripe CLI live mode requires password store setup** (GPG + pass) for secure key management . **Test mode works without this.**

- **Supabase CLI local stack requires Docker Desktop**—`supabase db pull` starts a local Postgres container to diff schemas . **Plan for Docker dependency.**

- **ohmygosh is explicitly not production-ready**—it is experimental and Windows is unsupported . **For exploration only.**

- **rfig requires kernel 6.2+ on Linux** for Landlock-based help probing; older kernels or restricted containers refuse probing but menus still work . **Check `uname -r` before evaluating.**

- **Zhell is Linux/Windows only**—macOS is not supported . **macOS users should evaluate rfig or Zap instead.**

- Self-hosted open-source solutions require proper setup and ongoing maintenance. **CLI tools handle cloud credentials**—ensure your deployment meets your organization's security standards before connecting production accounts.



---



**Made for developers, platform engineers, and organizations building transparent CLI tooling solutions.**

Let's make Developer Command Line Interface tools more open, data-driven, and terminal-friendly.
