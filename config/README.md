# H3 LoRA Benchmark — Run Instructions

## What this is
A local RTX 5090 benchmark run for MiniMax H3 video+audio LoRA training using AI Toolkit.
This is a 100-step benchmark only — not the full training run.

## What to use
- Dataset: use clips from `benchmark/` only (~30-50 clips).
- Config: `config/training_config.yaml` — use these settings exactly as given.

## Hardware assumed
- RTX 5090, 32GB VRAM
- 64GB system RAM
- If your hardware differs, flag it before running — settings may need adjustment.

## What to run
1. Load `config/training_config.yaml` into AI Toolkit.
2. Run exactly 100 steps — do not exceed this without approval.
3. Confirm audio is contributing to the training loss (not just video).

## What to report back
- Actual time per step (seconds/step)
- Peak VRAM and system RAM usage
- Any memory errors, crashes, or warnings
- Sample output / checkpoint from the 100-step run

## What NOT to do yet
- Do not scale to 1,000 steps
- Do not use additional clips beyond the benchmark set
- Do not change the config values without checking first
