# ⚠️ Important Usage & Security Notice

- Public configs in this repository are intended **only for normal usage** such as browsing websites and social media.
- Due to **high public usage and shared access**, these configs may become unstable, rate-limited, or stop working at any time.
- For **sensitive, private, or critical activities**, you MUST:
  - Fork this repository into your own **private GitHub repository**
  - Use your **own ProtonVPN account**
  - Generate configurations tied to your **own private keys**

Personal configs generated from your private repository have a higher connection success rate and stability compared to public shared configs.

---

# 🔐 Private Setup Guide (Step-by-Step)

## 1️⃣ Fork the Repository

1. Click **Fork** (top-right corner)  
2. Set repository visibility to **Private**  
3. Create the fork  

---

## 2️⃣ Configure Required Secrets

Navigate to:

`Repository → Settings → Secrets and variables → Actions → New repository secret`

Add the following secrets:

- `VPN_USERNAME` → Your ProtonVPN username  
- `VPN_PASSWORD` → Your ProtonVPN password  

All secrets must be added exactly with the names above.

---

## 3️⃣ Run the GitHub Workflow

1. Go to the **Actions** tab  
2. Select the workflow  
3. Click **Run workflow**  
4. Start execution  

The workflow will:
- Log into ProtonVPN
- Download new WireGuard configs
- Package them into a ZIP
- Send them to your Telegram (if configured)

---

## 4️⃣ Retrieve Your Configs

After successful execution:

- `ProtonVPN_WireGuard_Configs.zip` will be generated
- It will be:
  - Committed or stored as an artifact in your repository
  - Automatically sent to your Telegram bot (if configured)

Download the ZIP, extract it, and import the `.conf` files into your WireGuard client.

---

# 🛡️ ProtonVPN WireGuard Config Auto-Fetcher

This project provides an automated solution using Python/Selenium and GitHub Actions to regularly fetch and update the latest **WireGuard** configuration files from a ProtonVPN account.

The downloaded configurations are automatically updated in this repository and are pushed to the corresponding Telegram channel for immediate access.

# 📢 Telegram Channel

All final results are automatically compressed into a ZIP file and uploaded to our Telegram channel:

🔹 **Main Channel:** [DeltaKroneckerFreedom](https://t.me/GitKroneckerDelta)  

---

## 💻 Usage Guide (Windows Focus)

These WireGuard configuration files (`.conf`) are optimized for seamless use in a Windows environment.

### 📌 Recommended Tool for Optimal Performance (Windows)

For the best performance, stability, and compatibility on Windows, it is **highly recommended** to use the following client instead of the official WireGuard application:

* **Wiresock VPN Client (Recommended)**
    * **Link:** https://www.wiresock.net

Wiresock is a robust client that supports the WireGuard protocol, offering superior performance in connection management and traffic handling on Windows systems.

### ⬇️ Accessing the Config Files:

The files are available both on the GitHub repository and through the Telegram channel.

1.  **Download Source:** Choose your preferred method:
    * **Via GitHub:** Download the file directly from this repository:
      https://github.com/Delta-Kronecker/ProtonVPN-WireGuard-configuration/raw/refs/heads/main/ProtonVPN_WireGuard_Configs.zip
    * **Via Telegram:** Download the latest ZIP file uploaded to the channel DeltaKroneckerFreedom.

2.  **Extraction:** Extract the downloaded ZIP file. The files are organized into folders by two-letter country codes (e.g., `US`, `DE`, `NL`).
3.  **Client Use:**
    * Ensure the Wiresock client is installed and running.
    * Import your desired `.conf` files from the country folders into Wiresock and connect.

## 🔥 Keep This Project Going!

If you're finding this useful, please show your support:

⭐ **Star the repository on GitHub**

⭐ **Star our [Telegram posts](https://t.me/DeltaKroneckerGithub)** 

Your stars help keep the project maintained and updated.

---
