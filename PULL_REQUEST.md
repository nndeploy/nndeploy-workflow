# PR

## Workflow Template Submission Guide

This document explains how to submit a complete nndeploy workflow template. Using the face_swap algorithm as an example, it demonstrates the required file structure and specifications.

### Required Files

#### 1. Workflow Configuration File
- **Filename**: `face_swap.json`
- **Description**: Workflow definition file containing complete node connections and parameter configurations

#### 2. Input Resource Files
- **Filename**: Must match the internal reference names in the workflow
- **Description**: Test input data required for workflow execution (images, videos, etc.)

## Optional Files

#### 3. Dependencies Configuration File
- **Filename**: `requirements.face_swap.txt`
- **Naming Convention**: Must follow the format `requirements.[algorithm_name].txt`
- **Description**: Lists Python dependency packages and versions required for workflow execution

#### 4. Usage Documentation
- **Filename**: `readme.face_swap.md`
- **Naming Convention**: Must follow the format `readme.[algorithm_name].md`
- **Content Requirements**:
  - Python dependency package installation steps
  - Workflow usage instructions and parameter configuration guide
  - Common issues and solutions

#### 5. Cover Image
- **Filename**: `cover.face_swap.jpg`
- **Naming Convention**: Must follow the format `cover.[algorithm_name].jpg`
- **Size Requirements**: Fixed dimensions, adapted for frontend grid layout display

## 工作流模板提交指南

本文档说明如何提交一个完整的nndeploy工作流模板。以换脸(face_swap)算法为例，展示所需的文件结构和规范。

### 必需文件

#### 1. 工作流配置文件
- **文件名**: `face_swap.json`
- **说明**: 包含完整的节点连接关系和参数配置的工作流定义文件

#### 2. 输入资源文件
- **文件名**: 与工作流内部引用名称保持一致
- **说明**: 工作流运行所需的测试输入数据（图片、视频等）

## 可选文件

#### 3. 依赖配置文件
- **文件名**: `requirements.face_swap.txt`
- **命名规范**: 必须遵循 `requirements.[算法名].txt` 格式
- **说明**: 列出工作流运行所需的Python依赖包及版本

#### 4. 使用说明文档
- **文件名**: `readme.face_swap.md`
- **命名规范**: 必须遵循 `readme.[算法名].md` 格式
- **内容要求**:
  - Python依赖包的安装步骤
  - 工作流的使用方法和参数配置说明
  - 常见问题和解决方案

#### 5. 封面图片
- **文件名**: `cover.face_swap.jpg`
- **命名规范**: 必须遵循 `cover.[算法名].jpg` 格式
- **尺寸要求**: 固定尺寸，适配前端展示的方块网格布局

