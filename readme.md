###How to install cuda on windows 11? 

1. Cuda & CuDNN files Download

2. Python 3 & pip with Anaconda(latest installed)

3. Microsoft Visual studio 2022 C++ redistributables with dot net 4.5 or above installed
4. Make sure you have already Anaconda installed with JupyterNotebook & everything is working fine.

5. Download CUDA toolkit from here :- https://developer.nvidia.com/cuda-downloads#

6. choose your options like OS and arch of OS based on your system configurations. Then download the file and install it in your C//: DRIVE , while installation uses EXPRESS(recommended) mode.

![Alt text] (Screenshot 2024-08-03 014128.png)


7.After installation of CUDA , you have to download CuDNN (https://developer.nvidia.com/rdp/cudnn-archive) which is an extension supporting files of CUDA for running Deep Learning applications.
NOTE : MAKE SURE THE CUDNN VERSION AND CUDA TOOLKIT VERSIONS ARE SAME
8. Once you have downloaded CuDNN Local Installer for Windows (Zip) extract files at CUDA installation directory in C:// drive
9. now one by copy & replace these folders to CUDA installation directory

10. you have finally completed your CUDA Toolkit installation with CuDNN.
11. Now it’s time to set Path variables → open Edit environment variables in windows search bar , Click on Environment variables , the click on “path” under user variables then add path of “bin” and “libnvvp”.
12.Finally you’re done with the installation part of CUDA & CuDNN , just verify it’s properly installed , Goto Power-Shell and enter command “nvidia-smi”.



######################################################################## In cmd.exe prompt
1. conda create -n <myenv> python=3.6.8
2. conda activate <myenv>
3. conda install -c anaconda tensorflow-gpu keras-gpu
4. conda install pytorch torchvision torchaudio pytorch-cuda=12.4 -c pytorch -c nvidia   # batavajoh be version cuda 
5. pip install ipykernel

6. python -m ipykernel install --user --name <myenv> --display-name "Python (GPU)"    # then launch jypiternotebook
7. pip install --upgrade jupyterhub
8. pip install --upgrade --user nbconvert