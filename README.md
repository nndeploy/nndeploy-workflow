# nndeploy Workflow Collection

## User Guide

### 1. Obtain Workflow Files
Download the required workflow JSON configuration files from the corresponding algorithm directories:
- Object Detection: `detect/yolo.json`
- Image Classification: `classification/resnet.json`
- Object Tracking: `track/track.json`
- Object Segmentation: `segment/rmbg.json`
- Text-to-Image: `stable_diffusion/stable_diffusion_1.5.json`

### 2. Prepare Model Resources
Visit the [Model Repository](https://modelscope.cn/models/nndeploy/nndeploy/summary) to obtain corresponding models:
- Model files are systematically organized by algorithm type
- Please ensure complete download of model weight files and related configurations

### 3. Import Workflow Configuration
- Upload JSON configuration files through the frontend workflow management interface
- The system will automatically parse and visualize the node topology structure

### 4. Parameter Configuration Optimization
Adjust key parameters according to specific application scenarios:
- **Input Configuration**: Specify input image/video file paths
- **Output Configuration**: Set save paths for processing results
- **Core Parameters**:
  - `model_type_`: Model file format type
  - `model_value_`: Complete model file path
  - `device_type_`: Computing device type (CPU/GPU/NPU)
  - Other algorithm-specific parameters

### 5. Execute Workflow
- Verify the correctness of all parameter configurations
- Start the workflow for automated processing
- The system executes in order according to predefined node dependencies
- View processing results at the specified path upon completion

## Complete List

### 🎯 Computer Vision Fundamental Algorithms
+ **Object Detection** - YOLO Series High-Precision Object Detection - [detect/Detect_YOLO.json](detect/Detect_YOLO.json)
+ **Image Classification** - ResNet Deep Learning Image Classification - [classification/Classification_ResNet.json](classification/Classification_ResNet.json)
+ **Object Tracking** - Multi-Object Video Tracking Algorithm - [track/Track_FairMot.json](track/Track_FairMot.json)
+ **Object Segmentation** - Intelligent Background Removal Segmentation - [segment/Segment_RMBG.json](segment/Segment_RMBG.json)
+ **Universal Segmentation** - Segment Anything Universal Segmentation - [segment/Segment_Anything.json](segment/Segment_Anything.json)

### 📝 Text Recognition Processing
+ **OCR Recognition** - High-Precision Optical Character Recognition - [ocr/OCR.json](ocr/OCR.json)

### 🤖 Large Language Model Applications
+ **Qwen Dialogue** - Qwen2 Intelligent Dialogue System - [qwen/LLM_Qwen2_0.5B.json](qwen/LLM_Qwen2_0.5B.json)

### 🎨 AI Content Generation
+ **Text-to-Image** - Stable Diffusion Text-to-Image Generation - [fp16 precision](stable_diffusion/Text_2_Image_stable_diffusion_1.5_fp16.json), [fp32 precision](stable_diffusion/Text_2_Image_stable_diffusion_1.5_fp32.json)

### 👤 Face Processing Technology
+ **Basic Face Swap** - High-Quality Face Replacement - [face_swap/Face_Swap.json](face_swap/Face_Swap.json)
+ **Enhanced Face Swap** - Face Swap + GFPGAN Super-Resolution Enhancement - [face_swap/Face_Swap_Gan.json](face_swap/Face_Swap_Gan.json)
+ **Video Face Swap** - Batch Video Face Replacement Processing - [V1 Version](face_swap/Video_Swap_Face.json), [V2 Version](face_swap/Video_Swap_Face_V2.json)
+ **Real-time Face Swap** - Camera Real-time Face Replacement - [face_swap/Face_swap_from_camera.json](face_swap/Face_swap_from_camera.json)
+ **Multi-Face Swap** - Multi-Face Synchronous Replacement + Quality Enhancement - [face_swap/face_swap_gan_many_face.json](face_swap/face_swap_gan_many_face.json)

### 🌐 API Service Integration
+ **AIGC API** - AI Generated Content Standardized API Interface - [api_aigc/API_AIGC_OpenAI_Text_2_Image.json](api_aigc/API_AIGC_OpenAI_Text_2_Image.json)
+ **LLM API** - Large Language Model Dialogue API Service - [api_llm/API_LLM_Chat.json](api_llm/API_LLM_Chat.json)

### 🚀 Creative Algorithm Combinations
+ **Face Swap Segmentation Fusion** - Face Replacement + Background Intelligent Segmentation - [creative/Face_Swap_GAN_Segment.json](creative/Face_Swap_GAN_Segment.json)
+ **Multi-Algorithm Pipeline** - Segmentation + Detection + Classification Integrated Processing - [creative/Segment_Detect_Classification.json](creative/Segment_Detect_Classification.json)