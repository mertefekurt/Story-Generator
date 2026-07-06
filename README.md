# Story Generator

![Story Generator cover](assets/readme-cover.svg)

Long-form story drafting from a configurable theme, plot, tone, audience, and chapter count. The project keeps character, location, and event context close to the generation flow so longer manuscripts are easier to revise.

## Setup

```bash
git clone https://github.com/mertefekurt/Story-Generator.git
cd Story-Generator
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
cp theme.config theme.local.config
```

Add your key to `.env`, then run:

```bash
python story_generator.py --config theme.local.config
```

## Main files

```text
story_generator.py   generator, models, client, memory flow
theme.config         story configuration template
install_and_run.sh   guided setup
test_pdf.py          PDF rendering check
```
