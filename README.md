Folder Setup for hardware

Currency-Note-Classification-Vitis/
├── .ipynb_checkpoints/          # (existing) Jupyter checkpoint files
├── Dataset/                     # (existing) Training dataset
├── output/                      # (existing) Model output files
├── hw_implementation/           # New folder for hardware files
│   ├── hls/                    
│   │   ├── CNC.cpp             # HLS implementation (moved from root)
│   │   └── include/
│   │       └── cnn_params.h    # CNN parameters
│   │
│   ├── vivado/                 
│   │   ├── constraints/
│   │   │   └── currency_detection.xdc
│   │   ├── ip_repo/
│   │   │   └── cnn_1.0/       # Generated HLS IP
│   │   └── block_design/
│   │       └── system_bd.tcl
│   │
│   └── vitis/                  
│       ├── src/
│       │   └── currency_detection_app.c    # (moved from root)
│       └── include/
│           └── app_params.h
│
├── my_model.keras              # (existing) Keras model file
├── my_model.onnx              # (existing) ONNX model file
└── Currency Note Classification.ipynb  # (existing) Training notebook
