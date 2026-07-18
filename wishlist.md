# Feature wishlist

Ideas under consideration for MyVoiceBook. Numbers are for reference only—not a priority ranking.

## Speech models

1. **More built-in sherpa-onnx models** from the [pretrained model catalog](https://k2-fsa.github.io/sherpa/onnx/pretrained_models/index.html), for example:
   - [SenseVoice](https://k2-fsa.github.io/sherpa/onnx/sense-voice/index.html) — Chinese, English, Japanese, Korean, Cantonese
   - [Paraformer](https://k2-fsa.github.io/sherpa/onnx/pretrained_models/offline-paraformer/paraformer-models.html) — Chinese / bilingual zh-en
   - **Whisper medium** and English-only Whisper variants
   - More **streaming Zipformer** languages (Chinese, Korean, Vietnamese, Bengali, …)
   - Offline Zipformer CTC variants
   - **Parakeet 110M English** — evaluate as a lighter English option alongside the current Parakeet TDT models
2. **Import custom model packs** — add arbitrary sherpa-onnx bundles by URL with SHA-256 verification, beyond the built-in registry.

## Dictation

3. **Smart punctuation integrated into Zipformer** — fold punctuation and capitalization into the Zipformer pipeline so output reads naturally without a separate punctuation add-on download.
4. **Voice undo keywords** — say a phrase such as “scratch that” during hands-free dictation to undo the last committed segment (without tapping Undo).
5. Per-app IME defaults (e.g. always confirm in password fields).
6. Better punctuation for Whisper offline models without a separate add-on.
7. Adjustable free-tier limits for sponsors / trial modes.
8. **Field-aware dictation expansion** — build on numeric-field dictation (`NumericDictation` / `FieldContext`):
   - Spoken numbers beyond English (locale-aware word → digit)
   - Email / URL / password-aware modes (constrain characters, avoid mid-sentence casing and paragraph rules)
   - Richer phone formatting when the host field is `TYPE_CLASS_PHONE`
9. **Post-dictation correction chips + custom vocabulary** — after a committed segment, offer “did you mean?” suggestions backed by a user vocabulary / common corrections list.

## Notes

10. **Improved notes UI**, including:
    - Sort notes by date updated, date created, or title
    - Pinned / favorite notes at the top of the list
    - Quick actions (rename, duplicate, move to archive)
    - Tablet and foldable layouts with a list + editor side-by-side
    - ~~Clearer note previews and timestamps in the list~~ *(timestamps shipped on Android and desktop)*
11. **Search notes** — full-text search across note titles and bodies, with recent searches and highlighted matches.
12. **Backup notes**
    - **Export / import** — manual SQLite database backup and restore.
    - **Automated local backup** — scheduled copies into a user-chosen folder (via the system file picker; includes Drive and other providers).
13. **Desktop app + notes sync** — Linux desktop client with local-folder and Google Drive sync is shipping; speech recognition stays on-device, only note text syncs.
    - **Windows + macOS:** ship unsigned builds first (on macOS, Gatekeeper shows a warning; the app is still installable via right-click → Open).
    - **Wishlist later:** signed + notarized macOS DMG (Apple Developer Program).
14. **Hardened multi-device sync** — seamless recovery when phone and desktop edit at the same time, and safer first join when one side already has notes.

---

Have an idea? [Open a discussion](https://github.com/pcraciunoiu/myvoicebook-site/discussions) on the site repo.
