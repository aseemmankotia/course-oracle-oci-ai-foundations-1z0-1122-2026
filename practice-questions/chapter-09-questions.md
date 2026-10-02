## Chapter 9: OCI AI Services Part 1: Language, Speech & Vision — Practice Questions

**Q1.** A company wants to determine whether customers feel positively or negatively about specific product features mentioned within the same review (e.g., 'battery' vs 'camera'). Which OCI Language capability BEST supports this?

A) Aspect-Based Sentiment Analysis
B) Text Classification
C) Key Phrase Extraction
D) Named Entity Recognition

<details>
<summary>Answer</summary>

**Correct: A**

Aspect-Based Sentiment Analysis (ABSA) identifies sentiment tied to individual aspects/entities mentioned in the same text, unlike sentence-level sentiment.

**Why the others are wrong:**
- Text Classification assigns a category label to the whole document, not sentiment per aspect.
- Key Phrase Extraction only pulls important terms, it returns no sentiment.
- Named Entity Recognition identifies entities like people/orgs but does not score sentiment.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** Which OCI AI service should a call center use to convert recorded customer calls into searchable text transcripts?

A) OCI Language
B) OCI Speech
C) OCI Vision
D) OCI Anomaly Detection

<details>
<summary>Answer</summary>

**Correct: B**

OCI Speech performs speech-to-text transcription of audio recordings, which is exactly the requirement.

**Why the others are wrong:**
- OCI Language processes text input, not raw audio.
- OCI Vision processes images/documents, not audio.
- OCI Anomaly Detection finds outliers in numeric time-series data, unrelated to audio transcription.

</details>

---

**Q3.** An insurance company receives scanned claim forms and needs to automatically extract field labels and their corresponding values (e.g., 'Policy Number: 12345'). Which OCI AI service feature addresses this?

A) OCI Language Key Phrase Extraction
B) OCI Vision Document AI key-value extraction
C) OCI Speech transcription
D) OCI Vision image classification

<details>
<summary>Answer</summary>

**Correct: B**

OCI Vision's Document AI capability extracts structured key-value pairs, tables, and text from scanned document images.

**Why the others are wrong:**
- Key Phrase Extraction works on plain text, not scanned images, and doesn't pair labels with values.
- Speech transcription converts audio to text, unrelated to scanned forms.
- Image classification only assigns a single category label to the whole image, not field-level data.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** When OCI Speech transcribes an audio file, which output elements are included alongside the transcribed text?

A) Only the plain text transcript
B) Sentiment score for each sentence
C) Named entities detected in the audio
D) Word-level timestamps and confidence scores

<details>
<summary>Answer</summary>

**Correct: D**

OCI Speech output includes word-level timestamps, confidence scores, and punctuation, supporting formats like SRT/JSON in addition to plain text.

**Why the others are wrong:**
- Plain text alone omits timing/confidence data actually provided.
- Sentiment scoring is an OCI Language feature, not part of Speech output.
- Entity detection is an OCI Language feature; Speech does not perform NER.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q5.** A healthcare company wants to automatically detect personally identifiable information (PII) such as names and SSNs in text documents before storage. Which OCI Language feature should they use?

A) Text Classification
B) Key Phrase Extraction
C) PII Detection
D) Language Detection

<details>
<summary>Answer</summary>

**Correct: C**

PII Detection specifically identifies and can mask sensitive personal data types like names, SSNs, and emails within text.

**Why the others are wrong:**
- Text Classification labels documents by topic/category, not PII.
- Key Phrase Extraction highlights important terms, not sensitive data specifically.
- Language Detection only identifies which language the text is written in.

</details>

---

**Q6.** A retail company wants to automatically detect and count individual products with bounding boxes in shelf photos. Which OCI Vision capability is appropriate?

A) Image Classification
B) Document Classification
C) Object Detection
D) Text Extraction (OCR)

<details>
<summary>Answer</summary>

**Correct: C**

Object Detection locates and draws bounding boxes around multiple individual objects within a single image, enabling counting of each product.

**Why the others are wrong:**
- Image Classification assigns one label to the entire image, it cannot count or locate multiple items.
- Document Classification categorizes document type, unrelated to shelf photos.
- Text Extraction (OCR) reads text characters, not product objects.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** What is the key difference between OCI Language pretrained models and custom models?

A) Pretrained models require labeled training data; custom models do not
B) Pretrained models only support English; custom models support all languages
C) Custom models are trained on customer-specific labeled data via OCI Data Labeling, while pretrained models work out-of-the-box for general use cases
D) Custom models cannot be used for text classification

<details>
<summary>Answer</summary>

**Correct: C**

Custom models require the customer to supply labeled data (typically via OCI Data Labeling) to fine-tune for domain-specific needs, whereas pretrained models are ready to use immediately for general scenarios.

**Why the others are wrong:**
- This reverses the actual requirement — pretrained models need no extra training data.
- Language support is not the distinguishing factor between pretrained and custom models.
- Custom models are supported for text classification, among other tasks.

</details>

---

**Q8.** A developer wants to integrate OCI Vision object detection into an existing Python application with minimal boilerplate. Which consumption method is MOST appropriate?

A) OCI Console only
B) OCI SDK
C) Manually crafted REST calls with no authentication
D) OCI CLI only

<details>
<summary>Answer</summary>

**Correct: B**

The OCI SDK provides language-specific libraries (e.g., Python) that handle authentication and API calls, minimizing boilerplate for application integration.

**Why the others are wrong:**
- The Console is for manual testing/exploration, not programmatic app integration.
- REST calls require authentication (e.g., signing requests); omitting it is not viable and adds more boilerplate than using an SDK.
- The CLI is a command-line tool for scripting/admin tasks, not for embedding within an application's codebase.

</details>

---

