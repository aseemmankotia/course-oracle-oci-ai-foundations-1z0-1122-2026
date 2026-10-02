## Chapter 10: OCI AI Services Part 2: Document Understanding, Anomaly Detection & Forecasting — Practice Questions

**Q1.** A manufacturing plant streams temperature and vibration readings from 200 sensors every second. The company wants to be alerted the moment a sensor's behavior deviates from its normal historical pattern, without being told what future values will be. Which OCI AI service BEST meets this requirement?

A) OCI Forecasting
B) OCI Anomaly Detection
C) OCI Document Understanding
D) OCI Language

<details>
<summary>Answer</summary>

**Correct: B**

Anomaly Detection is purpose-built to flag outliers in multivariate operational/sensor time-series data using the MSET2 algorithm, exactly matching the 'deviation from normal pattern' requirement.

**Why the others are wrong:**
- Forecasting predicts future numeric values, it does not flag deviations from normal behavior.
- Document Understanding processes documents (text/tables/key-values), not sensor telemetry.
- OCI Language performs NLP tasks like sentiment and entity extraction, not numeric time-series analysis.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** A retail company has three years of monthly historical revenue data and wants to project revenue for the next two quarters to plan inventory. Which OCI AI service should they use?

A) OCI Anomaly Detection
B) OCI Forecasting
C) OCI Document Understanding
D) OCI Vision

<details>
<summary>Answer</summary>

**Correct: B**

OCI Forecasting is designed to predict future values from historical time-series data using AutoML, which fits projecting future revenue.

**Why the others are wrong:**
- Anomaly Detection identifies outliers in existing data, it does not project future values.
- Document Understanding extracts information from documents, unrelated to numeric time-series projection.
- OCI Vision analyzes images/video, not time-series revenue data.

</details>

---

**Q3.** A finance team receives thousands of scanned invoices and needs to automatically pull out the vendor name, invoice number, and total amount as structured key-value pairs. Which OCI AI service capability directly addresses this?

A) OCI Forecasting point predictions
B) OCI Anomaly Detection multivariate signals
C) OCI Document Understanding key-value extraction
D) OCI Speech transcription

<details>
<summary>Answer</summary>

**Correct: C**

OCI Document Understanding's key-value pair extraction feature is specifically designed to pull structured fields like invoice number, vendor, and totals from scanned documents.

**Why the others are wrong:**
- Forecasting works on numeric time-series, not document fields.
- Anomaly Detection works on sensor/operational signals, not documents.
- Speech transcription converts audio to text and has no document field extraction capability.

</details>

---

**Q4.** Which algorithm does OCI Anomaly Detection use internally to detect outliers in multivariate signal data?

A) Random Forest
B) ARIMA
C) MSET2 (Multivariate State Estimation Technique)
D) K-Means Clustering

<details>
<summary>Answer</summary>

**Correct: C**

OCI Anomaly Detection is built on the MSET2 (Multivariate State Estimation Technique) algorithm, developed by Oracle Labs, which models expected sensor behavior and flags deviations.

**Why the others are wrong:**
- Random Forest is a general-purpose ML classifier/regressor, not the algorithm OCI Anomaly Detection is built on.
- ARIMA is a classic univariate time-series forecasting technique, associated more with forecasting than anomaly detection.
- K-Means is an unsupervised clustering algorithm, not what powers OCI Anomaly Detection.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q5.** What is the KEY conceptual difference the exam expects you to know between OCI Anomaly Detection and OCI Forecasting?

A) Anomaly Detection only works with images while Forecasting only works with text
B) Anomaly Detection flags unusual patterns in existing/incoming data while Forecasting predicts future values from historical data
C) Anomaly Detection and Forecasting are the same service with different names
D) Forecasting requires labeled training data while Anomaly Detection requires no data at all

<details>
<summary>Answer</summary>

**Correct: B**

Anomaly Detection identifies outliers in operational/sensor data as it arrives; Forecasting projects future numeric values based on historical time-series trends. This distinction is explicitly tested.

**Why the others are wrong:**
- Neither service is restricted to images or text; both operate on numeric time-series data.
- They are distinct services solving different problems (detection of outliers vs prediction of future values).
- Forecasting does not require manually labeled data, and Anomaly Detection still requires historical data to build its baseline model.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q6.** An insurance company wants to build a solution that: (1) automatically classifies incoming claim documents as 'auto', 'health', or 'property', (2) extracts the claimant's name and claim amount from each form, and (3) flags unusual spikes in claim processing time recorded by their operational monitoring system. Which combination of OCI AI services should they use?

A) OCI Forecasting for classification and extraction, OCI Vision for spikes
B) OCI Document Understanding for classification and extraction, OCI Anomaly Detection for the processing-time spikes
C) OCI Language for classification and extraction, OCI Forecasting for the processing-time spikes
D) OCI Anomaly Detection for classification and extraction, OCI Document Understanding for the processing-time spikes

<details>
<summary>Answer</summary>

**Correct: B**

Document Understanding handles document classification and key-value/text extraction, while Anomaly Detection is the correct service for flagging unusual spikes in operational time-series metrics like processing time.

**Why the others are wrong:**
- Forecasting is not designed for document classification or field extraction.
- OCI Language handles NLP tasks like sentiment analysis, not document classification with layout-aware key-value extraction, and Forecasting doesn't detect spikes.
- The services are reversed — Anomaly Detection cannot classify or extract from documents, and Document Understanding cannot analyze operational time-series metrics.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** A developer wants to programmatically invoke OCI Document Understanding from within a CI/CD pipeline without writing raw HTTP calls. At an awareness level, which consumption method is MOST appropriate?

A) OCI Console only
B) OCI SDK (e.g., Python or Java SDK)
C) Physical data transfer appliance
D) OCI Console UI wizard exclusively, SDKs are not supported

<details>
<summary>Answer</summary>

**Correct: B**

OCI AI services can be consumed via Console, REST APIs, or SDKs; for programmatic pipeline integration without manual HTTP handling, using the language SDK (Python, Java, etc.) is the appropriate abstraction.

**Why the others are wrong:**
- The Console is a manual UI-based method, unsuitable for automated pipeline integration.
- Data transfer appliances are unrelated to invoking AI service APIs.
- SDKs are fully supported for OCI AI services alongside Console and REST API access.

</details>

---

**Q8.** A retailer wants to sort incoming scanned tax forms into pre-defined categories such as W-2, 1099, and receipt, then discard irrelevant scans automatically. Which OCI Document Understanding feature performs this step?

A) Table extraction
B) Key-value pair extraction
C) Document classification
D) Text extraction (OCR)

<details>
<summary>Answer</summary>

**Correct: C**

Document classification is the specific OCI Document Understanding feature that categorizes documents into predefined types like invoice, receipt, or tax form.

**Why the others are wrong:**
- Table extraction pulls tabular structured rows/columns from a document, it does not categorize the document type.
- Key-value pair extraction pulls specific labeled fields (e.g., name, amount), not the overall document category.
- Text extraction (OCR) converts image-based text into machine-readable text but does not classify the document type.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

