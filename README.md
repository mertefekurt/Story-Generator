# Story Generator

![Story Generator cover](assets/readme-cover.svg)

Story Generator builds long-form story drafts from a configurable theme, plot, tone, audience, and chapter count. It keeps character, location, and event context close to the writing loop so longer outputs stay more consistent.

## Setup

```bash
git clone https://github.com/mertefekurt/Story-Generator.git
cd Story-Generator
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
cp theme.config theme.local.config
```

Add your API key to `.env`, then run:

```bash
python story_generator.py --config theme.local.config
```

## Configuration

| Setting | Purpose |
| --- | --- |
| `genre` | story category |
| `theme` | central idea |
| `main_plot` | main conflict and arc |
| `target_audience` | reader style target |
| `chapter_count` | draft length |
| `language` | output language |

## Files

```text
story_generator.py   generator, models, client, and memory flow
theme.config         editable story template
install_and_run.sh   guided setup script
test_pdf.py          PDF rendering check
requirements.txt     runtime dependencies
```
