## **1. Configure your global Git settings:**  
   ```bash
   1) git config --global user.name "Your Name"

 =>git config: Starts the Git configuration process.

--global: Specifies that this setting applies globally to all repositories for the current user.

user.name: Refers to the Git configuration key for your name.

"Your Name": Sets the value of user.name to the specified name.


2)git config --global user.email "your-email@example.com"

   => git config: Starts the Git configuration process.

--global: Specifies that this setting applies globally to all repositories for the current user.

user.email: Refers to the Git configuration key for your email address.

"your-email@example.com": Sets the value of user.email to the specified email
   ```
## **2. Verify the configuration:**  
   ```bash
   1) git config --list

   => What It Does:
Lists all the Git configuration settings currently active at all levels (system, global, and local).

Displays key-value pairs of the settings (e.g., user.name=John Doe).

Purpose:
To verify that the settings for user.name and user.email were configured correctly.
Helps check other configuration settings like aliases, editor preferences, and more.
   ```