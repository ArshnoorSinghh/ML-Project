# work/ — your space

Everything you build lives here: lane experiments, notebooks, figures, and your capstone
report. The rest of the repo is the shared reference; this folder is yours.

## Rules of the road

1. **Copy, don't edit.** Need to change the pipeline? Copy the script here
   (e.g. `work/scripts/03_train_model_v2.py`) or adjust the feature lists in
   `scripts/ml_utils.py`. The reference pipeline in `scripts/` stays pristine — it's the
   baseline you compare against, and reviewers expect to find it unchanged.
2. **No datasets in git.** CSVs inside `work/` are gitignored, and CI fails if any dataset
   CSV is committed anywhere in the repo. Small summary tables belong in your report as
   markdown, not as data files.
3. **Stay reproducible.** Fix your random seeds and note them in your report. Someone with a
   fresh clone should be able to re-run your work from your instructions alone.
4. **Public-safety language.** Everything here may end up public with your submission:
   observed / measured / directional / decision-support — no client-identifying details,
   no causal claims without a design (see `DATA_USE.md`).

## Suggested layout

```text
work/
  notebooks/            your experiment notebooks
  scripts/              copied + modified pipeline pieces
  figures/              charts for your report
  capstone_report.md    your capstone write-up (start from the template)
```

## Capstone

Copy `capstone_report_template.md` to `capstone_report.md` and fill it in as you go — it
mirrors the eight axes your work is graded on, so writing it early keeps you honest.
