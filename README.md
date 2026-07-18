# Nick Dingwall

> Operations manager doing data and automation work inside the world's largest finance and accounting operation. Moving into data analytics full-time. This page is receipts, not adjectives.

---

## Day Job

**Automation and support.** Point person for automation on my team and branch. When a process is broken, I'm the one who rebuilds it in Power Automate, Power BI, a PWA, or a bot.

**Legacy modernization.** Converting a portfolio of decades-old Microsoft Access programs into governed Power BI semantic models. Data model first, then DAX, then the dashboard.

**Operations background.** Managed a 50-person operations team before pivoting technical. That's why my builds get adopted: I was the stakeholder for years before I was the builder.

| Layer | Tools |
|-------|-------|
| Analytics and BI | Power BI on Fabric, DAX, Power Query (M), SQL |
| Big data | Databricks notebooks, Advana, Qlik |
| Automation | Power Automate, PWAs, bots |
| Under the hood | Python, Postgres, Git, Linux, Docker |

---

## Homelab

Where I prove things work before I trust them. Everything below is running today, in a 3-node Proxmox cluster I operate like production.

| What happened | Why it matters |
|---------------|----------------|
| **Human-in-the-loop AI ops.** An AI agent proposes infrastructure changes as pull requests. I approve from my phone. A deterministic script applies them. The AI never touches infrastructure directly. | The governance problem every org adopting AI agents has, solved small. |
| **Infrastructure as code.** 20+ services in one compose file, zero open firewall ports, Cloudflare Tunnel with zero-trust policies per service. | The whole stack rebuilds from a git repo. |
| **Data integrity, tested.** A ZFS scrub surfaced 15 permanent errors from silent corruption. Traced to 7 files, quarantined, re-acquired, zero library impact. | Backups you haven't tested are a hypothesis. |
| **Disaster recovery, drilled.** UPS with scripted clean shutdown and BIOS restore-on-AC. Then I pulled the plug on purpose and watched it self-recover unattended. | The first drill failed because I pulled the data cable instead of power. Found that in a drill, not an outage. |
| **Data warehouse, shipped.** [fantasy-warehouse](https://github.com/nrd81/fantasy-warehouse): seven data feeds into a Postgres star schema, SQL edge views, and a 9-page Power BI report. Cron refresh, nightly backups, dead-man monitoring. | A full BI pipeline built and operated solo: ingest, model, transform, visualize, monitor. Same discipline as the day-job migrations, end to end on my own iron. |

**Repos:** [fantasy-warehouse](https://github.com/nrd81/fantasy-warehouse) (public) | [homelab-infra](https://github.com/nrd81/homelab-infra) (public) | homelab-operator (private, write-up coming)

---

## How I Decide

Match the problem to the product, not the product to the problem.

- An Access database that three people use doesn't need Databricks.
- A 50-step approval chain doesn't need a dashboard, it needs a flow.
- Diagnose before fixing. Verify every change. Write it down.

---

## Contact

**dingwall1@gmail.com**
