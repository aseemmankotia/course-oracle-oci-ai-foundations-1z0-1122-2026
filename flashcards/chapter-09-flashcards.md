## Chapter 9: OCI AI Services Part 1: Language, Speech & Vision — Flashcards

| # | Front (Question) | Back (Answer) |
|---|-----------------|---------------|
| 1 | OCI Language: which feature detects positive/negative sentiment toward specific aspects within a sentence? | Aspect-Based Sentiment Analysis (ABSA). Exam tip: distinct from overall sentence-level sentiment analysis, which scores the whole sentence instead of individual aspects. |
| 2 | OCI Speech primary function | Converts spoken audio into text (transcription), returning word-level timestamps, confidence scores, and punctuation via batch transcription jobs. |
| 3 | OCI Vision Document AI extracts what from scanned forms? | Text (OCR), tables, and key-value pairs, plus document type classification. Exam tip: structures data, unlike plain OCR-only extraction. |
| 4 | OCI Language Translation language coverage | Supports translation across 100+ languages using pretrained models. Exam tip: no custom training required for translation tasks. |
| 5 | Which OCI AI service to use: transcribing a customer support call recording? | OCI Speech — OCI Language operates on text input, not raw audio. |
| 6 | Which OCI AI service to use: detecting objects with bounding boxes in an image? | OCI Vision — specifically the Object Detection feature. |
| 7 | OCI Language PII Detection purpose | Identifies (and can mask) personal data such as names, SSNs, and emails in text. Exam tip: commonly tested in data privacy/compliance scenarios. |
| 8 | Key Phrase Extraction vs Named Entity Recognition (OCI Language) | Key Phrase Extraction pulls out important noun phrases/topics; NER identifies specific typed entities (person, org, location, date). Exam tip: don't confuse the two. |
| 9 | OCI Vision: Image Classification vs Object Detection | Image Classification labels the WHOLE image with one category; Object Detection locates MULTIPLE objects with bounding boxes within the image. |
| 10 | Ways to consume OCI AI Services | OCI Console (no-code testing), REST API (direct HTTP calls), SDKs (Python, Java, etc.), and CLI. Exam tip: know all four exist at an awareness level. |
| 11 | OCI Language: pretrained vs custom models | Pretrained models work immediately for general use cases; custom models require labeled training data (via OCI Data Labeling) for domain-specific classification/NER/sentiment. |
| 12 | OCI Speech supported use cases | Call center analytics, closed captioning/subtitles (SRT output), accessibility voice-to-text, meeting transcription. Exam tip: Speech does NOT do sentiment analysis — pass its text output to OCI Language for that. |
