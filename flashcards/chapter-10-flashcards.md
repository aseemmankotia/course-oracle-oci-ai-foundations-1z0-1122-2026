## Chapter 10: OCI AI Services Part 2: Document Understanding, Anomaly Detection & Forecasting — Flashcards

| # | Front (Question) | Back (Answer) |
|---|-----------------|---------------|
| 1 | What algorithm powers OCI Anomaly Detection? | MSET2 (Multivariate State Estimation Technique). Exam tip: know this is Oracle-developed and used specifically for detecting outliers in multivariate sensor/operational data. |
| 2 | OCI Anomaly Detection vs OCI Forecasting — core distinction? | Anomaly Detection flags unusual/outlier patterns in existing data; Forecasting predicts future values from historical time-series data. Exam tip: 'is this normal?' = Anomaly Detection, 'what happens next?' = Forecasting. |
| 3 | What are the four core capabilities of OCI Document Understanding? | Text extraction (OCR), table extraction, key-value pair extraction, and document classification. Exam tip: each maps to a distinct exam scenario keyword. |
| 4 | Which OCI AI service is used for predictive maintenance based on IoT sensor readings? | OCI Anomaly Detection. Exam tip: sensor data + 'unusual behavior' = Anomaly Detection, not Forecasting. |
| 5 | Which OCI AI service extracts vendor name and total amount from a scanned invoice as structured fields? | OCI Document Understanding's key-value pair extraction. Exam tip: 'structured labeled fields from a document' always points to key-value extraction, not text extraction. |
| 6 | What three methods can be used to consume OCI AI services? | OCI Console (UI), REST APIs, and SDKs (e.g., Java, Python, .NET, Go, TypeScript, Ruby). Exam tip: awareness-level only — know these three exist, not implementation details. |
| 7 | Does OCI Forecasting require labeled training data like a classification model? | No. It uses AutoML on historical time-series data to build the forecasting model automatically. Exam tip: contrast with supervised classification services that need labeled datasets. |
| 8 | What does OCI Forecasting output alongside a predicted value? | A prediction plus a confidence/prediction interval. Exam tip: exam may ask why intervals matter — they express forecast uncertainty. |
| 9 | A company wants to sort scanned documents into 'invoice', 'receipt', or 'tax form' categories. Which Document Understanding feature applies? | Document classification. Exam tip: classification = whole-document category, not field-level extraction. |
| 10 | Table extraction in OCI Document Understanding is used for what type of content? | Extracting structured rows and columns (e.g., line items on an invoice) while preserving their tabular layout. Exam tip: distinct from key-value pairs, which are single labeled fields. |
| 11 | Which OCI AI service would you choose for detecting unusual spikes in server CPU/memory metrics? | OCI Anomaly Detection. Exam tip: any scenario mentioning 'operational metrics', 'sensor data', or 'unusual spikes' signals this service. |
| 12 | Which OCI AI service would you choose to project next quarter's sales using 3 years of monthly sales history? | OCI Forecasting. Exam tip: 'historical time-series' + 'predict future' always maps to Forecasting. |
