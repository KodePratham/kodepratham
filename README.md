# Pratham Kode Manifest

> *Building tools and experiences that scale so others can build at scale too.*

This repository reflects my current operating system—technical opinions, product instincts, and the automation that keeps the `main` branch deployable every day. Think of it as the control room for the Kode Pratham playbook.

## Product Vision

- **Mission:** Empower every collaborator to ship thoughtfully engineered software by keeping the infrastructure predictable, the processes transparent, and the feedback loops fast.
- **Approach:** Data-informed iteration, ruthless prioritization, and a culture that values learning from experiments as much as shipping features.
- **Signals:** Healthy pipelines, clear observability, and metrics that tell whether a change actually improved the user experience.

## Core Principles

1. **Instrument everything.** Runbooks, dashboards, and CI feedback should give you answers before you ask questions.
2. **Build with ownership.** Small teams push past friction by owning every part of the stack—if it breaks in production, fix it, document it, improve it.
3. **Ship and iterate.** A well-tested prototype is just the beginning; every release is a learning opportunity.
4. **Communicate clearly.** Share context, assumptions, and metrics with every PR, issue, and sync so alignment stays tight.

## Getting Started

This repository assumes a modern JavaScript/TypeScript workflow but the core ideas translate to any stack.

### Setup

1. Clone the repo with your preferred Git credentials:

    ```bash
    git clone https://github.com/kodepratham/<project>.git
    cd <project>
    ```

2. Install dependencies:

    ```bash
    npm install
    ```

3. Copy environment defaults if provided and set any required secrets:

    ```bash
    cp .env.example .env
    ```

### Develop

- Run the primary development workflow via `npm run dev` or the framework’s equivalent.
- Lint and format with `npm run lint` and `npm run format` before pushing; consistent formatting removes noise from reviews.
- Run `npm test` to keep coverage honest and catch regressions before merge.

## Release Readiness

- Every PR must include a short summary, test plan, and impact assessment (regressions? migrations?).
- Automation scripts (lint, tests, builds) need to pass locally before pushing; the CI should simply confirm what you already know is green.
- Production deploys happen through the documented pipeline—no shortcuts, no unilateral pushes to `main`.

## Communication & Collaboration

- Use issues to capture assumptions, decisions, and open questions.
- Tag maintainers for feedback early; resolving disagreements with data prevents wasted cycles.
- Document any new observable artifacts (dashboards, alerts, schema changes) alongside the code that introduces them.

## Contact

- GitHub: [https://github.com/kodepratham](https://github.com/kodepratham)
- Twitter: [https://twitter.com/kodepratham](https://twitter.com/kodepratham)

Questions or escalations go through the normal channels (issues > PR > sync). Keep a bias toward written records so the entire product history remains accessible.

## License

MIT. Refer to `LICENSE` for details or add one if it is missing.