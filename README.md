# Enrichment MCP Server by Insightful Pipe

[![MCP Compatible](https://img.shields.io/badge/MCP-Compatible-blue)](https://insightfulpipe.com/mcp-servers/enrichment)
[![Insightful Pipe](https://img.shields.io/badge/Insightful_Pipe-MCP_Servers-purple)](https://insightfulpipe.com/mcp-servers)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **Enrich company and contact data with AI-powered data discovery through MCP.**

Part of the [Insightful Pipe MCP Server Collection](https://insightfulpipe.com/mcp-servers) — The Enrichment MCP server enables Claude, ChatGPT, Cursor, and other AI assistants to enrich business data. Get company profiles, funding data, tech stacks, and leadership information from email addresses and domains.

[![Explore All MCP Servers](https://img.shields.io/badge/Explore_All-MCP_Servers-blue?style=for-the-badge)](https://insightfulpipe.com/mcp-servers)

![Enrichment MCP Server](https://insightfulpipe.com/images/ip-logo.png)

## MCP Server URL

```
https://enrichment-crawlers.insightfulmcp.com/
```

## What is Enrichment MCP?

Enrichment MCP is a **remote Model Context Protocol server** that provides AI-powered data enrichment capabilities. This data intelligence integration allows you to:

- Enrich company data from email addresses
- Get detailed company profiles and metrics
- Discover tech stacks and tools used
- Find leadership and decision-maker information
- Access funding history and company size data

## Installation

### Claude

1. Copy the MCP Server URL: `https://enrichment-crawlers.insightfulmcp.com/`
2. Open [Claude Connectors Settings](https://claude.ai/settings/connectors)
3. Scroll to the bottom and click **Add custom connector**
4. Paste the URL and click **Add**
5. Click **Connect** on the connector to start authorization
6. Click **Authorize access** in the browser to complete the connection

### ChatGPT

Custom MCP servers are added through ChatGPT's **Developer mode**. Availability depends on your ChatGPT plan, and workspace admins may need to allow it.

1. Turn on **Developer mode** in ChatGPT settings
2. Create a new app for a remote MCP server and paste the URL: `https://enrichment-crawlers.insightfulmcp.com/`
3. Authorize with your InsightfulPipe account

See OpenAI's guide: [Developer mode and MCP apps in ChatGPT](https://help.openai.com/en/articles/12584461-developer-mode-and-mcp-apps-in-chatgpt)

### Claude Code

```bash
claude mcp add --transport http enrichment https://enrichment-crawlers.insightfulmcp.com/
```

### Cursor

Add the server to `~/.cursor/mcp.json` (all projects) or `.cursor/mcp.json` (one project):

```json
{
  "mcpServers": {
    "enrichment": {
      "url": "https://enrichment-crawlers.insightfulmcp.com/"
    }
  }
}
```

Then authorize the connection when Cursor prompts you.

## Available Actions

6 actions: 6 read, 0 write.

### Read Actions (6)

| Action | Description |
|--------|-------------|
| `discovery-crawler` | Identify company name, website, and description from email |
| `funding-crawler` | Gather funding and investment data (rounds, investors, valuation) |
| `leadership-crawler` | Gather leadership and executive information |
| `metrics-crawler` | Gather company metrics (employee count, revenue, growth) |
| `profile-crawler` | Gather company profile (industry, headquarters, year founded) |
| `tech-stack-crawler` | Detect technologies, languages, and frameworks used |

## Control What Your AI Can Do

You decide what AI agents can do with each connected account:

- **Turn individual actions on or off** for every connected account, so agents only see the actions you allow.
- **Connect as Read-only or Read & Write.** A read-only connection can only enable read actions.
- **Destructive actions stay off by default.** Actions such as deletes are disabled until an admin enables them.
- **Team access per account.** Restricted team members only use the accounts they are granted, with the read actions enabled on them.

## Usage Examples

### Company Discovery

```
"Identify the company for this email: john@acme.com"
```

### Company Profile

```
"Get the company profile for stripe.com"
```

### Tech Stack Discovery

```
"What technologies does notion.so use?"
```

### Leadership Lookup

```
"Who are the executives at anthropic.com?"
```

### Funding Data

```
"What's the funding history of openai.com?"
```

### Company Metrics

```
"Get employee count and revenue estimates for salesforce.com"
```

## Available Data Points

| Data Point | Description |
|------------|-------------|
| Company Name | Official company name |
| Industry | Business sector classification |
| Employee Count | Company size |
| Revenue Range | Estimated revenue |
| Funding Total | Total funding raised |
| Tech Stack | Technologies used |
| Headquarters | Location and address |
| Leadership | Key executives and founders |
| Year Founded | Company founding year |
| Website | Company website URL |

## Why Enrichment MCP?

### For Sales Teams
- **Lead qualification** - Instant company insights
- **Contact discovery** - Find decision makers
- **Account research** - Comprehensive profiles

### For Marketing Teams
- **List enrichment** - Enhance contact databases
- **Segmentation** - Better audience targeting
- **Personalization** - Relevant outreach

### For Analysts
- **Market research** - Company and industry data
- **Competitive analysis** - Competitor insights
- **Investment research** - Funding and growth data

## Enrichment Workflows

### Lead Scoring
Enrich leads with company size and funding to prioritize outreach.

### ABM Campaigns
Build comprehensive account profiles for account-based marketing.

### CRM Enhancement
Automatically enrich CRM records with fresh data.

### Competitive Intelligence
Monitor competitor tech stacks and hiring trends.

## Security & Privacy

- **Data encryption** - Secure transmission

## Ready-Made Skills and Prompts

- [Full Company Enrichment From Email](https://insightfulpipe.com/marketing-prompts-library/enrichment-full-company-enrichment-from-email)
- [Lead Qualification Enrichment](https://insightfulpipe.com/marketing-prompts-library/enrichment-lead-qualification-enrichment)
- [Competitor Company Research](https://insightfulpipe.com/marketing-prompts-library/enrichment-competitor-company-research)

## Explore More MCP Servers by Insightful Pipe

Visit **[insightfulpipe.com/mcp-servers](https://insightfulpipe.com/mcp-servers)** to discover our full collection of MCP servers for marketing and analytics.

### B2B & Data MCP Servers
- [LinkedIn Ads MCP](https://insightfulpipe.com/mcp-servers/linkedin-ads) - B2B advertising
- [Web Crawler MCP](https://insightfulpipe.com/mcp-servers/crawler) - Web scraping

### Analytics MCP Servers
- [Google Analytics MCP](https://insightfulpipe.com/mcp-servers/google-analytics) - Visitor analytics
- [Google Ads MCP](https://insightfulpipe.com/mcp-servers/google-ads) - Google advertising

**[View All MCP Servers →](https://insightfulpipe.com/mcp-servers)**

## Resources

- [Documentation](https://insightfulpipe.com/docs/connectors-enrichment-crawlers)
- [Video Tutorial](https://www.youtube.com/playlist?list=PLJNzvjxzI5Xwe__BJJLAelSF0ewO3mEFk)
- [InsightfulPipe Blog](https://insightfulpipe.com/blog)

## Support

- **Documentation**: [insightfulpipe.com/docs](https://insightfulpipe.com/docs)
- **All MCP Servers**: [insightfulpipe.com/mcp-servers](https://insightfulpipe.com/mcp-servers)
- **Email**: support@insightfulpipe.com

---

**[Insightful Pipe](https://insightfulpipe.com)** — AI-powered marketing analytics through MCP servers. [Explore all integrations →](https://insightfulpipe.com/mcp-servers)

## License

MIT License - see [LICENSE](LICENSE) for details.
