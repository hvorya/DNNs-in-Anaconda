### [How to install Cuda on Windows 11 and Anaconda?] 

1. Cuda & CuDNN files Download

2. Python 3 & pip with Anaconda(latest installed)

3. Microsoft Visual Studio 2022 C++ redistributables with dot net 4.5 or above installed
4. Make sure you have already Anaconda installed with JupyterNotebook & everything is working fine.

5. Download the CUDA toolkit from here:- https://developer.nvidia.com/cuda-downloads#

6. choose your options like OS and arch of OS based on your system configurations. Then download the file and install it in your C//: DRIVE, while installation uses EXPRESS(recommended) mode.

![Screenshot 2024-08-03 014128](https://github.com/user-attachments/assets/33717b2f-5b11-4c22-bd14-274a9eaab141)


7. After installing CUDA, you must download CuDNN (https://developer.nvidia.com/rdp/cudnn-archive), an extension that supports CUDA files for running Deep Learning applications.
- NOTE: MAKE SURE THE CUDNN VERSION AND CUDA TOOLKIT VERSIONS ARE SAME
8. Once you have downloaded CuDNN Local Installer for Windows (Zip), extract files to the CUDA installation directory in C:// drive
9. now one by copy & replace these folders to the CUDA installation directory

![1_VkR65ExTc1ZKQrjrQr-cPw](https://github.com/user-attachments/assets/af1088b2-8daf-4fcc-a45e-88e0bbaba196)

![1_Jz9mDeZrs7PFxTIIZxNUKg (1)](https://github.com/user-attachments/assets/30134d63-8035-4242-9d2a-8a2937d69122)

10. you have finally completed your CUDA Toolkit installation with CuDNN.
11. Now it’s time to set Path variables → open Edit environment variables in the Windows search bar, Click on Environment variables, click on “path” under user variables, then add the paths of “bin” and “lineup.”

- Right-click on Start, then click on Run.
Type: sysdm.cpl and click on OK.
Click on the "Advanced" tab, then click on the "Environment Variables..."
    
12. Finally, you’re done with the installation part of CUDA & CuDNN; just verify it’s properly installed, Goto Power-Shell, and enter the command “Nvidia-semi.”

![1_p32768CJR5XBOpA7CPLiMw (1)](https://github.com/user-attachments/assets/eec5eeed-d273-4ceb-b830-1fa5ad485ee1)


######################################################################## In cmd.exe prompt
1. conda create -n <myenv> python=3.6.8
2. conda activate <myenv>
3. conda install -c anaconda tensorflow-gpu keras-gpu
4. conda install pytorch torchvision torchaudio pytorch-cuda=12.4 -c pytorch -c nvidia   # batavajoh be version cuda 
5. pip install ipykernel

6. python -m ipykernel install --user --name <myenv> --display-name "Python (GPU)"    # then launch jypiternotebook
7. pip install --upgrade jupyterhub
8. pip install --upgrade --user nbconvert
