# Task 06 — Synthetic Media Process Log

## Project Objective

The objective of this experiment was to transform a data-driven research narrative into synthetic media using accessible AI tools.

Two different approaches were evaluated:

1. Synthetic audio using ElevenLabs
2. Synthetic avatar video using Vidnoz AI

Each approach included two iterations.

The experiment focused on realism, pacing, pauses, emotional expression, synchronization, disclosure, and detectability.

---

# Ground Truth

Before creating synthetic media, the statistical claims used in the scripts were validated against three datasets.

| Dataset | Records |
|---|---:|
| Facebook Ads | 246,745 |
| Facebook Posts | 19,009 |
| Twitter/X Posts | 27,304 |
| **Combined** | **293,058** |

Additional verified statistics included:

| Metric | Value |
|---|---:|
| Estimated Facebook ad spending | $261,868,355 |
| Estimated Facebook ad impressions | 11,251,948,521 |
| Facebook median interactions* | 133 |
| Facebook mean interactions* | ~2,210 |
| Twitter/X median likes | 1,406 |
| Twitter/X mean likes | ~6,914 |

\*Calculated using Facebook records where Total Interactions could be interpreted numerically.

The purpose of validating these numbers before generating synthetic media was to separate the realism of the presentation from the accuracy of the underlying information.

---

# Approach 1 — ElevenLabs Synthetic Audio

## Tool

**Tool:** ElevenLabs  
**Account:** Free tier  
**Voice:** Siren — Natural Realistic Conversational Voice  
**Artifact:** AI-generated synthetic narration

No real person's voice was cloned.

---

# ElevenLabs Iteration 1

The first version used the original research script and served as the baseline.

**Duration:** Approximately 1 minute 58 seconds

## Human Evaluation

| Characteristic | Rating |
|---|---:|
| Voice naturalness | 95% |
| Numerical pronunciation | 100% |
| Pacing | 100% |
| Pauses between ideas | 80% |
| Emotional variation | 90% |

## What Worked

The generated voice sounded highly natural and conversational.

The pronunciation of numerical statistics was particularly successful. This was important because the script included large values involving dataset sizes, estimated spending, impressions, and engagement statistics.

The pacing also worked well for an academic presentation.

## Main Problem

The most noticeable synthetic characteristic was the lack of natural breathing.

Although individual sentences sounded convincing, there were fewer substantial pauses between some sentences and ideas than would normally occur in human speech.

The voice sometimes appeared capable of speaking continuously without needing to breathe.

## Objective Pause Observation

The audio contained approximately 30 detectable pauses of at least 0.25 seconds.

Only approximately four pauses were 0.75 seconds or longer.

No detected pause reached one full second.

The median detectable pause was approximately 0.56 seconds.

This supported the human observation that the speech was convincing within sentences but less natural during transitions.

---

# ElevenLabs Iteration 2

For Version 2, the script formatting was changed to create stronger separation between ideas.

The same general voice configuration was retained so that pause behavior could be examined without introducing an entirely different voice.

**Duration:** Approximately 1 minute 56 seconds

## Human Evaluation

| Characteristic | Rating |
|---|---:|
| Voice naturalness | 98% |
| Numerical pronunciation | 100% |
| Pacing | 90% |
| Pauses between ideas | 90% |
| Emotional variation | 95% |

## Observation

Some characteristics received higher individual ratings, particularly naturalness and emotional variation.

However, Version 2 sounded faster overall and made the synthetic nature of the voice more noticeable.

Approximately 33 pauses of at least 0.25 seconds were detected, but only approximately two pauses were 0.75 seconds or longer.

This meant Version 2 contained more small pauses but fewer substantial pauses.

## Result

The experiment demonstrated that increasing the number of pauses did not automatically make the speech more human.

Pause placement and duration appeared to matter more than the total number of pauses.

---

# ElevenLabs Final Selection

**Version 1 was selected as the stronger final audio artifact.**

Although Version 2 received slightly higher ratings for some individual characteristics, Version 1 had better perceived pacing and sounded less noticeably synthetic overall.

This was an important experimental result because the second iteration did not automatically outperform the first.

---

# Approach 2 — Vidnoz Synthetic Avatar Video

## Tool

**Tool:** Vidnoz AI  
**Account:** Free tier  
**Avatar:** Annie  
**Voice:** Annie (Lifelike)  
**Artifact:** AI-generated synthetic avatar video

A stock synthetic avatar was used.

No real person's face or voice was cloned.

---

# Vidnoz Iteration 1

**Duration:** Approximately 46.1 seconds

Version 1 used the original shortened video script.

## Human Evaluation

| Characteristic | Rating |
|---|---:|
| Visual realism | 80% |
| Lip synchronization | 90% |
| Facial expressions | 50% |
| Body/head movement | 90% |
| Voice naturalness | 80% |
| Pacing | 70% |
| Emotional variation | 60% |
| Overall realism | 80% |

## Strengths

Lip synchronization was one of the strongest aspects of the artifact.

Body and head movement were also convincing.

These characteristics helped create the appearance of a presenter speaking directly to the viewer.

## Weaknesses

The avatar was still recognizably AI-generated.

Facial expressions were significantly less convincing than lip synchronization or body movement.

The voice also lacked natural emotional variation and sounded robotic in some sections.

## Main Problem

The main weakness was the mismatch between technically strong synchronization and less natural emotional presentation.

The mouth and body could move convincingly while the facial expression and vocal emotion still revealed the artificial nature of the presenter.

---

# Vidnoz Iteration 2

**Duration:** Approximately 51.4 seconds

Version 2 used shorter sentences and stronger separation between ideas.

The purpose was to determine whether additional pauses would improve pacing and make the synthetic presenter appear more natural.

## Observation

Version 2 appeared **less realistic than Version 1**.

The shorter sentence structure created longer and more noticeable pauses.

Instead of creating natural breathing behavior, the pauses interrupted the rhythm of the presentation.

The pacing therefore made the synthetic nature of the avatar more noticeable.

Exact numerical ratings were not assigned to Version 2 because the comparison was primarily qualitative.

---

# Vidnoz Final Selection

**Version 1 was selected as the stronger final video artifact.**

Its pacing was more continuous and realistic.

Version 2 demonstrated that mechanically adding additional pauses can reduce realism when the pauses become predictable or unnaturally long.

---

# Cross-Approach Finding

A similar result appeared independently in both generation approaches.

For ElevenLabs, modifying the pause structure did not clearly improve realism.

For Vidnoz, shorter sentences and stronger pauses actually reduced perceived realism.

This suggests that human-like speech cannot be reproduced simply by increasing the number of pauses.

Natural speech involves a combination of:

- breathing
- rhythm
- sentence length
- emphasis
- hesitation
- emotional variation
- pause duration
- pause placement

Synthetic systems may reproduce some of these characteristics successfully while still failing to reproduce their natural interaction.

---

# Detection Experiment

After completing the audio experiment, ElevenLabs Version 1 was tested using AI Voice Detector.

**Known ground truth:** Completely AI-generated

The detector returned:

- AI Score: 16%
- Verdict: Likely Human
- Segments analyzed: 19
- Maximum segment AI score: 50%

Only one segment was classified as "Likely AI."

This result represented a false negative because the recording was known to have been generated entirely using ElevenLabs.

The detection result became one of the most significant findings of the project.

---

# Time and Resource Constraints

The experiment used free-tier tools.

Free-tier generation limits affected the design of the video experiment.

The Vidnoz script was shortened so that it could be generated within the available free credits.

Rather than treating this only as a limitation, it became part of the practical experience of working with accessible synthetic-media tools.

---

# Ethical Safeguards

Throughout the experiment:

- no real person's voice was cloned
- no real person's face was reproduced
- stock/synthetic identities were used
- the artifacts explicitly disclosed their synthetic nature
- the statistics were verified before generation
- artifacts were created for academic research
- generation iterations were documented

---

# Final Outcome

The experiment successfully produced and evaluated four synthetic-media artifacts:

1. ElevenLabs Version 1
2. ElevenLabs Version 2
3. Vidnoz Version 1
4. Vidnoz Version 2

The experiment demonstrated that later iterations are not automatically better and that synthetic-media realism depends on the interaction of multiple characteristics rather than any single technical feature.
