# Benchmaxxer

A fake AI benchmark figure studio. Invent a benchmark, pick real models from
OpenRouter, type whatever numbers flatter you, and export a figure that looks
like it came out of a model launch post.

**Live: https://thefilipcom4607.github.io/benchmaxxer/**

## What it does

- Pulls the live model list from the OpenRouter API, with a paste-the-JSON
  fallback if the fetch is blocked. Search tolerates `gpt 6`, `gpt-6` and `gpt6`.
- Contenders can be individual models or whole labs. Lab mode groups the live
  list by vendor, so Anthropic, OpenAI and Meta become the bars, carrying their
  real model count, longest context window and cheapest price.
- Five figure types: columns, horizontal bars, scatter, line and radar.
- Ten presets, each a finished figure: the cropped-axis special, the
  cost-capability frontier, a scaling law, an arena leaderboard, a lab volume
  chart. The header button shuffles to a random one.
- Auto-scoring modes, including real context windows, real prompt prices, real
  tokens per dollar and how many models a lab has shipped, plus the important
  one: largest integer appearing in the model name.
- The house style copies the conventions of real launch-post charts, including a
  cropped y-axis with a break glyph where zero should be.
- Exports a 2400px-wide PNG or an SVG. The figure is drawn as SVG, so the export
  is exactly what the preview shows.
- Keeps your figure in the browser between reloads.

Everything runs in the browser. No build step, no dependencies, one file.

## Running it locally

Open `index.html`. That is the whole procedure.

## Not real

Every number this produces is made up by you. Do not put the output anywhere it
could be mistaken for an actual evaluation.
