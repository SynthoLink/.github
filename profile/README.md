# SynthoLink

⚠️ This project is a work in progress ⚠️

## Overview

SynthoLink is a lightweight and versatile file synchronization tool designed for discrete file synchronization between multiple clients. Unlike traditional cloud storage services such as OneDrive, Google Drive, or Nextcloud, SynthoLink focuses on syncing individual files dispersed throughout your system in real time. It operates as a background service, ensuring seamless and automatic synchronization of designated files across connected devices.

## Key Features

- **Discrete File Sync:** SynthoLink allows you to sync individual files rather than entire folders, providing flexibility in selecting and syncing specific configurations, system files, blobs, etc.

- **Automatic Background Sync:** The synchronization process runs in the background as a service, ensuring that your files are kept up to date without manual intervention.

- **Custom TCP Protocol:** SynthoLink utilizes a custom TCP protocol, which is well-documented and open-source. This custom protocol optimizes file synchronization, providing efficient and reliable data transfer between the server and clients.

- **SSL/TLS Encryption:** All communications between the server and clients are encrypted using SSL/TLS, ensuring the security and confidentiality of your information during transmission.

- **AES 256 Encryption:** File contents are encrypted using the advanced encryption standard (AES) with a 256-bit key, adding an extra layer of security to your synchronized files.

- **Diffie-Hellman Key Exchange:** SynthoLink uses the Diffie-Hellman key exchange protocol for syncing client keys securely, enhancing the overall security of the synchronization process.

- **OAuth for Client Authentication:** Client authentication is implemented using OAuth, ensuring secure and authorized access to the SynthoLink server.

## Getting Started

To use SynthoLink, follow these steps:

1. **Install SynthoLink Server:** Set up the SynthoLink server on a dedicated machine or cloud instance. Refer to the [server documentation](docs/server.md) for installation instructions.

2. **Install SynthoLink Client:** Install the SynthoLink client on each device you want to synchronize. Refer to the [client documentation](docs/client.md) for installation instructions.

3. **Configure Synchronization:** Configure the files and directories you want to synchronize by editing the SynthoLink configuration file on each client.

4. **Start the SynthoLink Service:** Start the SynthoLink service on each client, and your files will be automatically synchronized in real time.

## Documentation

For detailed information on how to install, configure, and use SynthoLink, refer to the [official documentation](docs/index.md).

## Possible use-cases

## SynthoLink: Use Cases and Comparisons

### Personal Use:
||Use-case|Comparison|
|---|---|---|
|Configuration Sync|Synchronize configuration files across personal devices.|Unlike cloud storage services that sync entire folders, SynthoLink lets you choose specific configuration files to sync, ensuring consistency across different environments.|
|Selective File Sync|Share specific files between personal devices, e.g., documents, scripts, or photos.|Provides granular control over file syncing compared to traditional cloud services, allowing you to sync only the files you need.|
|Cross-Platform Sync|Sync files between different operating systems seamlessly.|Offers cross-platform compatibility, ensuring that files are synchronized irrespective of the underlying operating system.|

### Enterprise Use:

||Use-case|Comparison|
|---|---|---|
|Distributed Configurations|Synchronize configuration files across servers in a distributed system.|Ideal for managing configurations in server environments where discrete file synchronization is crucial for system consistency.|
|Collaborative Content Sharing|Share specific project-related files among team members.|Provides a focused and efficient way to collaborate on specific files without the need to sync entire project folders.|
|Security and Compliance|Ensure secure file synchronization in compliance with industry regulations.|Utilizes SSL/TLS encryption, AES 256 encryption for file contents, and OAuth for client authentication, enhancing security compared to some traditional cloud services.|
|Auditable|The security department of your company can audit the project.|Since it's 100% open-source, the security experts at your company can audit the code and even suggest changes!|

### Comparison with Alternatives:

- SynthoLink Offers granular control over file syncing, enabling the synchronization of individual files dispersed throughout the system. Automatic background synchronization ensures real-time updates.
- It provides a similar versioning approach as a bare Git repository but focuses on automatic background synchronization of discrete files, making it suitable for non-code assets and configurations.
- It targets selective file synchronization rather than syncing entire folders. Custom TCP protocol optimizes data transfer, and encryption measures ensure secure transmission.

## Contributing

We welcome contributions from the community. If you find a bug, have an enhancement suggestion, or would like to contribute code, please check our [contribution guidelines](CONTRIBUTING.md).

---

**Note:** This README provides a high-level overview of SynthoLink. For detailed information, please refer to the documentation included in the project repository.
