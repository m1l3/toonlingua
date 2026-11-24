# ToonLingua architecture

International, rights-aware cartoon dubbing platform.

## MVP
Upload authorized media, choose target locale (initially mk-MK), create an asynchronous dubbing job, review translated dialogue and synthesized audio, export MP4.

## Components
- Python/FastAPI API and worker
- Vue frontend with locale preferences
- PostgreSQL job metadata
- n8n orchestration
- Whisper transcription with timestamps, translation, licensed synthetic voices, FFmpeg mixing
- Jellyfin for optional private playback

## Pipeline
Validate rights and input → transcribe → identify speakers → translate segments → synthesize → align and mix → review → export.

Never commit videos, API keys or personal data. Use licensed voices; do not clone actors without consent. Keep uploaded files private and set retention limits. Original music/effects separation is experimental.

## Milestones
1. Test Macedonian voice quality with an authorized short clip.
2. Implement job API and provider adapters.
3. Add worker and n8n integration.
4. Add internationalized UI and playback.
5. Add authentication, billing, quotas and rights management before public launch.
