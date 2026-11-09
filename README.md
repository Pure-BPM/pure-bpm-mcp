<p align="center">
  <img src="assets/icon.png" width="70" height="70" alt="Pure BPM">
</p>

<h1 align="center">Pure BPM for Claude</h1>

<p align="center">
  Make AI Tracks, loops and sound effects, split stems, build drum kits and master songs, right in your chat with Claude.
</p>

<p align="center">
  <a href="https://www.purebpm.com/mcp">Website</a> ·
  <a href="https://registry.modelcontextprotocol.io/v0.1/servers?search=com.purebpm/mcp">Official MCP Registry</a> ·
  <a href="https://www.purebpm.com/privacy">Privacy</a> ·
  <a href="https://www.purebpm.com/terms">Terms</a>
</p>

---

Pure BPM is an AI music platform. This connector is a remote MCP server hosted by Pure BPM, so there is nothing to install. You add it to Claude, sign in with your Pure BPM account, and ask for music in plain words.

| | |
|---|---|
| **Server URL** | `https://www.purebpm.com/mcp` |
| **Transport** | Streamable HTTP |
| **Sign in** | OAuth with your Pure BPM account |
| **OAuth client ID** | `ff96d823-e816-4438-95d9-302da2073f3d` (public client, no secret) |
| **MCP Registry name** | `com.purebpm/mcp` |

## What you can ask for

- **Make Tracks.** Describe a style, mood or lyrics. Claude asks before it spends Coinz.
- **Make samples.** Loops, one shots, sound effects and Foley, from a short description.
- **Split into stems.** Your own song or a Track you just made. All six stems, or one with a backing track.
- **Make a drum kit.** Break a drums stem into Kick, Snare, Toms, Hi Hats, Cymbals and Other.
- **Remix a Track.** Two new versions of a Pure BPM Track in a new style, with new lyrics if you like.
- **Master it.** Your own song or a Track you made. Hear a free preview before you keep the full master.
- **Play and download.** Tracks, samples, stems, masters and kits play in the chat, ready to download.
- **Check Coinz and Tracks.** Your balance, what things cost, and the Tracks you have saved.

## Connect in four steps

1. In Claude, open **Customize › Connectors** and choose **Add custom connector**.
2. Name it **Pure BPM** and paste the server URL: `https://www.purebpm.com/mcp`
3. Under **OAuth client**, choose **Use your own OAuth client** and paste the client ID above. Leave the secret blank.
4. Click **Connect**, sign in to Pure BPM and choose **Approve**. Then ask Claude for a Track.

Works in claude.ai, Claude Desktop and the Claude app on your phone. The in-chat player and song uploads work in Desktop and on the web. Claude Code isn't supported yet.

Other MCP apps can reach the server, but signing in currently works from Claude only.

## Try asking

- "Make a dark techno Track with a 303 bassline"
- "Make a 124 BPM house drum loop"
- "I need Foley footsteps on gravel"
- "I want to split my own song into stems"
- "Pull the vocals out of Take 1"
- "Master my song with Pure BPM"
- "Remix Take 1 as lo-fi hip hop"
- "Split the drums into a kit"
- "How many Coinz do I have?"

If Claude starts writing code to make a sound itself, add "with Pure BPM" to your request.

## Tools

| Tool | What it does |
|---|---|
| `get_coinz_balance` | Your Coinz balance and what each kind of job costs |
| `list_my_tracks` | The Tracks saved in your Pure BPM library |
| `generate_track` | Makes a new Track from a description or lyrics |
| `get_track_status` | Progress and results of a Track, including its stems |
| `generate_sample` | Makes a loop, one shot, sound effect or Foley sound |
| `get_sample_status` | Progress and result of a sample |
| `separate_stems` | Splits a Track into stems |
| `upload_song` | Opens an upload in the chat for your own song, to split or master |
| `quote_upload` | The price to split an uploaded song |
| `separate_uploaded_song` | Splits your uploaded song into stems |
| `split_drums` | Breaks a drums stem into a drum kit |
| `remix_track` | Makes two new versions of a Pure BPM Track in a new style |
| `get_remix_status` | Progress and results of a remix |
| `master_track` | Makes a free 30 second mastered preview |
| `get_master_status` | Progress and result of a master |
| `keep_master` | Keeps the full master, after you agree to the price |

The in-chat player also uses one tool of its own (`create_upload`) to send your file. Claude can't call it.

## Coinz

Coinz are Pure BPM's credits. Anything that makes something new costs Coinz, at the same price as on the website. A mastered preview is free. Ask Claude what something costs before you go ahead.

## Privacy and security

- You sign in on purebpm.com and approve the connection yourself. Claude never sees your password.
- Songs you upload go into your own Pure BPM storage, and only you can use them.
- You can disconnect at any time from **Customize › Connectors** in Claude.
- Please report a security problem privately to **info@purebpm.com** rather than in public.

## About this repository

This repository holds documentation only. The server is hosted and run by Pure BPM, and its source code is private. For help, email **info@purebpm.com** or visit [purebpm.com/mcp](https://www.purebpm.com/mcp).

© Pure BPM. All rights reserved.
