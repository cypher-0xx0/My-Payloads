# Bug Bounty Fuzzing Collections

A comprehensive collection of wordlists and payloads designed for bug bounty hunting, penetration testing, and security assessments. 

## 📂 Contents

Based on the repository contents (as seen in `image_56091d.png`), here is a breakdown of the available wordlists:

### API Testing
*   **`api_docs.txt`**: Common endpoints for finding API documentation (e.g., Swagger UI, OpenAPI specs).
*   **`new_api_fuzz.txt`**: Payloads and patterns specific to fuzzing modern APIs.
*   **`new_api_routes.txt`**: A list of common and standard API paths (e.g., `/api/v1/users`).

### Tech-Specific Files
*   **`asp-files.txt`**: Common `.asp` file names and paths.
*   **`aspx-files.txt`**: Common `.aspx` file names and paths.
*   **`php-files.txt`**: Common `.php` file names and paths.
*   **`wp-sensitive-dir.txt`**: Sensitive directories, configuration files, and common plugin/theme paths specific to WordPress installations.

### Discovery & Fuzzing
*   **`backup_files.txt`**: Common backup extensions (e.g., `.bak`, `.old`, `~`) and archive naming conventions.
*   **`env-files.txt`**: Payloads for discovering environment configuration files (e.g., `.env`, `docker-compose.yml`).
*   **`fuzz.txt`**: A general-purpose list for discovering hidden directories and files.
*   **`paths.txt`**: A broad list of common directory and file paths used across various web frameworks.
*   **`zip-files.txt`**: Common naming conventions for compressed archives (e.g., `backup.zip`, `source.tar.gz`).

### Parameters & Methods
*   **`http-methods.txt`**: A list of standard and non-standard HTTP methods (e.g., `GET`, `POST`, `PUT`, `TRACE`, `OPTIONS`) to test for misconfigurations or bypasses.
*   **`params.txt`**: Common parameter names used for discovering hidden inputs, testing for XSS, SSRF, or SQLi (e.g., `id`, `url`, `file`, `admin`).

### Infrastructure
*   **`resolvers.txt`**: A list of reliable DNS resolvers, useful for tools running mass DNS resolution or brute-forcing.

## 🚀 Usage

These lists can be used with popular fuzzing tools such as **ffuf**, **Gobuster**, **dirsearch**, or **Burp Suite Intruder**.

**Example using ffuf for directory discovery:**
```bash
ffuf -w paths.txt -u https://target.com/FUZZ
```
## ⚠️ Disclaimer 
* This repository is for educational purposes and authorized security testing only.
The author is not responsible for any misuse or damage caused by these files.
Always ensure you have explicit permission before testing any systems or applications.
