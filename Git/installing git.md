Steps to install Git (Version Control System):

#   1. Download Git
1. Open your web browser and go to the [official Git download page](https://git-scm.com/).
2. Click on the **Download for Windows** button. This will download the installer for Git.

#   2. Run the Installer
1. Once the download is complete, locate the downloaded file (`Git-<version>-64-bit.exe`) in your Downloads folder.
2. Double-click the installer to run it.

#   3. Install Git
1. The setup wizard will appear. Click on the [Next] button to proceed.
2. Select the destination location where you want Git to be installed or leave it as the default. Click [Next].
3. Select the components you want to install. The default options are usually fine. Click [Next].
4. Choose the start menu folder for the Git shortcuts or leave it as the default. Click [Next].
5. Select the default editor used by Git. You can choose **Visual Studio Code** if you have it installed, or any other text editor you prefer. Click [Next].
6. Adjust the PATH environment. It's recommended to use "Git from the command line and also from 3rd-party software." Click [Next].
7. Choose the HTTPS transport backend. Select **Use the OpenSSL library**. Click [Next].
8. Choose the line ending conversion. Select **Checkout Windows-style, commit Unix-style line endings**. Click [Next].
9. Choose the terminal emulator to use with Git Bash. You can select **Use MinTTY (the default terminal of MSYS2)**. Click [Next].
10. Choose the default behavior of `git pull`. You can use the default option or adjust according to your preference. Click [Next].
11. Choose credential helper. Select [Git Credential Manager Core]. Click [Next].
12. Enable file system caching and symbolic links if needed. Click [Next].
13. Experiment with extra options if you need them. Click [Next].
14. Click [Install] to start the installation process.

#   4. Complete the Installation
1. Once the installation is complete, ensure the checkbox for **Launch Git Bash** is selected.
2. Click [Finish]. Git Bash will open.

#   5. Configure Git
1. Open [Git Bash] from the start menu or the desktop shortcut.
2. Configure your username and email address, which will be associated with your Git commits. Run the following commands in Git Bash:

    ```bash
    git config --global user.name "bahati"
    git config --global user.email "bahatijacklee8.gmail@.com"
    ```

3. Verify the configuration by running:

    ```bash
    git config --list
    ```

#   6. **Generate SSH Key (Optional)**
If you plan to use SSH for authentication with Git repositories (like GitHub or GitLab), you need to generate an SSH key.

1. In Git Bash, run the following command:

    ```bash
    ssh-keygen -t rsa -b 4096 -C "bahatijacklee8.gmail@.com"
    ```

2. Press Enter to accept the default file location.
3. Enter a passphrase (optional) and confirm it.
4. Add the SSH key to the SSH agent by running:

    ```bash
    eval "$(ssh-agent -s)"
    ssh-add ~/.ssh/id_rsa
    ```

5. Copy the SSH key to your clipboard:

    ```bash
    clip < ~/.ssh/id_rsa.pub
    ```

6. Add the SSH key to your Git hosting service (GitHub, GitLab, etc.).
