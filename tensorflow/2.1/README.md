Tensflow Singularity container

Anaconda3: 2020.02 
Tensorflow: 2.1
HostOS: Ubuntu 18.04

Build
```
srun --pty bash
module load singularity
make
```

Usage

Running tensorflow in interactive mode

```
srun --pty bash
module load singularity
singularity run anaconda-2020.02-tensorflow-2.1.simg -c bash
```
