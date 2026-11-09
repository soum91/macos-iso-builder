# Claude development instructions

Read and follow [AGENTS.md](AGENTS.md) before changing source, release workflows, or publishing releases. Every GitHub Release must have factual, specific, evidence-linked notes and a matching CHANGELOG.md entry. Do not replace actual changes with generic text or claim unverified fixes.


## Diagnostic/reporting rule for Claude

Before implementing or changing any diagnostics or logs, follow the **Universal diagnostic copy and export contract** in `AGENTS.md`: verified Copy with visible feedback, native Share, native plain-text Files export, and complete selectable report. Avoid claiming these work until a signed-device paste and export check is complete.


## Universal diagnostic export contract

Every generated diagnostic/log report must offer verified Copy (clipboard read-back where supported, with visible success or failure), native Share, native Save as plain-text `.txt` via the platform file picker (`fileExporter` or `UIDocumentPickerViewController` on iOS), and selectable complete report text as fallback. Never rely on a silent clipboard-only button. Include app/build, device/OS, actionable error/return codes; redact secrets. Test cross-app paste, Share and Save to Files on a signed physical device before claiming working; otherwise mark unverified. Preserve existing release and assistant instructions.
