# Feature wishlist

Ideas under consideration for MyVoiceBook. Numbers are for reference only—not a priority ranking.

## Speech models

1. **More built-in sherpa-onnx models** from the [pretrained model catalog](https://k2-fsa.github.io/sherpa/onnx/pretrained_models/index.html), for example:
   - [SenseVoice](https://k2-fsa.github.io/sherpa/onnx/sense-voice/index.html) — Chinese, English, Japanese, Korean, Cantonese
   - [Paraformer](https://k2-fsa.github.io/sherpa/onnx/pretrained_models/offline-paraformer/paraformer-models.html) — Chinese / bilingual zh-en
   - **Whisper medium** and English-only Whisper variants
   - More **streaming Zipformer** languages (Chinese, Korean, Vietnamese, Bengali, …)
   - Offline Zipformer CTC variants
2. **Romanian language support** — first-class UI for Romanian, plus on-device models tuned for Romanian dictation (likely via multilingual Whisper or a dedicated sherpa-onnx release).
3. **Import custom model packs** — add arbitrary sherpa-onnx bundles by URL with SHA-256 verification, beyond the built-in registry.

## Dictation

4. **Smart punctuation integrated into Zipformer** — fold punctuation and capitalization into the Zipformer pipeline so output reads naturally without a separate punctuation add-on download.
5. Per-app IME defaults (e.g. always confirm in password fields).
6. Better punctuation for Whisper offline models without a separate add-on.
7. Adjustable free-tier limits for sponsors / trial modes.

## Notes

8. **Improved notes UI**, including:
   - Sort notes by date updated, date created, or title
   - Pinned / favorite notes at the top of the list
   - Clearer note previews and timestamps in the list
   - Quick actions (rename, duplicate, move to archive)
   - Tablet and foldable layouts with a list + editor side-by-side
9. **Search notes** — full-text search across note titles and bodies, with recent searches and highlighted matches.
10. **Backup notes**
    - **Export** — manual backup to a single file (JSON or Markdown bundle) you can save or share.
    - **Automated backup** — scheduled local backups on device and optional cloud backup (e.g. Google Drive or user-chosen storage), with restore from a previous backup. Speech stays on-device; only note text is backed up.

## Platform

11. Wear OS quick-capture companion (local-only).
12. Home-screen widget for one-tap dictation into a new note.

## Pro & distribution

13. Family sharing / license restore improvements via Play.
14. Open-source release of app code (when ready).

---

Have an idea? [Open a discussion](https://github.com/pcraciunoiu/myvoicebook-site/discussions) on the site repo.
