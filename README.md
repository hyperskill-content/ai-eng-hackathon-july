# AI Engineer Hackathon: July 2025

This is a starter repository for the July AI Engineer hackathon that contains datasets for MVP validation.

## A Brief Introduction

There are three curated datasets from Reddit where people share experiences and pain points. The datasets were gathered on July 4th, 2025.

#### Vibe-Coding (`vibecoding_neighbourhood/`)

Conversations from r/ChatGPTCoding, r/ClaudeAI, r/cursor, r/PromptEngineering, r/replit, and r/Windsurf. AI-assisted coding discussions from developers using ChatGPT, Claude, Cursor, and other tools.

#### Self-Host (`selfhost_neighbourhood/`)

Conversations from r/homelab, r/LocalLLaMA, r/LocalLLM, r/opensource, r/privacy, and r/selfhosted. Self-hosting and privacy communities sharing infrastructure setups and challenges.  

#### Working with Data (`data_neighbourhood/`)

Conversations from r/BusinessIntelligence, r/datacleaning, r/dataengineering, r/data, r/datascience, and r/datasets. Data professionals from BI, engineering, and science discussing tools and workflows.

## Dataset Structure 

The `starter_datasets/` folder contains three neighbourhoods, with JSON files of the top 500 hot posts from 6 subreddits per neighbourhood.

```
starter_datasets/
├── vibecoding_neighbourhood/     # AI coding tools & workflows
│   ├── reddit_ChatGPTCoding_hot_500.json
│   ├── reddit_ClaudeAI_hot_500.json
│   ├── reddit_cursor_hot_500.json
│   ├── reddit_PromptEngineering_hot_500.json
│   ├── reddit_replit_hot_500.json
│   └── reddit_Windsurf_hot_500.json
├── selfhost_neighbourhood/      # Privacy & self-hosting
│   ├── reddit_homelab_hot_500.json
│   ├── reddit_LocalLLaMA_hot_500.json
│   ├── reddit_LocalLLM_hot_500.json
│   ├── reddit_opensource_hot_500.json
│   ├── reddit_privacy_hot_500.json
│   └── reddit_selfhosted_hot_500.json
└── data_neighbourhood/          # Data professionals
    ├── reddit_BusinessIntelligence_hot_500.json
    ├── reddit_datacleaning_hot_500.json
    ├── reddit_dataengineering_hot_500.json
    ├── reddit_data_hot_500.json
    ├── reddit_datascience_hot_500.json
    └── reddit_datasets_hot_500.json
```

#### Data format
Every JSON file contains an array of posts, where individual posts include:

* Post metadata: ID, title, selftext content, URL, score, upvote ratio, comment count, creation timestamp, author, subreddit
* Post flags: Self-post status, moderation flags (stickied, locked, spoiler, etc.)
* Comment threads (limited to 100 comments): Nested comments with their own metadata (ID, body, score, timestamp, author, parent relationships, thread depth)
* Engagement metrics: Vote scores, comment counts, and interaction ratios  

