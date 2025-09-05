
Installing Python dependencies is required to execute this algorithm

step1: Download [requirements.face_swap_gan.txt](https://github.com/nndeploy/nndeploy-workflow/blob/main/face_swap/requirements.face_swap_gan.txt)

step2: 

```bash
pip install -r requirements.face_swap_gan.txt
# uninstall the current version of basicsr:
pip uninstall basicsr -y

# install basicsr directly from its GitHub repository:
pip install git+https://github.com/xinntao/BasicSR.git@master

# After installation is complete, also reinstall gfpgan:
pip uninstall gfpgan -y
pip install git+https://github.com/TencentARC/GFPGAN.git@master
```

step3: Restart nndeploy-app