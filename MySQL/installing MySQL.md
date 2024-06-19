Steps for installing and configuring the MySQL database:

#   1. Download MySQL Installer
1. Open your web browser and go to the [official MySQL downloads page](https://dev.mysql.com/downloads/installer/).
2. Click on **MySQL Installer for Windows**.
3. Choose the **Windows (x86, 32-bit), MSI Installer** and click on **Download**. You may be prompted to log in or sign up for an Oracle account, but you can choose to click on **No thanks, just start my download**.

#   2. Run the MySQL Installer
1. Once the download is complete, locate the downloaded file (it should be named something like `mysql-installer-community-<version>.msi`) in your Downloads folder.
2. Double-click the installer to run it.

#    3. Choose Setup Type
1. Choose Setup Type:
   - When the installer starts, you will see various setup types. Choose **Custom** to select the components you want to install, or you can choose **Developer Default** to install all the components commonly used for development.
   - Click **Next**.

#    4. Select Products and Features
1. In the **Select Products and Features** window, ensure that **MySQL Server**, **MySQL Workbench**, and other desired tools are selected.
2. Click **Next**.

#    5. Check Requirements
1. The installer will check for any missing requirements. If all requirements are met, click **Next**. If not, follow the instructions to install any missing requirements.

#    6. Installation
1. Click on **Execute** to start the installation of the selected components.
2. Wait for the installation to complete, then click **Next**.

#    7. Configuration
1. High Availability:
   - Choose **Standalone MySQL Server** (default) and click **Next**.

2. Type and Networking:
   - Select **Config Type** as **Development Machine**.
   - Ensure the **Port Number** is set to **3306**.
   - Click **Next**.

3. Authentication Method:
   - Choose the authentication method. It is recommended to use the **Strong Password Encryption** for better security.
   - Click **Next**.

4. Accounts and Roles:
   - Set the **Root Password**. Remember this password as you will need it to log in to MySQL.
   - Optionally, you can add more user accounts.
   - Click **Next**.

5. Windows Service:
   - Ensure **Configure MySQL Server as a Windows Service** is checked.
   - Set the **Service Name** (default is `MySQL`).
   - Choose **Start the MySQL Server at System Startup**.
   - Click **Next**.

6. Apply Configuration:
   - Click on **Execute** to apply the configuration settings.
   - Once the configuration is complete, click **Finish**.

#    8. Complete the Installation
1. The installation is now complete. Click **Finish** to exit the installer.

#    9. Verify the Installation
1. Open Command Prompt or PowerShell:
   - Press `Win + R`, type `cmd`, and press Enter to open Command Prompt.
   - Alternatively, you can press `Win + R`, type `powershell`, and press Enter to open PowerShell.

2. Log in to MySQL:
   - In the Command Prompt or PowerShell, type the following command and press Enter:
     ```sh
     mysql -u root -p
     ```
   - Enter the root password you set during the installation.
   - You should now be logged into the MySQL shell.

#    10. Optional: Using MySQL Workbench
1. Open MySQL Workbench:
   - You can use MySQL Workbench to manage your MySQL databases through a graphical interface.
   - Open MySQL Workbench from the Start Menu.

2. Create a New Connection:
   - Click on the **+** symbol next to **MySQL Connections**.
   - Fill in the connection details (Connection Name, Hostname, Port, Username, etc.).
   - Test the connection and click **OK**.
