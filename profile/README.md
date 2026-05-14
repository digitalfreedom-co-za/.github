# Digital Freedom (Pty) Ltd

**Digital Freedom is both the name of the company and the goal we are working toward.**

Marcel Berger and Jasmin Rosenstock are building a life beyond the conventional nine-to-five — independent, deliberate, and on our own terms. Together we are pursuing exactly what the company name suggests: freedom over how we spend our time, where we live, what we work on, and how we measure success. This organization holds the code, infrastructure, and creative work that turn that intention into something real.

## The idea behind the name

For most of modern working life, the default contract is the same. A salary in exchange for a fixed schedule, a fixed location, and someone else's priorities. It is a reliable arrangement, and for many people it works. But it is not the only arrangement, and it is not the one we want.

Digital Freedom is the practical alternative we are building for ourselves:

- **Time freedom.** Working when we are most effective, taking breaks when our bodies and minds need them, and being present for the parts of life that matter.
- **Location freedom.** The work happens wherever a laptop and a stable internet connection can travel. Our company is registered in South Africa, the work is currently done from Germany, and the next move is open. The whole stack is portable by design.
- **Creative freedom.** The right to choose the projects, the technology, the audience, and the standards we hold ourselves to — without compromise filtered through quarterly objectives we did not write.
- **Financial freedom.** Multiple independent income streams, owned outright, that compound over time rather than depend on a single employer.

These four are not slogans. They are the constraints we design every decision around — which projects we take on, which we politely decline, how we structure our days, and what we choose to ship.

## The two of us

### Marcel Berger — Indie app developer, software architect, author

Marcel is the technical half of Digital Freedom. Twenty years of software engineering in enterprise environments — microservice architectures for banks, identity and access management for regulated industries, instant payment platforms, digital transformation projects in critical infrastructure (KRITIS) — now applied to running an independent software business as a solo founder. Production-first, secure by default, designed to last.

The focus is end-to-end app development: native Swift apps for iOS and macOS, cross-platform Flutter apps for iOS and Android, the Quarkus-based Java microservices that power them, the Kubernetes platform that runs those services, the GitOps pipeline that deploys them, and the developer tooling that makes the whole stack pleasant to operate.

#### Products currently shipping

Five production products live in this organization. Each one is a complete operation — mobile app, backend services, infrastructure, and operations — built and run by a single person.

- **[DokuAI](https://dokuai.app)** — AI-powered reporting and documentation for construction and field service. Photos or voice recordings go in; structured, ready-to-send reports come out. Five microservices, Apache Kafka, OpenAI Whisper for transcription, OpenAI Vision for image understanding, PostgreSQL for state. Flutter app for iOS and Android.
- **[Sommelio](https://sommelio.app)** — AI wine recommendations from a single photo. Point the camera at a bottle or label; Sommelio extracts the wine profile, matches it against the user's taste, and streams personalised suggestions in real time. Three microservices, Kafka, OpenAI Vision, server-sent events. Flutter app, eight languages.
- **[PaperlessIQ](https://paperlessiq.app)** — Intelligent document management for iOS. On-device OCR through Apple Vision, automatic metadata extraction, iCloud sync, optional AI classification. Native SwiftUI with SwiftData and CloudKit. Offline-first — nothing leaves the device unless the user wants it to.
- **[Pourenzo](https://pourenzo.app)** — AI bartender for the home bar. Photograph the available bottles; Pourenzo identifies what is there and generates cocktail recipes that can actually be made with that inventory. Three microservices, Kafka, OpenAI Vision. Flutter app with multi-language support.
- **[SnapShots](https://snapshots-quiz.app)** — AI-generated word puzzle game. Every hour the backend produces a fresh set of puzzles: GPT-4o picks the words, DALL-E 3 generates visual clues, everything translated into eight languages. Global leaderboard, streak system, offline play. Quarkus backend, PostgreSQL, Flutter app.

#### The platform behind it

All five products run on a single Civo-hosted Kubernetes cluster with GitOps via ArgoCD, Helm-based deployments, container images in GitHub Container Registry, Maven artefacts in GitHub Packages, observability through Prometheus and Grafana. CI/CD pipelines carry every change from `git push` to App Store release entirely through GitHub Actions — no manual deploys, no hidden state.

The cluster maintains itself. A Claude-powered platform operations agent runs every hour, reads the cluster state, detects problems, restarts unhealthy services, scales node pools, applies resource patches to Helm charts, and commits the changes back through the GitOps pipeline. A second agent runs daily and does the slower work — analysing patterns, tuning Helm charts, refining security policies. No human in the loop for routine operations.

#### Books

- **[Solopreneur — The Art of Working Alone](https://amzn.eu/d/06PCcWKD)** — What it actually takes to build, ship, and operate software products without a team. Decision-making under uncertainty, systems thinking, and the structural realities of working independently. Written from inside the journey rather than after it.

#### Open source

The repositories in this organization are private by design — they are the commercial backbone. Most of Marcel's open-source work, smaller experiments, and tooling live on the personal account at [github.com/marcelrgberger](https://github.com/marcelrgberger):

- **Claude Code plugins** that let Anthropic's Claude Code agent drive desktop applications directly: `pages-cli` for Apple Pages, `numbers-cli` for Apple Numbers, `xcode-cli` for the full Xcode toolchain, `whatsapp-cli` for WhatsApp on macOS, `inwx-dns` for DNS management.
- **Native macOS apps** — `auto-brew` keeps Homebrew and every installed package up to date in the background; `civo-cloud-manager` is a SwiftUI front end for the Civo cloud and the Kubernetes cluster running underneath; `dictator-app` brings system-wide offline dictation via WhisperKit on Apple Silicon.
- **CLI tools** — `askapro-cli` is an AI-powered document analysis tool with 85+ expert consultation roles; `l10n_translator_cli` automates ARB translation through OpenAI for Flutter localisation; `alertmanager-talk-bridge` forwards Prometheus alerts to Nextcloud Talk.
- **Larger projects** — `paperless-neo` is an AI-native fork of Paperless-ngx with a modern UI and multi-user RBAC.
- **A Homebrew tap** at `marcelrgberger/homebrew-tap` distributes the macOS apps.

Stars and pull requests on these projects are the strongest signal we have for which experiments are worth more of our time. If a tool helps you, please consider starring it.

#### Core technologies

- **Languages and mobile:** Java, Dart and Flutter, Swift and SwiftUI, Go, Python, TypeScript
- **Backend frameworks:** Quarkus (primary), Spring Boot, REST, GraphQL, Apache Kafka, server-sent events
- **Cloud and infrastructure:** Kubernetes, Docker, Helm, ArgoCD, GitHub Actions, Civo Cloud, Azure, OpenShift
- **Data and messaging:** PostgreSQL, MongoDB, SQLite, Liquibase, CloudKit, S3-compatible object storage
- **Observability:** Prometheus, Grafana, Loki, Alertmanager
- **Security and identity:** Keycloak, OAuth2, OpenID Connect, JSON Web Tokens, Let's Encrypt, Authentik
- **AI and automation:** OpenAI API (GPT-4o, Vision, DALL-E 3, Whisper), Anthropic Claude, on-device Vision and Speech frameworks

### Jasmin Rosenstock — Beauty content

Jasmin is the creative half of Digital Freedom. She produces beauty content on YouTube — the makeup, the skincare, the products, the routines, the experiments. Her channel is her own brand, her own platform, and one of the cornerstones of how Digital Freedom works in practice: an independent business built one upload at a time, owned end-to-end, with no agency, no studio, and no editorial line other than her own.

What you will find on the channel:

- **Makeup tutorials and looks** — full faces, specific techniques, going from product on the table to finished look on camera.
- **Product reviews and first impressions** — honest takes on new launches and long-term opinions on the products that survived the rotation.
- **Routines** — the daily, weekly, and seasonal beauty routines that actually get used, not the idealised ones meant for thumbnails.
- **Lifestyle and behind the scenes** — the parts of an independent creator's life that do not fit into a tutorial: the planning, the studio setup, the gear, the moments between the videos.

The channel is in German, the audience reaches well beyond German-speaking countries, and the work happens on Jasmin's own schedule — which is the entire point.

Find her on YouTube at [@jasminelise_beauty](https://www.youtube.com/@jasminelise_beauty).

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

- **Marcel's GitHub** at [github.com/marcelrgberger](https://github.com/marcelrgberger) — star the open-source projects you find useful, read the code, open issues, send pull requests. Stars on small projects are not vanity metrics for us; they tell us which experiments deserve more of our time.
- **Jasmin's YouTube channel** at [youtube.com/@jasminelise_beauty](https://www.youtube.com/@jasminelise_beauty) — subscribe, hit the bell, leave comments, share videos with people who would enjoy them. Every subscriber is one more vote for independent beauty content built without an agency behind it.

Both channels are how we earn the room to keep building. If our work helps you in any way, the most useful thing you can do is help us reach the next person who would benefit from it.

## Where to find the company

- **Website:** [digitalfreedom.co.za](https://digitalfreedom.co.za)
- **Registration:** Digital Freedom (Pty) Ltd, South Africa
- **Marcel — personal website:** [marcelrgberger.com](https://marcelrgberger.com)
- **Marcel — code, plugins, and open source:** [github.com/marcelrgberger](https://github.com/marcelrgberger)
- **Marcel — book:** [Solopreneur — The Art of Working Alone](https://amzn.eu/d/06PCcWKD)
- **Jasmin — beauty content:** [youtube.com/@jasminelise_beauty](https://www.youtube.com/@jasminelise_beauty)

Thank you for stopping by. Building this kind of independence takes time, and the most encouraging thing in the world is finding out other people are interested in the journey.
