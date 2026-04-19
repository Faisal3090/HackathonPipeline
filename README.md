# P95.AI Lead Outreach Pipeline

## What this does
Automated intelligent lead qualification and personalized outreach 
system for P95.AI built with n8n + Ollama (llama3.2).

## Pipeline Architecture
## A/B Testing
- Hot leads get 2 variants:
  - Variant A: p95 latency/reliability pain point
  - Variant B: alert fatigue/on-call burnout pain point

## Tech Stack
- n8n (automation pipeline)
- Ollama + llama3.2 (local AI, completely free)
- Gmail API (sending)
- Google Sheets API (logging)
- Clay.com (lead enrichment)
- Cloudflare Tunnel (webhook exposure)

## Lead Scoring
- Hot (score 75+): Direct pitch, 15-min call CTA
- Warm (score 50-74): Friendly, offer free audit
- Cold (score below 50): Light touch, offer benchmark report

## How to run
1. Install n8n: `npx n8n`
2. Install Ollama: https://ollama.com
3. Pull model: `ollama pull llama3.2`
4. Import workflow JSON into n8n
5. Add Gmail credentials (Google Cloud OAuth)
6. Add Google Sheets credentials
7. Execute workflow

## Files
- `HackathonPipeline.json` — n8n pipeline
