# nndeploy Workflow Collection

## User Guide

### 1. Download Workflow Files
Download JSON configuration files from the corresponding algorithm directories

### 2. Get Model Resources
Visit the [Model Repository](https://modelscope.cn/models/nndeploy/nndeploy/summary) to download required models

### 3. Import Configuration
- Upload JSON files via the frontend workflow interface
- System automatically parses and visualizes node topology

### 4. Configure Parameters
Adjust settings for your use case:
- **Input**: Specify image/video file paths
- **Output**: Set result save paths
- **Parameters**: Configure workflow settings

### 5. Run Workflow
- Verify all configurations
- Execute workflow for automated processing
- View results at the specified output path
- [API Loading and Execution](usage.md)


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
+ **LLM_Qwen** - Qwen Serial LLM - [qwen/LlmQwen.json](qwen/LlmQwen.json)
+ **LLM_Qwen_MNN** - Qwen Serial LLM IMPL MNN - [qwen/LLM_Qwen_MNN.json](qwen/LLM_Qwen_MNN.json)
+ **Qwen** - Qwen2 Intelligent Dialogue System - [qwen/LLM_Qwen2_0.5B.json](qwen/LLM_Qwen2_0.5B.json)


### 🎨 AI Content Generation
+ **Text-to-Image** - Stable Diffusion Text-to-Image Generation impl C++ - [fp16 precision](stable_diffusion/Text_2_Image_stable_diffusion_1.5_fp16.json), [fp32 precision](stable_diffusion/Text_2_Image_stable_diffusion_1.5_fp32.json)
+ **Text-to-Image** - Text-to-Image Generation impl diffusers - [diffusion/Text2Image_Impl_Diffusers.json](diffusion/Text2Image_Impl_Diffusers.json)
+ **Text-to-Image** - Text-to-Image Generation impl diffusers - [diffusion/Text2Image_CogView4_Impl_Diffusers.json](diffusion/Text2Image_CogView4_Impl_Diffusers.json)
+ **Inpaiting** - Image inpainting workflow based on Diffusers - [diffusion/Inpaiting_Impl_Diffusers.json](diffusion/Inpaiting_Impl_Diffusers.json)
+ **Image-to-image** - Image-to-image generation workflow based on Diffusers - [diffusion/Image2Image_Impl_Diffusers.json](diffusion/Image2Image_Impl_Diffusers.json)

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