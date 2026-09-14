# YouTube MCP Server by Insightful Pipe

[![MCP Compatible](https://img.shields.io/badge/MCP-Compatible-blue)](https://insightfulpipe.com/mcp-servers/youtube)
[![Insightful Pipe](https://img.shields.io/badge/Insightful_Pipe-MCP_Servers-purple)](https://insightfulpipe.com/mcp-servers)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **Connect YouTube Analytics to AI assistants with MCP.**

Part of the [Insightful Pipe MCP Server Collection](https://insightfulpipe.com/mcp-servers) — The YouTube MCP server brings YouTube Analytics reports to Claude, ChatGPT, Cursor, and other AI assistants to analyze your channel performance, video metrics, and audience insights.

[![Explore All MCP Servers](https://img.shields.io/badge/Explore_All-MCP_Servers-blue?style=for-the-badge)](https://insightfulpipe.com/mcp-servers)

![YouTube MCP Server](https://insightfulpipe.com/images/youtube-color-icon.svg)

## MCP Server URL

```
https://youtube.insightfulmcp.com/
```

## What is YouTube MCP?

YouTube MCP is a **remote Model Context Protocol server** that provides AI assistants with access to your YouTube channel data. This comprehensive integration allows you to:

- Query video performance using natural language
- Analyze channel growth and subscriber trends
- Get AI-powered content recommendations
- Monitor watch time, views, and engagement

## Installation

### Claude

1. Copy the MCP Server URL: `https://youtube.insightfulmcp.com/`
2. Open [Claude Connectors Settings](https://claude.ai/settings/connectors)
3. Scroll to the bottom and click **Add custom connector**
4. Paste the URL and click **Add**
5. Click **Connect** on the connector to start authorization
6. Click **Authorize access** in the browser to complete the connection

### ChatGPT

Custom MCP servers are added through ChatGPT's **Developer mode**. Availability depends on your ChatGPT plan, and workspace admins may need to allow it.

1. Turn on **Developer mode** in ChatGPT settings
2. Create a new app for a remote MCP server and paste the URL: `https://youtube.insightfulmcp.com/`
3. Authorize with your InsightfulPipe account

See OpenAI's guide: [Developer mode and MCP apps in ChatGPT](https://help.openai.com/en/articles/12584461-developer-mode-and-mcp-apps-in-chatgpt)

### Claude Code

```bash
claude mcp add --transport http youtube https://youtube.insightfulmcp.com/
```

### Cursor

Add the server to `~/.cursor/mcp.json` (all projects) or `.cursor/mcp.json` (one project):

```json
{
  "mcpServers": {
    "youtube": {
      "url": "https://youtube.insightfulmcp.com/"
    }
  }
}
```

Then authorize the connection when Cursor prompts you.

## Available Actions

21 actions: 21 read, 0 write.

### Read Actions (21)

| Action | Description |
|--------|-------------|
| `channel` | Channel-level performance metrics including views, watch time, subscribers, and engagement |
| `channel_basic` | Channel performance metrics (basic) |
| `channel_cards` | Card interactions (use params to add card dimensions) |
| `channel_combined` | Combined channel metrics |
| `channel_demographics` | Channel metrics by demographic segments (age group and gender) |
| `channel_device_os` | Channel metrics by device/OS (override dimensions) |
| `channel_end_screens` | End screen performance (override dimensions to include end screen types) |
| `channel_playback_location` | Channel metrics by playback location (override dimensions to playbackLocationType) |
| `channel_province` | Channel metrics by province |
| `channel_sharing_service` | Channel metrics by sharing service |
| `channel_traffic_source` | Traffic source metrics (override dimensions for detailed sources) |
| `demographics` | Audience demographics data including age groups and gender breakdown |
| `playlist_basic` | Playlist metrics (supply filters/dimensions to target playlists) |
| `playlist_combined` | Combined playlist metrics |
| `playlist_device_os` | Playlist metrics by device/OS (override dimensions) |
| `playlist_playback_location` | Playlist metrics by playback location |
| `playlist_province` | Playlist metrics by province |
| `playlist_traffic_source` | Playlist traffic sources |
| `reports.query` | Custom YouTube Analytics reports query - specify metrics, dimensions, and filters |
| `traffic_sources` | Traffic source data showing where viewers discover your content |
| `video` | Video-level performance metrics including views, watch time, and engagement |

## Control What Your AI Can Do

You decide what AI agents can do with each connected account:

- **Turn individual actions on or off** for every connected account, so agents only see the actions you allow.
- **Connect as Read-only or Read & Write.** A read-only connection can only enable read actions.
- **Destructive actions stay off by default.** Actions such as deletes are disabled until an admin enables them.
- **Team access per account.** Restricted team members only use the accounts they are granted, with the read actions enabled on them.

## Usage Examples

### Channel Performance

```
"How is my YouTube channel performing this month?"
```

### Playlist Analysis

```
"Which of my playlists get the most watch time?"
```

### Audience Insights

```
"What demographics make up my YouTube audience?"
```

### Traffic Analysis

```
"Where is my YouTube traffic coming from?"
```

## Why YouTube MCP?

### For YouTubers
- **Performance insights** - Understand what's working
- **Content ideas** - AI-driven topic suggestions
- **Growth tracking** - Monitor channel progress

### For Video Marketers
- **Campaign analysis** - Track video marketing ROI
- **Trend identification** - Stay ahead of content trends

### For Agencies
- **Multi-channel management** - Handle multiple YouTube accounts
- **Automated reporting** - Generate client reports easily
- **Performance benchmarking** - Compare across channels

## Security & Privacy

- **Google OAuth 2.0** - Secure YouTube authentication
- **Read-only reports** - No changes to your channel
- **Official YouTube API** - Direct integration with Google's API
- **Data encryption** - Secure data handling

## Ready-Made Skills and Prompts

- [Youtube Channel Performance Dashboard](https://insightfulpipe.com/marketing-prompts-library/youtube-youtube-channel-performance-dashboard)
- [Youtube Video Performance Analysis](https://insightfulpipe.com/marketing-prompts-library/youtube-youtube-video-performance-analysis)
- [Youtube Audience Demographics Report](https://insightfulpipe.com/marketing-prompts-library/youtube-youtube-audience-demographics-report)

## Explore More MCP Servers by Insightful Pipe

Visit **[insightfulpipe.com/mcp-servers](https://insightfulpipe.com/mcp-servers)** to discover our full collection of MCP servers for marketing and analytics.

### Video & Social MCP Servers
- [TikTok Ads MCP](https://insightfulpipe.com/mcp-servers/tiktok-ads) - Short-form video ads
- [Instagram MCP](https://insightfulpipe.com/mcp-servers/instagram) - Social video analytics
- [Facebook Pages MCP](https://insightfulpipe.com/mcp-servers/facebook-pages) - Facebook video

### Advertising MCP Servers
- [Google Ads MCP](https://insightfulpipe.com/mcp-servers/google-ads) - YouTube advertising
- [Facebook Ads MCP](https://insightfulpipe.com/mcp-servers/facebook-ads) - Meta advertising

**[View All MCP Servers →](https://insightfulpipe.com/mcp-servers)**

## Resources

- [Documentation](https://insightfulpipe.com/docs/connectors-youtube)
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
