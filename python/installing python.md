The steps to install Python:

#  1.   Download Python
1. Open your web browser and go to the [official Python download page](https://www.python.org/downloads/).
2. Click on the [Download Python] button. This will download the latest version of Python.

#   2. Run the Installer
1. Once the download is complete, locate the downloaded file (`python-<version>.exe`) in your Downloads folder.
2. Double-click the installer to run it.

#   3. Install Python
1. Start the Installer:
   - When the installer window opens, make sure to check the box that says [Add Python to PATH] at the bottom.
   - Click on [Customize installation] to proceed with the installation.

2. Optional Features:
   - Ensure that the following features are selected:
     - Documentation
     - pip (Python's package installer)
     - tcl/tk and IDLE
     - Python test suite
     - py launcher
   - Click [Next].

3. Advanced Options:
   - Ensure that the following options are selected:
     - Install for all users
     - Add Python to environment variables
   - Optionally, you can select other options as needed.
   - Choose the installation directory or leave it as default. Click [Install].

4. Wait for Installation:
   - The installer will install Python and its components. This process may take a few minutes.

5. Complete the Installation:
   - Once the installation is complete, you will see a setup was successful message. Click on [Close].

#  4. Verify the Installation
1. Open Command Prompt or PowerShell:
   - Press `Win + R`, type `cmd`, and press Enter to open Command Prompt.
   - Alternatively, you can press `Win + R`, type `powershell`, and press Enter to open PowerShell.

2. Check Python Version:
   - In the Command Prompt or PowerShell, type the following command and press Enter:
     ```sh
     python --version
     ```
   - This should display the version of Python that you installed.

3. Check pip Version:
   - To verify that pip was installed correctly, type the following command and press Enter:
     ```sh
     pip --version
     ```
   - This should display the version of pip that was installed.

#   5. Install Additional Packages (Optional)
1. Use pip to Install Packages:
   - You can install additional Python packages using pip. For example, to install `numpy`, type the following command and press Enter:
     ```sh
     pip install numpy
     ```
