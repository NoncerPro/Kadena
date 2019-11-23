# Kadena GPU miner for Nvidia graphic cards


### Links 

Website: http://noncer.pro

Discord server : https://discord.gg/mXnyrHa

releases: https://github.com/NoncerPro/Kadena/releases


Options
------------------------------------------
```Options:
  -a, --address    Your public key                           [string] [required]
  -s, --server     Node server address
                   Example: -s fr1.chainweb.com               [array] [required]
  -p, --port       Node server port                           [array] [required]
  -n, --name       Rig name                                             [string]
  -d, --devices    Active GPUs
                   Example: -d=0 1 3
                   Default: All available GPUs                           [array]
  -t, --threads    Number of threads per GPU
                   Example: -t 2 or -t 2 2 4
                   Default: 1                                            [array]
  -i, --intensity  between 10 to 30. Supports decimals
                   Example: -i 26.5 or -i 23.6 30 25
                   Default: 26.5                                         [array]
  --api            Enable/Disable API
                   Default: Enable                                     [boolean]
  --apiport        API port
                   Default: 3000                                        [number]                 
  -c, --chain      Preferred chain to mine on                           [number]
  -h, --help       Show help                                           [boolean]
  -v, --version    Show version number                                 [boolean]
```

Requirements
------------------------------------------
Binary packages have been built with **CUDA 10.0**. You need to update your driver to the latest version in order to use them.

The minimum supported Compute Capability is SM3.5. You can check your cards' SM support in the following link:
https://developer.nvidia.com/cuda-gpus

If you are running the noncerpro.exe file directly, make sure you have set UV_THREADPOOL_SIZE to atleast 32;

Usage
------------------------------------------
Download the binary packge for Windows/Linux, edit mine.bat/mine.sh file and insert your own wallet address and run it.

Make sure you tune intensity with -i or --intensity. It supports decimals for fine tuning (eg :-i 26.5).
   
Overclocking
------------------------------------------
Blake2s is a core intensive algo. Don't waste your time on memory clock.

HiveOS
------------------------------------------
Soon

Dev fee
------------------------------------------
This miner has a fixed 5% dev fee. That means 5 minutes in every 100 minutes, miner will run with the donation address. 

Happy mining!
