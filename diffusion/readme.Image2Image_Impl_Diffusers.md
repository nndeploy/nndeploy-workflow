
# Diffusion Pipeline Quick Guide

This manual provides a concise introduction to deploying and using text2image, image2image, and inpainting in nndeploy.

---

## 1. Model Download and Environment Configuration

- **Domestic Acceleration**:  
  Set Hugging Face mirror before startup to accelerate model downloads.  
  Linux/macOS:
  ```bash
  export HF_ENDPOINT=https://hf-mirror.com
  ```
  Windows PowerShell:
  ```powershell
  $env:HF_ENDPOINT = "https://hf-mirror.com"
  ```

- **Restricted Model Access**:  
  Need to apply for permissions on Hugging Face, obtain Access Token and login.  
  1. Visit model page and apply for permissions  
  2. [Get Access Token](https://huggingface.co/settings/tokens)  
  3. Install tools and login:
     ```
     pip install huggingface_hub
     huggingface-cli login --token <your_token>
     ```

---

## 2. Memory and Performance Optimization

- **enable_model_cpu_offload**: Significantly reduces VRAM usage when enabled, recommended when VRAM is insufficient.
- **enable_sequential_cpu_offload**: Further reduces VRAM usage with slightly decreased speed.
- **xformers**: After installation, enable `enable_xformers_memory_efficient_attention` to improve efficiency and reduce VRAM.
  ```
  pip install xformers
  ```

---

## 3. Main Parameters Reference

| Parameter Name        | Description            | Recommended/Default  |
|-----------------------|------------------------|----------------------|
| pretrained_model_name_or_path | Model name or local path | See official docs |
| torch_dtype           | Inference precision    | float16              |
| use_safetensors       | Prefer safetensors weights | True             |
| num_inference_steps   | Sampling steps         | 20~50                |
| guidance_scale        | Text guidance strength | 7.5~12.0             |
| guidance_rescale      | Guidance rescaling     | 0.0                  |
| scheduler             | Sampler type           | default              |
| strength              | Edit/repair original image retention ratio | 0.8 |
| is_random             | Whether to use random seed | True             |
| generator_seed        | Random seed            | 42                   |
| enable_model_cpu_offload | Transfer weights to CPU | False            |
| enable_sequential_cpu_offload | Sequential CPU offload | False         |
| enable_xformers_memory_efficient_attention | xformers efficient attention | False |

---

## 4. Common Issues Quick Reference

- **Slow/Failed Downloads**: Configure Hugging Face mirror, check model permissions, use local models.
- **Insufficient VRAM**: First enable `enable_model_cpu_offload`, then consider `enable_sequential_cpu_offload`.
- **Slow Inference**: Disable `enable_sequential_cpu_offload` or upgrade hardware.
- **xformers Installation Failed**: Check Python/CUDA compatibility, see [official documentation](https://github.com/facebookresearch/xformers).

---

If you have any questions, feel free to submit issues or join our discussion group.
