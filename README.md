# HomeDash-RS 🏠📊

Welcome to **HomeDash-RS**, a simple and straightforward dashboard designed for your homelab, powered by Rust! This project aims to provide an easy-to-use interface for managing your home server applications like Plex, Radarr, and Sonarr. 

[![Download Releases](https://img.shields.io/badge/Download%20Releases-Click%20Here-brightgreen)](https://github.com/KrzyMrmnKlwn/homedash-rs/releases)

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **User-Friendly Interface**: Navigate easily through your homelab applications.
- **Real-Time Updates**: Get live data from your services.
- **Customizable Dashboard**: Tailor the layout to fit your needs.
- **Multi-Application Support**: Manage multiple services like Plex, Radarr, and Sonarr in one place.
- **Docker Support**: Run HomeDash-RS in a containerized environment.
- **Responsive Design**: Access your dashboard on any device.

## Technologies Used

- **Rust**: The core language for building the application.
- **React**: For building the user interface.
- **Docker**: To containerize the application.
- **Docker Compose**: For managing multi-container Docker applications.
- **Dockwatch**: To monitor and manage Docker containers.
- **Plex, Radarr, Sonarr**: Media management tools integrated into the dashboard.

## Installation

To get started with HomeDash-RS, you need to download the latest release. Visit our [Releases section](https://github.com/KrzyMrmnKlwn/homedash-rs/releases) to find the appropriate file for your system. Download and execute the file to set up the dashboard.

### Prerequisites

- Ensure you have Docker installed on your machine.
- Basic knowledge of using the command line.

### Steps to Install

1. **Download the Release**: Go to the [Releases section](https://github.com/KrzyMrmnKlwn/homedash-rs/releases) and download the latest version.
2. **Extract the Files**: Unzip the downloaded file.
3. **Run Docker Compose**:
   ```bash
   docker-compose up -d
   ```
4. **Access the Dashboard**: Open your web browser and go to `http://localhost:8080`.

## Usage

Once installed, you can access the HomeDash-RS dashboard from your web browser. The dashboard provides an overview of your services, allowing you to monitor their status and access their features directly.

### Main Features

- **Service Monitoring**: Check the status of Plex, Radarr, and Sonarr.
- **Media Management**: Add, remove, or update your media libraries.
- **Settings**: Configure your services and customize the dashboard layout.

## Configuration

You can customize HomeDash-RS to fit your specific needs. Configuration options include:

- **Environment Variables**: Set up environment variables for your Docker containers.
- **Dashboard Layout**: Modify the layout by dragging and dropping widgets.
- **Theme Options**: Choose between light and dark themes.

### Example Configuration

Here's an example of how to set environment variables in your `docker-compose.yml` file:

```yaml
version: '3'
services:
  homedash:
    image: krzymrmnklwn/homedash-rs:latest
    environment:
      - PLEX_URL=http://plex:32400
      - RADARR_URL=http://radarr:7878
      - SONARR_URL=http://sonarr:8989
    ports:
      - "8080:8080"
```

## Contributing

We welcome contributions to HomeDash-RS! If you would like to contribute, please follow these steps:

1. **Fork the Repository**: Create a copy of the repository on your GitHub account.
2. **Create a Branch**: Make a new branch for your feature or bug fix.
   ```bash
   git checkout -b feature/my-feature
   ```
3. **Make Changes**: Implement your changes and test them thoroughly.
4. **Submit a Pull Request**: Push your changes and submit a pull request to the main repository.

## License

HomeDash-RS is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For any inquiries or feedback, feel free to reach out:

- **GitHub**: [KrzyMrmnKlwn](https://github.com/KrzyMrmnKlwn)
- **Email**: contact@example.com

Thank you for checking out HomeDash-RS! We hope it enhances your homelab experience. For more updates and releases, visit our [Releases section](https://github.com/KrzyMrmnKlwn/homedash-rs/releases).