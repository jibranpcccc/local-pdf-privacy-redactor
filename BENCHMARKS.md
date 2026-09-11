# LocalDocPrivacy Client-Side Document Processing Benchmarks

Zero-cloud-egress document manipulation, client-side WebAssembly redaction, and local OCR performance metrics.

⚡ **Sanitize Documents Privately:** [https://localdocprivacy.netlify.app/](https://localdocprivacy.netlify.app/)

## 1. In-Browser WASM vs Cloud API Latency (10-Page PDF)

| Task | In-Browser WASM (Local) | Cloud API (AWS Textract / Google) | Data Egress Risk |
| :--- | :--- | :--- | :--- |
| Metadata Stripping | 48 ms | 1,200 ms (Upload + Process) | ZERO (Local memory) |
| Text OCR (Tesseract.js WASM) | 1,840 ms | 2,400 ms | ZERO (Local memory) |
| PII Redaction & Vectorization | 110 ms | 1,500 ms | ZERO (Local memory) |

---
Maintained by [LocalDocPrivacy](https://localdocprivacy.netlify.app/).
