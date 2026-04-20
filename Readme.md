Segmentation Guided EndoCLIP Foundation Model

```bash
ENDOMEDCLIP/
│
├── data/
│   ├── raw/
│   │   ├── Kvasir-SEG/
│   │   └── cvcclinicdb/
│   ├── processed/
│   │   ├── manifests/
│   │   ├── bboxes/
│   │   └── visualizations/
│
├── notebooks/
│   ├── 01_dataset_audit.ipynb
│   ├── 02_mask_to_patch_debug.ipynb
│   └── 03_dual_view_debug.ipynb
│
├── src/
│   ├── config.py
│   ├── utils/
│   │   ├── io.py
│   │   ├── masks.py
│   │   ├── visualize.py
│   │   └── bbox.py
│   ├── datasets/
│   │   ├── kvasir.py
│   │   ├── cvc.py
│   │   └── combined.py
│   ├── tokenization/
│   │   └── mask_to_patch.py
│   ├── models/
│   │   ├── clip_encoder.py
│   │   └── dual_view_encoder.py
│   └── scripts/
│       ├── audit_kvasir.py
│       ├── audit_cvc.py
│       ├── export_bboxes.py
│       ├── visualize_patch_tokens.py
│       └── test_dual_view.py
│
├── tests/
│   ├── test_mask_to_patch.py
│   ├── test_bbox_extraction.py
│   └── test_dataset_loading.py
│
├── requirements.txt
├── README.md
└── .gitignore
```
