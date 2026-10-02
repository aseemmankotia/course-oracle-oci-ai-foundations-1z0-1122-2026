# Chapter 10 Cheat Sheet: Document Understanding, Anomaly Detection & Forecasting

## Service Comparison Table

| Service | Input | Purpose | Key Feature |
|---|---|---|---|
| Document Understanding | Scanned documents/images (PDF, JPEG, PNG, TIFF) | Extract & classify document content | Text, table, key-value extraction + classification |
| Anomaly Detection | Multivariate sensor/operational time-series | Flag outliers/unusual patterns | Built on MSET2 algorithm |
| Forecasting | Historical univariate/multivariate time-series | Predict future values | AutoML-based, outputs prediction + confidence interval |

## Exam Distinction: Anomaly Detection vs Forecasting
- **Anomaly Detection** → "Is this reading normal?" — looks BACKWARD/AT CURRENT data for deviations.
- **Forecasting** → "What will happen next?" — looks FORWARD to predict future values.
- Both use time-series data, but their OUTPUT differs: anomaly flags vs numeric future predictions.

## OCI Document Understanding — Four Capabilities
| Feature | What it does |
|---|---|
| Text extraction (OCR) | Converts image/scan text into machine-readable text |
| Table extraction | Preserves rows/columns from tabular content |
| Key-value extraction | Pulls specific labeled fields (invoice #, vendor, amount) |
| Document classification | Categorizes whole document (invoice, receipt, tax form, etc.) |

## Consumption Methods (Awareness Level)
| Method | Use Case |
|---|---|
| Console | Manual testing, quick demos, no-code exploration |
| REST API | Direct HTTP integration, language-agnostic |
| SDK | Programmatic integration (Java, Python, .NET, Go, TypeScript, Ruby) |

## Common Exam Traps
1. **Confusing Anomaly Detection with Forecasting** — remember: outlier detection ≠ future prediction.
2. **Confusing key-value extraction with table extraction** — key-value = single labeled field; table = structured rows/columns.
3. **Assuming Document Understanding can process live sensor streams** — it only processes documents/images, not time-series telemetry.
4. **Thinking classification and key-value extraction are the same** — classification labels the WHOLE document; key-value extraction pulls specific FIELDS within it.

## Quick Decision Rule
- Documents/scans/forms → **Document Understanding**
- Sensor/operational data + "is this unusual?" → **Anomaly Detection**
- Historical numeric time-series + "predict future" → **Forecasting**

## Memory Trick
"**D**ocuments get **D**ecoded (Document Understanding). **A**nomalies get **A**larmed (Anomaly Detection). **F**orecasts get **F**uture numbers (Forecasting)."
