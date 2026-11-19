# scalp-bot

Workspace for building and testing a scalping trading strategy.

## Tools

### `/watch` — video analysis skill

Vendored from [bradautomates/claude-video](https://github.com/bradautomates/claude-video)
(v0.3.2, MIT — see `.claude/skills/watch/LICENSE`). Lets Claude Code read a
video (URL or local file) as timestamped frames + transcript, e.g. to pull a
strategy's rules out of a trading tutorial.

Requirements: Python 3.10+, `ffmpeg`/`ffprobe`, and `yt-dlp`
(`pip install "yt-dlp[default]"`). Optional: a `GEMINI_API_KEY` in
`~/.config/watch/.env` to let Gemini watch the whole video.

Check setup:

```bash
python3 .claude/skills/watch/scripts/setup.py --json
```
