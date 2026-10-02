## Chapter 5: Deep Learning Foundations Part 2: CNNs, RNNs, Transformers & When to Use DL — Flashcards

| # | Front (Question) | Back (Answer) |
|---|-----------------|---------------|
| 1 | Which DL architecture family is the default choice for image classification and object detection? | CNN (Convolutional Neural Network). Exam tip: 'image data' in a scenario almost always points to CNN. |
| 2 | Which DL architecture family is designed for sequential/time-ordered data like sensor streams or text before Transformers? | RNN (Recurrent Neural Network), including LSTM/GRU variants. Exam tip: keyword 'sequence' or 'time series' → RNN family. |
| 3 | What is the core innovation that lets Transformers outperform RNNs on long text sequences? | Self-attention — computes relationships between all tokens in parallel instead of processing sequentially. Exam tip: 'long-range dependency' + 'parallel processing' = Transformer. |
| 4 | CNN vs RNN vs Transformer — match data type to architecture | CNN = spatial/image data. RNN = sequential/temporal data (older approach). Transformer = sequential data with long-range context, basis of modern LLMs. |
| 5 | In self-attention, what are the three vectors computed for each token? | Query, Key, Value (Q, K, V). Attention weight = compatibility of Query and Key; output = weighted sum of Values. |
| 6 | What operation do CNNs use to extract local features from images? | Convolution — sliding learned filters (kernels) across the image to detect edges, textures, and shapes. |
| 7 | When should you prefer classical ML over deep learning? | When the dataset is small, structured/tabular, and interpretability matters. DL needs large data volumes and is harder to explain. |
| 8 | When should you prefer deep learning over classical ML? | When data is unstructured (images, audio, raw text), large labeled datasets exist, and automatic feature extraction is needed. |
| 9 | What is a known weakness of basic RNNs on very long sequences? | Vanishing/exploding gradients — earlier information degrades as the sequence gets longer, limiting long-range dependency capture. |
| 10 | What architecture family underlies modern large language models (e.g., GPT-style models)? | Transformer — self-attention based, processes tokens in parallel rather than sequentially like RNNs. |
| 11 | Enterprise use case: fraud detection from images of scanned checks — which architecture family? | CNN — image-based feature extraction for spatial pattern recognition (e.g., signature/check anomalies). |
| 12 | Enterprise use case: customer support chatbot understanding multi-turn conversation context — which architecture family? | Transformer — self-attention captures context across the whole conversation, better than RNN for long context. |
