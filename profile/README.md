<p align="center">
  <img src="https://gata.works/img/logo-header.png" alt="Gata Router Logo" width="128" height="128">
</p>

<h1 align="center">Gata Router</h1>

<p align="center">
  <strong>AI Powered Ticket Router for Zendesk</strong><br>
  Route support tickets with 90%+ accuracy. Reduce triage time. Let your team focus on solving problems.
</p>

<p align="center">
  <a href="https://github.com/gata-router/terraform-aws-gata/blob/main/LICENSE.txt"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT License"></a>
  <a href="https://gata.works"><img src="https://img.shields.io/badge/website-gata.works-orange.svg" alt="Website"></a>
</p>

---

## What is Gata?

Gata triages and routes Zendesk support tickets using machine learning. Instead of humans manually categorising tickets, Gata analyses content, assigns priority, and routes to the appropriate team automatically.

Everything runs in your AWS account. The only external data exchange is with Zendesk.

**Ideal for teams with:**
- 1,000+ tickets per month
- 80%+ of tickets arriving unclassified
- Balanced or uneven distribution of ticket categories

## Get Started

Ready to deploy? The [Terraform module](https://github.com/gata-router/terraform-aws-gata) is your starting point.

```sh
git clone git@github.com:gata-router/terraform-aws-gata.git
cd terraform-aws-gata/examples/quickstart
```

Check the [quickstart guide](https://github.com/gata-router/terraform-aws-gata/tree/main/examples/quickstart) to get up and running.

## Need Help?

If you want hands-on support deploying Gata or need custom development for your environment, [get in touch](https://gata.works/#contact). We offer:

- Installation and configuration
- Custom integrations
- Workflow customisation
- Ongoing maintenance and support

Gata is backed by [Dave Hall Consulting](https://davehall.com.au), an IT services company with over two decades of experience.

## Repositories

| Repository | Description |
|------------|-------------|
| [terraform-aws-gata](https://github.com/gata-router/terraform-aws-gata) | Terraform module for deploying Gata on AWS. Start here. |
| [gata-data-prep](https://github.com/gata-router/gata-data-prep) | Prepares training datasets from your Zendesk ticket history. |
| [gata-finetune](https://github.com/gata-router/gata-finetune) | Fine-tunes the BERT model on your ticket data. |
| [gata-inference](https://github.com/gata-router/gata-inference) | Runs the trained model for real-time ticket classification. |

## How It Works

Gata uses the right model for each task:

- **Routing** — A BERT model fine-tuned on your historic ticket data
- **Prioritisation** — Amazon Nova Micro for cost-effective priority assignment
- **Summarisation** — Amazon Nova Lite summarises closed tickets

Target cost: **$0.02–0.05 USD per ticket** including all AWS infrastructure.

## License

Gata Router is released under the [MIT License](https://github.com/gata-router/terraform-aws-gata/blob/main/LICENSE.txt).

---

Built and maintained by [Dave Hall Consulting](https://davehall.com.au)
