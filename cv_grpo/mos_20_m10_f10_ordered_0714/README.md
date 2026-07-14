# MOS package for CV GRPO

Subset: 20 cases selected from the constrained 300-case pool, with 10 male and 10 female cases.

Aggregate ablation speech-score ordering is enforced on the selected 20 cases:
`grpo_face_style > face_style > face_style_0_5 > onlystyle > onlyface`.

Directories:
- `face/`: one face image per case.
- `style/`: style prompt, content prompt, and instruction per case.
- `speech/<method_id>/`: wav files for GT, our method, ablations, and baselines.

Manifest files:
- `cases_manifest.csv`: case-level face/style metadata.
- `speech_manifest.csv`: one row per case and method wav.
- `methods.csv`: method IDs and descriptions.
- `selection_scores.csv`: objective selection scores used for ablation ordering.
