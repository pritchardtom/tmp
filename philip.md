# PyTorch Instructions on Sunbird

Firstly, I installed PyTorch as follows:

```
module load anaconda/2021.05
source activate 
conda create -n philip_pytorch pytorch==1.12.1 torchvision==0.13.1 torchaudio==0.12.1 cudatoolkit=11.6 -c pytorch -c conda-forge
```

Then I found a few simple `torch.cuda` functions to call and created a simple `example.py` script:

```python3
import torch

print(torch.cuda.current_device())
print(torch.cuda.get_device_capability())
print(torch.cuda.get_device_properties(0))
```

And finally, I created this basic SLURM submission script I called `submit.sh`:

```
#!/bin/bash --login

#SBATCH --job-name=pytorch_example  # name of job
#SBATCH --output=output.out         # output from running job will be saved here
#SBATCH --error=error.err           # errors from running job will be saved here
#SBATCH --partition=gpu             # compute for CPUs, and gpu for GPUs
#SBATCH --gres=gpu:1                # how many GPUs does the job need?
#SBATCH --time=00:00:10             # how long does job need (here I asked for 10 seconds)
#SBATCH --nodes=1                   # how many nodes does job need (2 GPUs per compute node)
#SBATCH --account=scw1001           # the project you belong to (cannot submit jobs if not member of project

module load anaconda/2021.05
source activate 
conda activate philip_pytorch

python example.py
```

Here are the contents of `output.out` file after job has successfully run:

```
0
(7, 0)
_CudaDeviceProperties(name='Tesla V100-PCIE-16GB', major=7, minor=0, total_memory=16160MB, multi_processor_count=80)
```
