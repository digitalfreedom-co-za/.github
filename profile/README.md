# Digital Freedom — a Berger & Rosenstock GbR brand

**Digital Freedom is both the brand we build under and the goal we are working toward.**

Marcel Berger and Jasmin Rosenstock are building a life beyond the conventional nine-to-five — independent, deliberate, and on our own terms. Together we are pursuing exactly what the company name suggests: freedom over how we spend our time, where we live, what we work on, and how we measure success. This organization holds the code, infrastructure, and creative work that turn that intention into something real.

## The idea behind the name

For most of modern working life, the default contract is the same. A salary in exchange for a fixed schedule, a fixed location, and someone else's priorities. It is a reliable arrangement, and for many people it works. But it is not the only arrangement, and it is not the one we want.

Digital Freedom is the practical alternative we are building for ourselves:

- **Time freedom.** Working when we are most effective, taking breaks when our bodies and minds need them, and being present for the parts of life that matter.
- **Location freedom.** The work happens wherever a laptop and a stable internet connection can travel. The business runs today as a German GbR, operated from Bad Nauheim; a South African Pty Ltd is the planned next step. The whole stack is portable by design.
- **Creative freedom.** The right to choose the projects, the technology, the audience, and the standards we hold ourselves to — without compromise filtered through quarterly objectives we did not write.
- **Financial freedom.** Multiple independent income streams, owned outright, that compound over time rather than depend on a single employer.

These four are not slogans. They are the constraints we design every decision around — which projects we take on, which we politely decline, how we structure our days, and what we choose to ship.

## The two of us

### Marcel Berger — Indie app developer, software architect, author

Marcel is the technical half of Digital Freedom. Twenty years of software engineering in enterprise environments — microservice architectures for banks, identity and access management for regulated industries, instant payment platforms, digital transformation projects in critical infrastructure (KRITIS) — now applied to running an independent software business as a solo founder. Production-first, secure by default, designed to last.

The focus is end-to-end app development: native Swift apps for iOS and macOS, cross-platform Flutter apps for iOS (Android versions are planned per product, not yet shipped), the Quarkus-based Java microservices that power them, the Kubernetes platform that runs those services, the GitOps pipeline that deploys them, and the developer tooling that makes the whole stack pleasant to operate.

#### Products

Each product is a complete operation — mobile or desktop app, backend services where applicable, infrastructure, and operations — built and run by a single person. The canonical live catalogue at any moment is at <a href="https://marcelrgberger.com" target="_blank" rel="noopener noreferrer">marcelrgberger.com</a>.

**Live in the App Store**

- **<a href="https://dokuai.app" target="_blank" rel="noopener noreferrer">DokuAI</a>** (<a href="https://apps.apple.com/app/id6749177847" target="_blank" rel="noopener noreferrer">App Store</a>) — AI-powered reporting and documentation for construction and field service. Photos or voice recordings go in; structured, ready-to-send reports come out. Five microservices, Apache Kafka, OpenAI Whisper for transcription, OpenAI Vision for image understanding, PostgreSQL for state. Flutter app, iOS.
- **<a href="https://snapshots-quiz.app" target="_blank" rel="noopener noreferrer">SnapShots</a>** (<a href="https://apps.apple.com/app/id6759857715" target="_blank" rel="noopener noreferrer">App Store</a>) — AI-generated word puzzle game. Every hour the backend produces a fresh set of puzzles: GPT-4o picks the words, DALL-E 3 generates visual clues, everything translated into eight languages. Global leaderboard, streak system, offline play. Quarkus backend, PostgreSQL, Flutter app.
- **<a href="https://civo-cloud-manager.app.website" target="_blank" rel="noopener noreferrer">CivoCloudManager</a>** (<a href="https://apps.apple.com/app/id6760776010" target="_blank" rel="noopener noreferrer">App Store</a>) — Native macOS app for Civo Cloud: full CRUD, Kubernetes deep integration with live metrics, pods and logs, S3 file browser, firewall management, eight languages. Swift 6, SwiftUI, zero dependencies.

**In development**

- **<a href="https://sommelio.app" target="_blank" rel="noopener noreferrer">Sommelio</a>** — AI wine recommendations from a single photo. Three microservices, Kafka, OpenAI Vision, server-sent events. Flutter app, eight languages.
- **<a href="https://paperlessiq.app" target="_blank" rel="noopener noreferrer">PaperlessIQ</a>** — Intelligent document management for iOS. On-device OCR through Apple Vision, automatic metadata extraction, iCloud sync, optional AI classification. Native SwiftUI with SwiftData and CloudKit.
- **<a href="https://pourenzo.app" target="_blank" rel="noopener noreferrer">Pourenzo</a>** — AI bartender for the home bar. Three microservices, Kafka, OpenAI Vision. Flutter app with multi-language support.
- **BoatCare** — iOS native maintenance log for boat owners with on-device AI. Engine hours, antifoul cycle, electronics audit, winterisation. SwiftUI, SwiftData, Core ML.
- **<a href="https://github.com/digitalfreedom-co-za/bucketeer" target="_blank" rel="noopener noreferrer">Bucketeer</a>** — Native macOS app for browsing, transferring, mounting and syncing object storage across AWS, Civo, Cloudflare R2, Backblaze B2, Wasabi, DigitalOcean Spaces, Storj, MinIO and Azure Blob. Source-available on GitHub, App Store only on release. Swift 6.

#### The platform behind it

All products run on a single Civo-hosted Kubernetes cluster with GitOps via ArgoCD, Helm-based deployments, container images in GitHub Container Registry, Maven artefacts in GitHub Packages, observability through Prometheus and Grafana. CI/CD pipelines carry every change from `git push` to App Store release entirely through GitHub Actions — no manual deploys, no hidden state.

The cluster maintains itself. A Claude-powered platform operations agent runs every hour, reads the cluster state, detects problems, restarts unhealthy services, scales node pools, applies resource patches to Helm charts, and commits the changes back through the GitOps pipeline. A second agent runs daily and does the slower work — analysing patterns, tuning Helm charts, refining security policies. No human in the loop for routine operations.

#### Studio for client work — <a href="https://theapparchitect.com" target="_blank" rel="noopener noreferrer">theapparchitect.com</a>

Alongside the in-house products, Marcel offers project-shaped engagements to small and mid-sized businesses through **The App Architect** — the studio brand operated under the same GbR.

- **Full Build.** From whiteboard to App Store. Planning, architecture, UX and delivery. Source code, build pipelines and a written handover at the end. Fixed scope, fixed price.
- **Architecture Review.** Two focused weeks looking at the system you already have. Written report with prioritised actions and risk ratings — practical findings, not academic.
- **Embedded Architect.** Part-time inside your team. Owns the system-design calls and keeps your engineers unblocked. Months, not days.

The studio's positioning: *Code is cheap. Architecture is the moat.* One architect, end-to-end, accountable for the outcome — no agency layers between the work and the customer. The same engineering discipline that runs the in-house products is applied to the client's stack.

#### Books

- **<a href="https://amzn.eu/d/06PCcWKD" target="_blank" rel="noopener noreferrer">Solopreneur — The Art of Working Alone</a>** — What it actually takes to build, ship, and operate software products without a team. Decision-making under uncertainty, systems thinking, and the structural realities of working independently. Written from inside the journey rather than after it.

#### Open source

The product repositories in this organization are private by design — they are the commercial backbone. Most of Marcel's open-source work, smaller experiments, and tooling live on the personal account at <a href="https://github.com/marcelrgberger" target="_blank" rel="noopener noreferrer">github.com/marcelrgberger</a>:

- **Claude Code plugins** that let Anthropic's Claude Code agent drive desktop applications directly — `pages-cli` for Apple Pages, `numbers-cli` for Apple Numbers, `xcode-cli` for the full Xcode toolchain, `whatsapp-cli` for WhatsApp on macOS, `inwx-dns` for INWX DNS management, `jira-cli` for Atlassian Jira Cloud.
- **Native macOS apps** — `auto-brew` keeps Homebrew and every installed package up to date in the background with a full Brew GUI and an AppSnapshot engine for migrating app data across Macs; `civo-cloud-manager` is the SwiftUI front end for the Civo cloud and the Kubernetes cluster running underneath, shipped on the App Store as well.
- **CLI tools** — `askapro-cli` is an AI-powered document analysis tool with 85+ expert consultation roles; `l10n_translator_cli` automates ARB translation through OpenAI for Flutter localisation; `alertmanager-talk-bridge` forwards Prometheus alerts to Nextcloud Talk.
- **Larger projects** — `paperless-neo` is an AI-native fork of Paperless-ngx with a modern UI and multi-user RBAC.
- **A Homebrew tap** at `marcelrgberger/homebrew-tap` distributes the macOS apps.

Within this organization itself, **<a href="https://github.com/digitalfreedom-co-za/bucketeer" target="_blank" rel="noopener noreferrer">Bucketeer</a>** is source-available — the native macOS app for cross-provider object storage. Source readable, App Store only on release.

Stars and pull requests on these projects are the strongest signal we have for which experiments are worth more of our time. If a tool helps you, please consider starring it.

#### Core technologies

- **Languages and mobile:** Java, Dart and Flutter, Swift and SwiftUI, Go, Python, TypeScript
- **Backend frameworks:** Quarkus (primary), Spring Boot, REST, GraphQL, Apache Kafka, server-sent events
- **Cloud and infrastructure:** Kubernetes, Docker, Helm, ArgoCD, GitHub Actions, Civo Cloud, Azure, OpenShift
- **Data and messaging:** PostgreSQL, MongoDB, SQLite, Liquibase, CloudKit, S3-compatible object storage
- **Observability:** Prometheus, Grafana, Loki, Alertmanager
- **Security and identity:** Keycloak, OAuth2, OpenID Connect, JSON Web Tokens, Let's Encrypt, Authentik
- **AI and automation:** OpenAI API (GPT-4o, Vision, DALL-E 3, Whisper), Anthropic Claude, on-device Vision and Speech frameworks

### Jasmin Rosenstock — Beauty content as **Jasmin Elise · Beauty**

Jasmin is the creative half of Digital Freedom. Her brand positioning is *Glowy skin. Heatless curls. Me-time.* — hair styling, skincare routines, and small beauty hacks for women who consciously take time for themselves and want to bring out their best. Over forty, based in Bad Nauheim, and proof that the right routines beat the right age.

The website <a href="https://jasminelise-beauty.de" target="_blank" rel="noopener noreferrer">jasminelise-beauty.de</a> is the central hub. It pulls the latest videos and shorts directly from the YouTube channel and organises everything around three rabbit holes a viewer can keep returning to:

- **Hair styling.** Dyson Airwrap deep-dives across every attachment in the ecosystem, ghd Waver and flat-iron beach waves, round-brush blowouts, heatless curlers, thermal-brush waves — long tutorials and quick fixes that actually hold.
- **Skincare routines.** Weekend resets, morning and night routines, the small habits that compound into a real glow over time. No twenty-step routines, no products you'll never use again.
- **Beauty hacks.** Tool reviews, time-savers, the little tricks that get you out of the door looking like you tried. Including practical hair recovery (gym hair in ten minutes, the morning-after refresh, humidity-proof anti-frizz strategies).

The channel is in German, the audience reaches well beyond German-speaking countries, and the work happens on Jasmin's own schedule — which is the entire point. The site, the channel and the editorial line are all owned end-to-end: no agency, no studio, no external producer.

Find her on YouTube at <a href="https://www.youtube.com/@jasminelise_beauty" target="_blank" rel="noopener noreferrer">@jasminelise_beauty</a> and on her site at <a href="https://jasminelise-beauty.de" target="_blank" rel="noopener noreferrer">jasminelise-beauty.de</a>.

## What lives in this organization

This GitHub organization is the production home for everything we run commercially. Without going through the full catalogue, the broad categories are:

- **Mobile and desktop applications.** The Flutter apps for DokuAI, Sommelio, Pourenzo, SnapShots, plus a handful of smaller native and cross-platform apps we use ourselves or ship to dedicated audiences.
- **Backend services.** A few dozen Quarkus-based Java microservices providing image recognition, audio transcription, report generation, recommendation engines, persistence layers, and feedback collection.
- **Platform infrastructure.** The Civo-hosted Kubernetes cluster definition, ArgoCD application manifests, Helm charts, monitoring stack, autoscaler, secrets management, and the platform operations agents that keep it healthy.
- **CI/CD foundations.** Reusable GitHub Actions workflows, composite actions, the internal container registry, the internal Maven registry, and the templates that scaffold new repositories with all of this wired up from the first commit.
- **Templates and tooling.** Cookiecutter-style scaffolding for new Flutter apps, new Quarkus services, and new Java libraries — the patterns extracted from the existing products and made available for the next one.
- **Internal documentation.** Runbooks, architectural notes, conventions, and the wiki we treat as the single source of truth for how things are done here.

Most of this is private by design. Some of the patterns and lessons flow back into Marcel's open-source work on his personal account.

## Follow along

If the idea of building an independent working life resonates with you — whether you are interested in the technical side, the creative side, or simply curious how the story develops — there are a few ways to follow along:

- **Marcel's GitHub** at <a href="https://github.com/marcelrgberger" target="_blank" rel="noopener noreferrer">github.com/marcelrgberger</a> — star the open-source projects you find useful, read the code, open issues, send pull requests. Stars on small projects are not vanity metrics for us; they tell us which experiments deserve more of our time.
- **Jasmin's site and channel** at <a href="https://jasminelise-beauty.de" target="_blank" rel="noopener noreferrer">jasminelise-beauty.de</a> and <a href="https://www.youtube.com/@jasminelise_beauty" target="_blank" rel="noopener noreferrer">youtube.com/@jasminelise_beauty</a> — subscribe, hit the bell, leave comments, share videos with people who would enjoy them. Every subscriber is one more vote for independent beauty content built without an agency behind it.

Both channels are how we earn the room to keep building. If our work helps you in any way, the most useful thing you can do is help us reach the next person who would benefit from it.

## Where to find the company

- **Brand:** <a href="https://digitalfreedom.co.za" target="_blank" rel="noopener noreferrer">digitalfreedom.co.za</a>
- **Legal entity:** Berger & Rosenstock GbR, Bad Nauheim, Germany
- **Marcel — personal site:** <a href="https://marcelrgberger.com" target="_blank" rel="noopener noreferrer">marcelrgberger.com</a>
- **Marcel — studio for client work:** <a href="https://theapparchitect.com" target="_blank" rel="noopener noreferrer">theapparchitect.com</a>
- **Marcel — code, plugins, open source:** <a href="https://github.com/marcelrgberger" target="_blank" rel="noopener noreferrer">github.com/marcelrgberger</a>
- **Marcel — book:** <a href="https://amzn.eu/d/06PCcWKD" target="_blank" rel="noopener noreferrer">Solopreneur — The Art of Working Alone</a>
- **Jasmin — beauty site:** <a href="https://jasminelise-beauty.de" target="_blank" rel="noopener noreferrer">jasminelise-beauty.de</a>
- **Jasmin — YouTube:** <a href="https://www.youtube.com/@jasminelise_beauty" target="_blank" rel="noopener noreferrer">youtube.com/@jasminelise_beauty</a>

Thank you for stopping by. Building this kind of independence takes time, and the most encouraging thing in the world is finding out other people are interested in the journey.
