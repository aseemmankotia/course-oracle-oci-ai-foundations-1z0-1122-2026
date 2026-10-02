## Chapter 9 Cheat Sheet: OCI Language, Speech & Vision

### Service-to-Task Matching
| Business Need | Correct Service | Feature |
|---|---|---|
| Analyze text sentiment/entities/topics | OCI Language | Sentiment, NER, Key Phrase, Classification |
| Translate text between languages | OCI Language | Translation (100+ languages, pretrained) |
| Detect/redact sensitive data in text | OCI Language | PII Detection |
| Convert audio to text | OCI Speech | Speech-to-Text Transcription |
| Classify a whole image | OCI Vision | Image Classification |
| Locate multiple objects in an image | OCI Vision | Object Detection |
| Extract text/tables/key-values from scanned docs | OCI Vision | Document AI |

### OCI Language Capabilities
- **Language Detection** — identifies the language of input text.
- **Sentiment Analysis** — sentence-level AND aspect-based (per-feature) sentiment.
- **Key Phrase Extraction** — surfaces important topics/phrases (no entity types).
- **Named Entity Recognition (NER)** — extracts typed entities: person, org, location, date, etc.
- **Text Classification** — assigns document-level category labels.
- **PII Detection** — finds/masks names, SSNs, emails, phone numbers.
- **Punctuation & Text Normalization** — cleans raw/ASR text.
- **Translation** — pretrained, 100+ languages, no custom training needed.
- **Pretrained vs Custom** — pretrained = ready out-of-box; custom = requires labeled data via OCI Data Labeling for domain-specific tuning.

### OCI Vision Capabilities
- **Image Classification** — one label for the entire image (e.g., 'dog').
- **Object Detection** — multiple objects located with bounding boxes + labels.
- **Document AI** — OCR text extraction, table extraction, key-value pair extraction, document type classification (e.g., invoices, receipts, IDs).
- Supports both pretrained and custom-trainable models for classification/detection.

### OCI Speech Capabilities
- **Speech-to-Text Transcription** — batch transcription of audio files.
- Output includes: transcribed text, word-level timestamps, confidence scores, punctuation.
- Supported output formats: plain text, SRT (subtitles), JSON.
- Common use cases: call center analytics, captioning/subtitles, accessibility, meeting notes.
- Does NOT perform sentiment/entity analysis — chain output into OCI Language for that.

### Consumption Methods (awareness level)
| Method | Best For |
|---|---|
| OCI Console | Manual testing, no-code exploration |
| REST API | Direct HTTP integration, custom auth handling |
| SDK (Python, Java, etc.) | Application integration, less boilerplate |
| CLI | Scripting and admin automation |

### Exam Gotchas
- Don't confuse **Key Phrase Extraction** (no types) with **NER** (typed entities).
- **Aspect-based sentiment** ≠ overall sentence sentiment — exam distinguishes both.
- **OCI Speech** ≠ OCI Language: Speech only transcribes; it has no built-in sentiment/entity features.
- **Document AI** is part of OCI Vision, not OCI Language, even though it deals with 'documents.'
- Custom models require labeled data; pretrained models do not.
