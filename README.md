# Kadena GPU miner for NVIDIA & AMD graphic cards


### Links 

Website: http://noncer.pro

Discord server : https://discord.gg/mXnyrHa

releases: https://github.com/NoncerPro/Kadena/releases

![](https://img.shields.io/github/downloads/NoncerPro/Kadena/total.svg?style=plastic)

Options
------------------------------------------
```Options:
  -a, --address     Your public key                          [string] [required]
  -m, --mode        force solo or pool mining mode
                    Default is based on server url                      [string]
  -s, --server      Server address
                    Example: -s fr1.chainweb.com or
                    -s fr1.chainweb.com:443                   [array] [required]
  -p, --port        Server port
                    You don't need this if server address has
                    the port appended at the end                         [array]
  --pl, --platform  Mining platform
                    nvidia or amd
                    Default: nvidia                                     [string]
  -n, --name        Rig name                                            [string]
  -x, --pass        Pool password                                       [string]
  -d, --devices     Active GPUs
                    Example: -d=0 1 3
                    Default: All available GPUs                          [array]
  -t, --threads     Number of threads per GPU
                    Example: -t 2 or -t 2 2 4
                    Default: 2                                           [array]
  -i, --intensity   between 10 to 30. Supports decimals
                    Maximum for none rtx nvidia cards is 23
                    Example: -i 26.5 or -i 23.6 25
                    Default: 26                                          [array]
  -c, --chain       Preferred chain to mine on                          [number]
  -r, --random      Enable/Disable random starting nonce
                    Default: false                                     [boolean]
  --ai, --api       Enable/Disable API
                    Default: true                                      [boolean]
  --ap, --apiport   API port
                    Default: 3000                                       [number]
  -u, --usebin      AMD only. Use prebuilt kernel binaries
                    Default: true                                      [boolean]
  -h, --help        Show help                                          [boolean]
  -v, --version     Show version number                                [boolean]
```

Requirements
------------------------------------------
Nvidia kernels have been built with **CUDA 10.0**. You need to update your driver to the latest version in order to use them.

The minimum supported Compute Capability is SM3.5. You can check your cards' SM support in the following link:
https://developer.nvidia.com/cuda-gpus

AMD kernel has been only tested on amdgpupro driver. This miner does not support rocm and other drivers.

If you are running the noncerpro.exe file directly, make sure you have set UV_THREADPOOL_SIZE to atleast 32;

Usage
------------------------------------------
Download the binary packge for Windows/Linux, edit mine-nvidia or mine-amd bash/bat file and insert your own wallet address and run it.

Make sure you tune intensity with -i or --intensity. It supports decimals for fine tuning (eg :-i 26.5).
   
Overclocking
------------------------------------------
Blake2s is a core intensive algo. Don't waste your time on memory clock.

HiveOS
------------------------------------------
Soon

Dev fee
------------------------------------------
This miner has a fixed 2% dev fee. That means 5 minutes in every 100 minutes, miner will run with the donation address. 
Devfee of versions prior to 2.0 is 5%.

Happy mining!
