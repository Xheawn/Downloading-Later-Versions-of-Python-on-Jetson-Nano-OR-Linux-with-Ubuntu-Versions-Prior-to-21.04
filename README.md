# Downloading-Newer-Versions-of-Python-on-Jetson-Nano-Linux-with-Ubuntu-Versions-Prior-to-21.04
This tutorial helps you to download newer versions of Python without using the deadsnakes packages

Since only the Ubuntu with versions >= 21.04 support newer versions of Python (Ubuntu versions prior to 21.04 typically don't support downloading newer versions of Python directly through the standard APT repositories, such as Python3.10), users with Ubuntu version < 21.04 used other methods. 

For example, the most common one was using the deadsnakes packages to solve this problem. However, the author of the deadsnakes stopped providing the packages from June 2023, thus that method is no longer available. 

Therefore, this is sort of a tutorial that guides you to install newer versions of python (in my case it was Python3.10) on your Jetson Nano or Linux. Follow the following steps to make it happen!

# 1 - Downloading Python from the Official Website
Find the Python version you want to install on the offcial Python downloading website.

https://www.python.org/downloads/source/

# 2 - Extract the Downloaded Python Tarball and cd into its Directory
After you done with the extraction, open your and terminal enter:

cd "your python directory"

Note that you replace "your python directory" with where you installed it. It was /home/usr/Downloads/Python-3.10.13 in my case.

# 3 - Build and Install
Enter: 

make

This command typically takes a long time to process, please be patient wait until it's done.

Then enter:

sudo make altinstall

# 4 - Verify your installation
Enter:

python3.x


to verify that it is successfully installed (Replace "x" with the version number).

 



