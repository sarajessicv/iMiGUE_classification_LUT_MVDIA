# iMiGUE Micro Gesture Classification

### System requirements

-   Ubuntu 16.04 or higher (64-bit)
-   macOS 10.12.6 (Sierra) or higher (64-bit) (no GPU support)
-   Windows Native - Windows 7 or higher (64-bit) (no GPU support after TF 2.10)
-   Windows WSL2 - Windows 10 19044 or higher (64-bit)

### Software requirements

-   Python (version 3.9<=3.11)
-   pip (version >=19.0 for Linux and Windows native, 20.3 or higher on macOS)
-   Windows Native Requires [Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019](https://learn.microsoft.com/fi-FI/cpp/windows/latest-supported-vc-redist?view=msvc-170)

### Python virtual environment creation

-   Step 1: Create the python virtual environment with the command `python -m venv .$NAME OF YOUR ENVIRONMENT$`
-   Step 2: Activate the virtual environment with command `.$NAME OF THE ENVIRONMENT$\Scripts\activate.bat` on Windows, `source .$NAME OF THE ENVIRONMENT$/bin/activate` on other OSs
-   Step 3: Install the required packages with the command `pip install -r requirements.txt`
-   Step 4: Success!

### The project structure

`./datamanipulation.ipynb`: A notebook with which the training data has been modified to fit the models. (not needed for inference/testing) <br>
`./pose.ipynb`: A notebook with which the Main model has been trained with. (not needed for inference/testing) <br>
`./Test_inference.ipynb`: Run this notebook to run inference on the created models. (remember to change the directory of the testing data manually in this notebook) <br>
`./models`: A folder which hosts all of the relevant files for the pretrained model <br>

The Github page of the iMiGUE dataset can be found [here](https://github.com/linuxsino/iMiGUE). 

### NOTE!

The implementation has been ran succesfully only on macOS Sonoma 14.3.1. (Unix based) system thus far. If you intend to run the codes on Windows, Tensorflows recommended way is to use a WSL-virtual machine (see guide at https://www.tensorflow.org/install/pip#windows-wsl2)
