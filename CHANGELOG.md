# Changelog

## 1.3.0

- Add buffered speech synthesis with MP3 and PCM encoding and a distinct speech host. The transcription adapter recognizes assemblyai-stt-3-7, sends speech_models and reports migration warnings for older IDs. Reviewed npm: @ai-sdk/assemblyai 3.0.82 to 3.0.85. Offline validation passed: node Scripts/test-packages.mjs (56 packages, 3672 owning tests and 1760 compatibility tests), generation, tooling, isolation, and version selection. Speech is buffered. Existing native STT GET-query and schema differences are recorded in the audit. See Docs/Archive/WeeklyUpstreamAudit20261122.md for retained gaps. Paid provider calls were skipped.
  Compatibility: Additive speech API and settings. The transcription adapter places every supplied model ID in the speech_models array.
