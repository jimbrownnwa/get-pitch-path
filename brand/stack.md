# Marketing Stack

> Written by /start-here. Updated when new tools are connected.
> Last Updated: 2026-04-11 (/start-here)

## Connected Tools

| Tool | Type | Status | Config |
|------|------|--------|--------|
| HubSpot (MCP) | CRM + Email | connected | MCP server active |
| Gmail (MCP) | Personal email | connected | MCP server active |
| Canva (MCP) | Design / graphics | connected | MCP server active |
| Google Calendar (MCP) | Scheduling | connected | MCP server active |
| n8n (MCP) | Workflow automation | connected | MCP server active |
| Telegram (MCP) | Messaging | connected | MCP server active |

## MCP Servers

| Server | Tools Available | Status |
|--------|----------------|--------|
| claude_ai_HubSpot | CRM objects, contacts, properties, owners | running |
| claude_ai_Gmail | Read/search/draft email | running |
| claude_ai_Canva | Design generation, export, folders, editing | running |
| claude_ai_Google_Calendar | Events, free time, calendars | running |
| claude_ai_n8n | Workflow execution + management | running |
| plugin_telegram | Messaging, reactions, attachments | running |

## Not Connected (Recommended)

| Tool | Why | Setup |
|------|-----|-------|
| Replicate | Image/video generation for /creative skill | `setx REPLICATE_API_TOKEN r8_...` |
| Dedicated ESP (ConvertKit / Beehiiv) | Newsletter-native sends, better than HubSpot for creator audiences | Add API key to .env |
| Analytics (GA4 / PostHog) | Track conversion + performance learnings | Add API key to .env |
| Playwright / Firecrawl MCP | Competitor research + SERP analysis for /keyword-research + /seo-content | Install MCP server |

## Notes

- HubSpot MCP can serve as the primary Email ESP for deployment of email sequences until a dedicated creator-focused ESP is connected.
- Canva MCP is available for design work, which complements /creative once a Replicate token is added.
- n8n MCP opens the door to cross-tool automation workflows (similar to Zapier).
