# Mansi Agarwal

Clinical psychology researcher applying for PhD positions in quantitative and methods-focused psychology. My work is about measuring psychological change accurately, and about checking that an analysis method can be trusted before it is used on real participants.

**Current role:** Project Research Scientist-I, King George's Medical University (KGMU), Lucknow. I work on a multi-centre randomised controlled trial of psychosocial interventions for common psychological problems.

**Previous role:** Project Research Scientist-I, NIMHANS, Bengaluru. I set up trials and managed data for digital mental health research: REDCap builds, randomisation and multi-site participant onboarding.

**Education:** M.Sc. Clinical Psychology, Kristu Jayanti College, Bengaluru

## Research interests

- Measuring how a person's skill or psychological state changes over time
- Personalized algorithmic environments: whether systems that adapt to a person's responses still let researchers estimate what works
- Validity and reliability of psychological measures
- Using simulation to test a method before collecting data

## Projects

### [adaptive-assignment-recovery](https://github.com/MansiAgrwal/adaptive-assignment-recovery)

Personalized digital environments, such as adaptive learning platforms, recommender systems and digital health apps, choose what each person encounters next from their earlier responses. Can researchers still tell which experiences actually change people? This repository tests that question by simulating a personalized environment with a controlled rule-learning task.

What I found so far, in one simulated scenario: the choice of analysis model mattered more than whether the algorithm personalized. A model that ignored differences between fast and slow learners got the direction of the effect wrong. A model that allowed for those differences recovered the true effect, including under personalization. The next version will test whether this holds under more realistic conditions.

### [selective-history-lab](https://github.com/MansiAgrwal/selective-history-lab)

A simulation pilot for a study of personalized learning. Simulated learners practise two skills while a personalization algorithm chooses each activity from a limited retained history of their responses, and a hidden Markov model fitted by maximum likelihood tries to recover how much each activity teaches. The repository also audits two public learning datasets. A rerun then asked whether each hypothesis gives the study something real to detect. Ignoring persistent differences between learners shrank the estimated effects toward zero, by 17–93% depending on how much learners differed. The retained-history rule barely changed what learners practised in a three-activity task, and a second measurement channel helped only when it was recorded on every practice trial.

### [recognition-memory-decoding](https://github.com/MansiAgrwal/recognition-memory-decoding)

A re-analysis of public single-neuron recordings from the human medial temporal lobe (58 patients). When a person misjudges whether they have seen an image before, does neural activity follow the image's true status or the person's judgment? Neither question produced a positive result. The checks along the way found that the dataset's truth label is documented backwards, that eight files are missing learning trials, and that image category can push both decoding tests away from chance without any memory signal. Each test is therefore compared with a within-category null, and simulations show why it is needed.

### [eeg-motor-imagery-decoding](https://github.com/MansiAgrwal/eeg-motor-imagery-decoding)

Can scalp EEG tell imagined left-hand from right-hand movement in a person the decoder has never seen? The notebook uses public PhysioNet recordings from 20 people, with the analysis plan fixed before it was run. The pre-specified test was not significant: a standard CSP decoder averaged 55% balanced accuracy (p = .10). Re-centring each person's EEG covariances before decoding raised this to 64%. The README explains why that figure is still optimistic, and why the side of the screen where the cue appears could account for part of what any of these decoders detect.

### [prepost-mixed-anova](https://github.com/MansiAgrwal/prepost-mixed-anova)

A Colab notebook for one of the most common designs in intervention research: two or more groups measured before and after. It reads an SPSS file and produces a mixed ANOVA with assumption checks, follow-up tests and effect sizes, saved as Excel and Word reports. A validation script checks its results against independent calculations, and the commit history documents the corrections made after review.

### [literature-evidence-pipeline](https://github.com/MansiAgrwal/literature-evidence-pipeline)

Notebooks for mapping a broad literature in a way that can be checked afterwards. The main search ran 153 pre-specified queries across 40 domains in OpenAlex and PubMed. Every paper is traced back to the query that found it, duplicates are merged only on exact matches, and screening queues are stratified so that counterevidence is not crowded out by highly cited papers.

### [personalized-feedback-reports](https://github.com/MansiAgrwal/personalized-feedback-reports)

Personalization in practice. I automated a digital mental-health study's hand-written feedback reports: the code turns each participant's questionnaire answers (K10 distress, coping strategies, and barriers to seeking help) into an individual Word report. The main work was finding the hard cases within the existing report structure before the logic was carried into a larger system for automating intervention delivery. The repository runs on synthetic data.

## Tools

R (lavaan; still developing) · Python (pandas, NumPy, SciPy, scikit-learn, MNE, PyNWB, python-docx) · OpenAlex and PubMed APIs · SPSS/AMOS · REDCap

---

All code here runs on simulated data, published literature records or public de-identified datasets. No participant data from any study I have worked on is included.
