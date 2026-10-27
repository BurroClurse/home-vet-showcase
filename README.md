# home-vet

A health record system for my three pets, a dog and two cats, run through Claude Code skills. The repo with the records is private. This page describes how it works.

It deals with the same problems as a human health record. Vet records arrive as PDFs and phone photos, and they need to become structured data before anyone can track a lab trend or check a medication.

## What it does

- **Record intake.** Turns uploaded vet PDFs and photos into structured records for each pet: conditions, medications, vaccines, labs, weights and a timeline.
- **Lab interpretation.** Explains bloodwork and shows trends across visits.
- **Drug check.** Checks medication, product and toxin safety by species, including the MDR1 gene and drug interactions.
- **Literature search.** Searches PubMed limited to dogs and cats with the revised National Library of Medicine species filter.
- **Visit prep.** Writes a one-page summary to bring to the vet.
- **Care schedule.** Shows what's due and sets calendar reminders.

## How it's built

- Each task is a Claude Code skill. The skills can also be installed as a plugin and used outside the repo.
- Records sync between the Mac and cloud sessions through GitHub, with a dry-run check before syncing.
- Shell and Python tests cover the sync script.
