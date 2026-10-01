# Task 06 – Constructing and Evaluating Synthetic Media

## Overview

This repository documents an academic experiment involving the creation,
iteration, and evaluation of synthetic audio and video.

The project uses verified descriptive statistics derived from three social-media
datasets associated with the 2024 presidential election.

Two synthetic-media approaches were evaluated:

1. ElevenLabs synthetic audio
2. Vidnoz AI synthetic avatar video

> **Synthetic Media Disclosure:** All audio and video artifacts in this
> repository were generated using artificial intelligence for academic research.
> No real person's identity or cloned voice was used.

## Research Question

How do generation choices such as pacing, pauses, voice characteristics,
facial expressions, and synchronization affect the perceived realism of
synthetic media?

## Approach 1 – ElevenLabs

Two versions of synthetic narration were generated using the Siren synthetic
voice.

Version 1 was approximately 1 minute 58 seconds.

Version 2 modified the pause structure to investigate whether stronger
separation between ideas would improve perceived realism.

Version 1 was ultimately selected as the stronger audio artifact because
Version 2 sounded faster and made some synthetic characteristics more
noticeable.

## Approach 2 – Vidnoz

Two synthetic-avatar videos were generated using the Annie avatar and
Annie (Lifelike) voice.

Version 1 duration: approximately 46.1 seconds.

Version 2 duration: approximately 51.4 seconds.

Version 2 used shorter sentences and stronger pauses. However, the resulting
longer pauses disrupted the pacing and made the synthetic presentation appear
less realistic.

Version 1 was therefore selected as the stronger video artifact.

## Detection Experiment

The final ElevenLabs Version 1 artifact was tested using AI Voice Detector.

Result:

- AI Score: 16%
- Verdict: Likely Human
- Maximum segment AI score: 50%
- Known ground truth: Completely AI-generated

The detector therefore produced a false-negative result.

This demonstrates why automated detection should not be treated as definitive
evidence of authenticity.

## Key Finding

Across both generation approaches, adding more pauses did not automatically
increase realism.

The experiment suggests that natural synthetic-media presentation depends on
the interaction between pacing, pause duration, emotional expression,
facial behavior, breathing patterns, and synchronization.

The detection experiment further demonstrated that realistic synthetic media
may not always be correctly identified by automated detection systems.

## Repository Contents

- `SCRIPT.md` – Source narrative and scripts
- `PROCESS_LOG.md` – Generation tools, settings, iterations, and observations
- `EVALUATION.md` – Critical comparison of the synthetic artifacts
- `DETECTION_REPORT.md` – Detection and provenance analysis
- `artifacts/` – Synthetic audio and video files
- `evidence/` – Screenshots from generation and detection

## Ethics and Disclosure

All artifacts were created for educational research.

Stock/synthetic voices and avatars were used rather than cloning a real
person's identity.

The project demonstrates the importance of disclosure, provenance, human
verification, and responsible synthetic-media use.
