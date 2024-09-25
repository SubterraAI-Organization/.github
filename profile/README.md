# SubterraAI

SubterraAI has evolved into a highly modular platform that integrates edge computing and real-time image analysis from Minirhizotron tubes. These high-resolution cameras are strategically placed to capture root structures at multiple soil depths, enabling in-situ root phenotyping without disturbing the soil.

## Key Features

### 1. **Split Computing for Efficient Data Processing**
The development of SubterraAI now leverages **split computing**, a new feature designed to tackle the challenges of deploying large deep neural networks (DNNs) on memory-constrained devices. This approach splits the DNN into two parts:
- **Edge Device**: Executes a lightweight version of the model to handle preliminary data processing.
- **Cloud Server**: Offloads complex data processing tasks, optimizing energy efficiency and reducing communication latency.

By employing split computing, SubterraAI ensures rapid data processing in the field while maintaining model accuracy. Using the **YOLOv8 architecture**, we have demonstrated that splitting the network can compress the model while retaining the necessary accuracy for real-time root analysis. This innovation allows for faster processing and improved resource management, even in resource-constrained environments.

### 2. **Advanced Multimodal Deep Learning Architecture**
SubterraAI incorporates an advanced multimodal deep learning architecture (v3) that includes the following models:
- **U-Net**: Excels in consistent data environments, such as medical imaging, providing robust root segmentation.
- **YOLOv8**: Optimized for real-time predictions, suitable for scenarios requiring rapid root structure analysis.
- **Detectron2**: Particularly effective for heterogeneous datasets, adaptable to field conditions where environmental factors vary.

We achieved notable precision and recall scores:
- **YOLOv8**: Precision - 0.85, Recall - 0.85
- **Detectron2**: Precision - 0.98, Recall - 0.98

This combination of models allows us to flexibly select the best-suited model for each specific task, ensuring accurate root segmentation and trait identification.

## How It Works

1. **Data Capture**: Minirhizotron tubes capture high-resolution images of root structures at multiple soil depths.
2. **Edge Processing**: Initial image analysis and preprocessing are performed on edge devices using a split version of the DNN.
3. **Cloud Processing**: The preprocessed data is sent to the cloud server for advanced image analysis using the multimodal deep learning architecture.
4. **Results**: Real-time data analysis enables root phenotyping without soil disturbance, providing researchers with actionable insights.

## Why SubterraAI?

- **Energy Efficiency**: Split computing reduces the computational load on edge devices, optimizing battery life and processing speed.
- **Real-Time Analysis**: YOLOv8's real-time capabilities enable rapid data processing and feedback in field conditions.
- **Flexible Model Selection**: The combination of U-Net, YOLOv8, and Detectron2 allows for tailored analysis depending on environmental and data conditions.
- **High Accuracy**: Achieved precision and recall scores ensure reliable root segmentation and trait identification.


