# Solana Wallet Brute Force Tool: Security Research & Exploration

**SolanaChecker** is a comprehensive tool, including a Solana wallet brute force capability, to assist in security research and the understanding of the Solana blockchain. *Please use this tool responsibly.* This is a powerful tool designed for advanced users.

<p align="left">
    <img src="/files/vision.webp" />
</p>

## Program Features: Including Brute Force Functionality

1. **Check Solana Address Balance**  
   Easily verify Solana balances. Quickly see if your address is holding the expected amount.

   
<p align="left">
    <img src="/files/side.webp" />
</p>

2. **Check Solana Tokens for Fraud**  
   Analyze token security. Protect yourself from potentially fraudulent projects.

<p align="left">
    <img src="/files/prompt.webp" />
</p>

3. **Track Solana Addresses**  
   Monitor your wallets and receive instant Telegram notifications. Stay informed on activity.

4. **Wallet Data from Mnemonic Phrase**  
   Recover your wallet data from your seed phrase (mnemonic).

	
<p align="left">
    <img src="/files/executable.webp" />
</p>

5. **Generate a Single Solana Wallet**  
   Generate new wallets with unique keys.

<p align="left">
    <img src="/files/bright.webp" />
</p>

6. **Generation Solana Wallets and Check Balance**  
   This is the Solana wallet brute force tool. Randomly generates seed phrases and checks for balances. Results are logged to a file and can be sent to Telegram. *USE WITH EXTREME CAUTION.*

<p align="left">
    <img src="/files/log.webp" />
</p>

## Setting up Telegram for Alerts

Configure Telegram notifications to receive alerts. Enter your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file.

## Getting Started with the Brute Force Tool

Download the pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project - The Technical Process

Build this project by installing these dependencies. **vcpkg** is recommended for easy dependency management.

### Installing Dependencies Using vcpkg:

1.  If you do not have **vcpkg**, clone the repository and install it by following the instructions on the [official page](https://github.com/microsoft/vcpkg).

2.  Add **vcpkg** to your system's PATH environment variable.

3.  Install dependencies:

    -   Install **OpenSSL**:
        ```bash
        vcpkg install openssl
        ```

    -   Install **nlohmann-json**:
        ```bash
        vcpkg install nlohmann-json
        ```

    -   Install **Crypto++**:
        ```bash
        vcpkg install cryptopp
        ```

    -   Install **libsodium**:
        ```bash
        vcpkg install libsodium
        ```

4.  Build the project in Visual Studio or using your preferred C++ compiler.

### Building in Visual Studio:

1.  Open the project solution.
2.  Ensure **vcpkg** is correctly integrated (see instructions on [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be located in the `bin` folder.

### Building with a C++ Compiler:

1.  Verify that all dependencies are installed via **vcpkg**.
2.  Compile using the following command:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line and the Brute Force Tool

Use these commands:

1.  **-s / -search**  
    Run the brute force function (use with EXTREME CAUTION). This generates seed phrases.

2.  **-t / -track (ADDRESS)**
	Track a specific address.

3.  **-g / -gen (NUMBER)**
	Generate wallets.

4.  **-m / -mnemonic (MNEMONIC)**
	Extract wallet info from a seed phrase.

5.  **-b / -balance (ADDRESS)**
	Check the balance.
	

## Important: Safety & Ethical Guidelines

-   Use the tool responsibly and *only* for authorized security research.
-   *NEVER* use this tool for illegal purposes.
-   Always protect your seed phrases.
-   Understand the risks.
-   Keep your software updated.

## License

This project is licensed under the [MIT License](/LICENSE). You are free to use, modify, and distribute the code in accordance with the terms of the license.



Update: url is active and operational