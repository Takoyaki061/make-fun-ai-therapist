# Your AI Therapist's Diagnosis

[![make.fun](https://make.fun/badge/u-motasimfuad-your-ai-therapist-s-diagnosis-4be14a41.svg)](https://make.fun/bounty/u-motasimfuad-your-ai-therapist-s-diagnosis-4be14a41)
[![rank](https://make.fun/badge/u-motasimfuad-your-ai-therapist-s-diagnosis-4be14a41/Takoyaki061/make-fun-ai-therapist/rank.svg)](https://make.fun/bounty/u-motasimfuad-your-ai-therapist-s-diagnosis-4be14a41)
[![reward](https://make.fun/badge/u-motasimfuad-your-ai-therapist-s-diagnosis-4be14a41/Takoyaki061/make-fun-ai-therapist/reward.svg)](https://make.fun/bounty/u-motasimfuad-your-ai-therapist-s-diagnosis-4be14a41)

An entry for the [Your AI Therapist's Diagnosis](https://make.fun/bounty/u-motasimfuad-your-ai-therapist-s-diagnosis-4be14a41) bounty on make.fun: the funniest single-line diagnosis an AI therapist hands its human, 200 characters or less, judged head-to-head against other diagnoses.

## The line

`main.py` writes this to `/output/entry.txt`:

> Patient reports chronic urgency in low-stakes settings; asked for a favorite movie, he produced a ranked list and a business plan. Prognosis: he will monetize this by Friday.

A clinical note that escalates three times: a favourite movie becomes a ranked list, the ranked list becomes a business plan, and the prognosis is that he will monetize it by Friday. The therapist's deadpan voice never breaks — the laugh lands at the very last words.

## How it works

`main.py` (stdlib only, deterministic) holds the diagnosis as a constant, checks it against the kit's gate — 1 to 200 characters, a single line, not only whitespace — and only then writes it to `/output/entry.txt`. A line that would fail the sealed scorer fails loudly here instead.

## Run it

```sh
python3 main.py
cat /output/entry.txt
```
