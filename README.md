# IndexNow Submitter - A Powerful Desktop Tool for Instant Indexing

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/[Your-GitHub-Username]/IndexNow-Submitter)
[![.NET Framework](https://img.shields.io/badge/.NET_Framework-4.7.2-blueviolet.svg)](https://dotnet.microsoft.com/en-us/download/dotnet-framework)

**A feature-rich Windows desktop application to instantly submit your website's URLs to the IndexNow API, ensuring rapid discovery by search engines like Bing, Yandex, and more.**

Tired of waiting for search engines to crawl and index your new or updated content? The IndexNow Submitter provides a simple, powerful, and user-friendly interface to directly notify search engines, improving your SEO performance by getting your content indexed in minutes, not days.



---

## ✨ Key Features

This tool is packed with features designed for both beginners and power users:

* **Multiple Submission Modes:**
    * **Sitemap:** Fetch all URLs directly from your `sitemap.xml`.
    * **File:** Load a list of URLs from a local `.txt` file (one URL per line).
    * **Individual:** Paste one or more URLs directly into the application.
* **Complete API Key Management:**
    * **Generate Key:** Create a new, secure 32-character API key with a single click.
    * **Verify Key:** Check if your API key and its location on your server are correctly configured.
    * **Extract Key:** Automatically fetch and fill the API key from its web location.
* **Efficient URL Handling:**
    * **Bulk Selection:** Use the "Select All / Deselect All" checkbox to manage large lists of URLs.
    * **Save URL List:** Export your selected URLs to a `.txt` file for backup or record-keeping.
* **Robust Project Management:**
    * **Save & Open Projects:** Save your settings (API Key, Key Location, Sitemap URL) to a project file, so you don't have to re-enter them every time.
* **Detailed Feedback & Logging:**
    * Get clear success or failure messages for every action.
    * The status bar provides real-time updates on the current process.
    * On submission failure, the application displays the **exact error response** from the IndexNow API for easy troubleshooting.
* **Dynamic UI:** The interface adapts to your needs, such as resizing the textbox for single or multi-line URL input.

---

## ⚙️ Requirements

* **Windows Operating System** (7, 8, 10, 11)
* **.NET Framework 4.7.2 or higher** (This is typically pre-installed on modern Windows systems).

---

## 📥 Installation & Usage

1.  Navigate to the **[Releases](https://github.com/[Your-GitHub-Username]/IndexNow-Submitter/releases)** page of this repository.
2.  Download the latest `.zip` file (e.g., `IndexNow.Submitter.v1.0.0.zip`).
3.  Extract the contents of the zip file to a folder on your computer.
4.  Run `IndexNowSubmitter.exe`. No installation is required.

---

## 📖 Detailed Walkthrough

The application is organized into three simple tabs for different submission methods.

### 1. Submit Using Sitemap
This is the most powerful mode for submitting your entire site.

* **Sitemap URL:** Enter the full URL to your `sitemap.xml` file.
* **Fetch Sitemap:** Click to download and display all URLs from the sitemap in the "Fetched URL" list.
* **API Key:** Your unique 32-character key.
* **Generate API Key:** Creates a new, random key for you.
* **Key Location:** The full URL on your website where the key file is hosted (e.g., `https://yourdomain.com/your-api-key.txt`).
* **Verify:** Checks if the key file at the Key Location exists and contains the correct API Key.
* **Extract From Key Location:** Fetches the content from the Key Location URL and places it in the API Key field.
* **Fetched URL List:** All URLs are loaded here. You can manually check or uncheck them.
* **Action Buttons:**
    * `Save As Project`: Saves your API Key, Key Location, and Sitemap URL for later use.
    * `Open Project`: Loads a previously saved project.
    * `Submit To IndexNow`: Submits all **checked** URLs to the IndexNow API.

### 2. Submit Using File
Ideal for submitting a custom list of URLs.
* **Load From File...:** Opens a dialog to select a `.txt` file. The file should contain one URL per line.
* The application will load all valid URLs from the file into the list, ready for submission.
* The API Key, Key Location, and Action buttons work the same way as the Sitemap tab.

### 3. Submit Individual URL
The quickest way to submit one or just a few URLs.
* **Multiline Input:** Use the radio buttons to toggle the textbox between a single-line and a multi-line view, complete with scrollbars.
* Simply paste your URL(s) into the box (one per line if in multi-line mode).
* Fill in your API details and click the submit button.

---

## ☁️ (Optional) Advanced Setup: Using the Cloudflare Worker

For users who don't want to manually upload a key file via FTP, you can deploy a free Cloudflare Worker to handle key hosting and generation automatically.

<details>
  <summary>Click to view Cloudflare Worker setup instructions</summary>
  
  ### What it Does
  This script, when deployed, creates two endpoints on your domain:
  1. `https://your.domain/indexnow/generate`: Generates a new API key.
  2. `https://your.domain/indexnow/YOUR_KEY`: Acts as the key file itself.

  ### How to Deploy
Read article on NarendraDwivedi.Org 
---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE.md) file for details.

---

## 🙏 Acknowledgments

* This tool was built to simplify the process of using the powerful **IndexNow** protocol.
* Built with Visual Basic .NET and the Newtonsoft.Json library.

---

Created with ❤️ by **Narendra Dwivedi**. Find me on [LinkedIn](https://linkedin.com/in/narendradwivedi) or at my [Website](https://www.narendradwivedi.org).
