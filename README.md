# YouTube MCP Server

[![MCP Compatible](https://img.shields.io/badge/MCP-Compatible-blue)](https://insightfulpipe.com/mcp-servers/youtube)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **Connect YouTube Data API and YouTube Analytics to AI assistants with MCP.**

The YouTube MCP server unifies YouTube Data API and YouTube Analytics API, enabling Claude, ChatGPT, Cursor, and other AI assistants to analyze your channel performance, video metrics, and audience insights.

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
- Manage playlists and interact with comments

## Installation

### Claude

1. Copy the MCP Server URL: `https://youtube.insightfulmcp.com/`
2. Open [Claude Connectors Settings](https://claude.ai/settings/connectors)
3. Scroll to the bottom and click **Add custom connector**
4. Paste the URL and click **Add**
5. Click **Connect** on the connector to start authorization
6. Click **Authorize access** in the browser to complete the connection

### ChatGPT

1. Copy the MCP Server URL: `https://youtube.insightfulmcp.com/`
2. Open ChatGPT Settings → **Connections**
3. Click **Add Connection** and paste the URL
4. Authorize with your InsightfulPipe account

### Claude Code

```bash
claude mcp add youtube https://youtube.insightfulmcp.com/
```

### Cursor

1. Open Cursor Settings → **MCP Servers**
2. Add new server with URL: `https://youtube.insightfulmcp.com/`
3. Authorize the connection

## Available Actions

### YouTube Data API (Read)

| Action | Description |
|--------|-------------|
| `get_activities` | Lists channel activity events (uploads, likes, favorites, comments, subscriptions) |
| `get_search` | Search for YouTube videos, channels, and playlists |
| `get_videos` | Get video details, statistics, and content information |
| `get_channels` | Get channel information, statistics, and content details |
| `get_playlists` | List playlists by channel ID or playlist IDs |
| `get_playlistitems` | Get items within a playlist |
| `get_subscriptions` | List subscriptions and subscribers |
| `get_comments` | Get individual comments |
| `get_commentthreads` | Get all comment threads (top-level comments and replies) for a video or channel |
| `get_videocategories` | Get video categories for a region |
| `get_videoabusereportreasons` | Get video abuse report reasons |
| `get_members` | Get channel members (requires membership features) |
| `get_membershipslevels` | Get membership levels for a channel |
| `get_videos_trending` | Get trending/popular videos by region and category |
| `get_channels_topvideos` | Get the most-viewed videos from a specific channel |

### YouTube Data API (Write)

| Action | Description |
|--------|-------------|
| `insert_playlistitem` | Add a video to a playlist |
| `update_playlistitem` | Update a playlist item (position, notes) |
| `insert_comment` | Reply to an existing comment (creates replies, not top-level comments) |
| `update_comment` | Update comment text |
| `delete_comment` | Delete a comment |
| `update_video` | Update video metadata (title, description, tags, privacy) |
| `insert_playlist` | Create a new playlist |
| `update_playlist` | Update playlist metadata |

### YouTube Analytics

| Action | Description |
|--------|-------------|
| `channel_basic` | Channel performance metrics (basic) |
| `channel_cards` | Card interactions (use params to add card dimensions) |
| `channel_combined` | Combined channel metrics |
| `channel_demographics` | Channel metrics by demographic segments |
| `channel_device_os` | Channel metrics by device/OS |
| `channel_end_screens` | End screen performance |
| `channel_playback_location` | Channel metrics by playback location |
| `channel_province` | Channel metrics by province |
| `channel_sharing_service` | Channel metrics by sharing service |
| `channel_subtitles` | Channel metrics by subtitle language |
| `channel_traffic_source` | Traffic source metrics |
| `playlist_basic` | Playlist metrics |
| `playlist_combined` | Combined playlist metrics |
| `playlist_device_os` | Playlist metrics by device/OS |
| `playlist_playback_location` | Playlist metrics by playback location |
| `playlist_province` | Playlist metrics by province |
| `playlist_traffic_source` | Playlist traffic sources |

## Usage Examples

### Channel Performance

```
"How is my YouTube channel performing this month?"
```

### Video Analysis

```
"Which of my videos have the highest average view duration?"
```

### Search YouTube

```
"Search for videos about 'machine learning tutorials'"
```

### Audience Insights

```
"What demographics make up my YouTube audience?"
```

### Traffic Analysis

```
"Where is my YouTube traffic coming from?"
```

### Manage Playlists

```
"Add my latest video to the 'Best of 2024' playlist"
```

## Why YouTube MCP?

### For YouTubers
- **Performance insights** - Understand what's working
- **Content ideas** - AI-driven topic suggestions
- **Growth tracking** - Monitor channel progress

### For Video Marketers
- **Campaign analysis** - Track video marketing ROI
- **Competitive research** - Analyze competitor channels
- **Trend identification** - Stay ahead of content trends

### For Agencies
- **Multi-channel management** - Handle multiple YouTube accounts
- **Automated reporting** - Generate client reports easily
- **Performance benchmarking** - Compare across channels

## Security & Privacy

- **Google OAuth 2.0** - Secure YouTube authentication
- **Granular permissions** - Control read vs write access
- **YouTube Partner** - Official API integration
- **Data encryption** - Secure data handling

## Related MCP Servers

- [Google Ads MCP](https://insightfulpipe.com/mcp-servers/google-ads) - YouTube advertising
- [TikTok Ads MCP](https://insightfulpipe.com/mcp-servers/tiktok-ads) - Short-form video ads
- [Instagram MCP](https://insightfulpipe.com/mcp-servers/instagram) - Social video analytics

## Resources

- [Documentation](https://insightfulpipe.com/docs/youtube)
- [Video Tutorial](https://www.youtube.com/playlist?list=PLJNzvjxzI5Xwe__BJJLAelSF0ewO3mEFk)
- [InsightfulPipe Blog](https://insightfulpipe.com/blogs)

## Support

- **Documentation**: [insightfulpipe.com/docs](https://insightfulpipe.com/docs)
- **Email**: support@insightfulpipe.com

## License

MIT License - see [LICENSE](LICENSE) for details.
