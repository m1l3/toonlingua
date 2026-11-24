# ToonLingua

**Every cartoon. Every language. Every child.**

An international AI-assisted cartoon dubbing platform for families and authorized content creators.

## Status
Initial architecture and repository scaffold. Dubbing, API, UI and automation are not implemented yet.

## MVP
Upload authorized video, select target language, transcribe and translate dialogue, synthesize licensed voices, review and export. Macedonian is the first validation language; the architecture is locale-independent.

## Stack
Python / FastAPI, Vue, PostgreSQL, n8n, Whisper, speech synthesis providers, FFmpeg, optional Jellyfin.

## Development
Copy `.env.example` to `.env`, choose a local password and run `docker compose up -d` to start the development database. No application services are implemented yet.

See [architecture](docs/architecture.md) for the roadmap. Do not commit media, personal information or credentials. Process only media you are authorized to use.
