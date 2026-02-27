# Multi-Agent Orchestration

A multi-agent pipeline for ingesting, summarizing, prioritizing, and formatting content into a digest.

## Project Structure

```
multi-agent-orchestration/
├── agents/
│   ├── ingestor/     # Loads and preprocesses raw input files
│   ├── summarizer/   # Summarizes ingested content
│   ├── prioritizer/  # Prioritizes summarized content
│   └── formatter/    # Formats the final digest output
├── data/
│   └── input/        # Your raw files go here
├── output/           # The final digest appears here
├── tests/            # Unit and integration tests
├── .env              # API keys (gitignored!)
└── docker-compose.yml
```

## Prerequisites

- Python 3.11+
- Docker and Docker Compose

## Quick Start

1. Add your API keys to `.env`.
2. Place raw files in `data/input/`.
3. Run with Docker Compose:

   ```bash
   docker compose up
   ```

4. Find the digest in `output/`.

## Development

Run tests:

```bash
pytest tests/
```

## License

MIT
