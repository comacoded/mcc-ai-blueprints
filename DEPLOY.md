# MCC AI Blueprints — Deploy Reference

## Live URL
https://mcc-ai-blueprints-production.up.railway.app

## GitHub
https://github.com/comacoded/mcc-ai-blueprints

## Railway Project
https://railway.com/project/f39cf130-3024-4b48-9275-2db20bcd525b

## File Structure

```
deploy/
├── public/
│   └── index.html     # All content — single self-contained file (256KB)
├── server.js           # Express + compression
├── package.json
├── Procfile
└── .gitignore
```

## How to Update

1. Edit the source file:
   ```
   /Users/nickcoma/Documents/MCC Work/Blueprint Folder/mcc-blueprint-heatmaps.html
   ```

2. Copy to deploy:
   ```
   cp "/Users/nickcoma/Documents/MCC Work/Blueprint Folder/mcc-blueprint-heatmaps.html" \
      "/Users/nickcoma/Documents/MCC Work/Blueprint Folder/deploy/public/index.html"
   ```

3. Commit and deploy:
   ```
   cd "/Users/nickcoma/Documents/MCC Work/Blueprint Folder/deploy"
   git add -A && git commit -m "Update content"
   railway up --detach
   ```

## What's Included

### Comparison & Feasibility (left sidebar)
- **Best to Start With** — Composite ranking across 6 dimensions with clickable breakdowns
- **Feasibility Comparison** — Pairwise heatmap of feasibility profiles
- **Future Extensions** — Growth/productivity comparison heatmap
- **Tech Stack Overlap** — Technology Jaccard similarity heatmap
- **Data Source Overlap** — Data source Jaccard similarity heatmap

### iX Workflow Mapping (left sidebar)
- **Combined View** — Overview dashboard (60 processes, 52% coverage)
- **T&O** — 27 processes, 56% coverage
- **Corporate Affairs** — 33 processes, 48% coverage

## Data Sources
- `MCC_AI_Blueprints_Master.xlsx` — Blueprint scores, Harvey Balls, tech stacks, data sources
- `MCC AI Transformation - Extended and Classified.xlsx` — Consulting classifiers (platform readiness, data readiness, deployment suitability, foundation dependency, operational risk)
- iX workflow mapping HTMLs — T&O, Corporate Affairs, Combined
