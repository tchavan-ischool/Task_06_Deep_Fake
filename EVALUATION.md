# Task 06 — Critical Evaluation of Synthetic Media

## Overview

This project evaluated two forms of synthetic media:

1. AI-generated audio using ElevenLabs
2. AI-generated avatar video using Vidnoz AI

Each approach was generated twice so that changes in pacing and pause structure could be evaluated.

The purpose was not simply to create convincing synthetic media.

The experiment examined what aspects of synthetic representation appear realistic, what aspects fail, and what characteristics may reveal that an artifact is AI-generated.

---

# 1. ElevenLabs Evaluation

## Version Comparison

|        Criterion        | V1   | V2   |
|-------------------------|-----:|-----:|
| Voice naturalness       | 95%  | 98%  |
| Numerical pronunciation | 100% | 100% |
| Pacing                  | 100% | 90%  |
| Pauses                  | 80%  | 90%  |
| Emotional variation     | 90%  | 95%  |

Version 1 was approximately 1 minute 58 seconds.

Version 2 was approximately 1 minute 56 seconds.

---

## What Held Up Well?

The strongest aspect of the ElevenLabs output was pronunciation.

Large numerical values were pronounced correctly and clearly.

The voice was also highly natural and conversational.

Version 1 in particular maintained strong pacing throughout the presentation.

---

## What Failed?

The primary weakness was breathing behavior.

The voice did not appear to require breaths in the same way a human narrator would.

Some transitions between sentences occurred too quickly.

Version 2 attempted to improve this through stronger pause formatting.

However, the modification did not clearly improve the artifact.

Although more small pauses appeared, Version 2 sounded faster and more noticeably synthetic overall.

---

## Could It Fool a Listener?

The audio was sufficiently realistic that an automated detector later classified it as "Likely Human."

As a human listener who knew the artifact was synthetic, I could still identify subtle clues such as breathing behavior and speech rhythm.

However, these clues were significantly less obvious than stereotypical robotic text-to-speech characteristics.

---

# 2. Vidnoz Evaluation

## Version 1

|      Criterion      |  V1 |
|---------------------|----:|
| Visual realism      | 80% |
| Lip synchronization | 90% |
| Facial expressions  | 50% |
| Body/head movement  | 90% |
| Voice naturalness   | 80% |
| Pacing              | 70% |
| Emotional variation | 60% |
| Overall realism     | 80% |

Version 1 was approximately 46.1 seconds.

---

## What Held Up Well?

Lip synchronization was highly convincing.

Body and head movement were also relatively realistic.

These characteristics helped create a recognizable human-presenter format.

---

## What Failed?

Facial expression was the weakest visual characteristic.

Although the mouth synchronized well with the narration, the rest of the face did not display the same degree of natural emotional behavior.

The synthetic voice also sounded robotic in emotional delivery.

This created a mismatch between accurate mechanical synchronization and limited emotional realism.

---

# Vidnoz Version 2

Version 2 was approximately 51.4 seconds.

The script was divided into shorter sentences to create stronger pauses between ideas.

However, Version 2 appeared less realistic.

The longer pauses interrupted the presentation's rhythm and made the AI-generated nature of the presenter more noticeable.

This demonstrated that adding pauses is not automatically equivalent to reproducing natural human breathing.

---

# 3. Audio vs. Video

The two approaches revealed different synthetic characteristics.

## ElevenLabs

The audio artifact was strongest in:

- voice naturalness
- pronunciation
- pacing
- emotional variation

Its primary weakness involved breathing and rhythm.

## Vidnoz

The avatar video was strongest in:

- lip synchronization
- body movement
- head movement

Its primary weaknesses involved:

- facial expression
- vocal emotion
- pacing
- visibly synthetic appearance

---

# 4. Unexpected Finding

Before conducting the experiment, I expected that adding more pauses would make synthetic speech sound more human.

The results did not consistently support that expectation.

In ElevenLabs Version 2, additional pause formatting produced more short pauses but did not improve overall perceived pacing.

In Vidnoz Version 2, stronger sentence separation created longer pauses that made the avatar less realistic.

This suggests that the realism of synthetic speech depends on the **quality and placement of pauses**, not simply their quantity.

---

# 5. Detection Evaluation

ElevenLabs Version 1 was tested using AI Voice Detector.

The recording was known to be completely synthetic.

However, the detector returned:

**AI Score:** 16%

**Verdict:** Likely Human

**Average AI Score:** 16%

**Maximum AI Score:** 50%

**Segments analyzed:** 19

Only one segment was classified as "Likely AI."

This represented a false-negative result.

---

# 6. Human vs. Automated Evaluation

The detector result was especially interesting when compared with the human evaluation.

I rated the ElevenLabs voice naturalness at 95%.

The detector then classified the artifact as likely human.

However, because I knew how the recording was generated, I could identify subtle characteristics such as unnatural breathing and transitions.

This demonstrates that humans and automated systems may rely on different signals when evaluating synthetic media.

Neither should automatically be treated as infallible.

---

# 7. Detection vs. Provenance

The project revealed an important distinction between detection and provenance.

**Detection** attempts to infer whether an artifact is synthetic.

**Provenance** documents how an artifact was created.

The detector incorrectly inferred that the ElevenLabs recording was likely human.

The provenance record, however, clearly establishes that the artifact was synthetic.

The repository contains:

- the original script
- the generation tool
- selected voice
- generation iterations
- output files
- screenshots
- human evaluation
- detector result

Therefore, provenance provides stronger evidence of origin in this experiment than automated detection.

---

# 8. Ethical Evaluation

The experiment demonstrates why synthetic-media ethics cannot depend entirely on whether a person can detect AI generation.

A highly realistic artifact can still be synthetic.

Similarly, an artifact can communicate accurate information while using an artificial presenter.

Responsible synthetic-media use therefore requires attention to:

- truth
- disclosure
- consent
- provenance
- context
- verification

The project avoided cloning a real person's voice or identity.

All artifacts were created using synthetic or stock identities.

---

# 9. Overall Finding

The strongest overall finding from this experiment is:

> **Synthetic-media realism depends on the interaction between timing, rhythm, emotional expression, breathing behavior, synchronization, and visual behavior. Improving one characteristic does not necessarily improve the entire artifact.**

The experiment also demonstrated:

> **Realistic presentation is not evidence of authenticity, and automated detection is not proof of origin.**

---

# Conclusion

Synthetic-media systems can now produce highly convincing audio and reasonably realistic human-like video using accessible tools.

However, subtle characteristics still reveal limitations.

More importantly, the detector experiment demonstrated that synthetic media may sometimes be sufficiently realistic to be classified as human by automated systems.

For this reason, responsible synthetic-media use should emphasize transparent disclosure, provenance, factual verification, and human judgment rather than relying exclusively on automated detection.

