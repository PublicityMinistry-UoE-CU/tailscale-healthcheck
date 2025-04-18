# Tailscale Healthcheck 🚀

![Tailscale Healthcheck](https://img.shields.io/badge/Tailscale%20Healthcheck-v1.0.0-brightgreen)

Welcome to the **Tailscale Healthcheck** repository! This Python-based Flask application monitors the health of devices in a Tailscale network. With it, you can easily check the health status of all devices, specific devices, and get lists of healthy or unhealthy devices.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Endpoints](#endpoints)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)
- [Links](#links)

## Features

- **Device Monitoring**: Check the health status of all devices in your Tailscale network.
- **Specific Device Check**: Query the health status of individual devices.
- **Health Lists**: Retrieve lists of healthy and unhealthy devices.
- **Docker Support**: Easily deploy the application using Docker.
- **Lightweight**: Built with Flask for quick responses and minimal resource usage.

## Installation

To get started, clone the repository and install the required packages.

```bash
git clone https://github.com/PublicityMinistry-UoE-CU/tailscale-healthcheck.git
cd tailscale-healthcheck
pip install -r requirements.txt
```

Alternatively, you can use Docker to run the application:

```bash
docker build -t tailscale-healthcheck .
docker run -p 5000:5000 tailscale-healthcheck
```

## Usage

After installation, you can start the Flask application by running:

```bash
python app.py
```

Visit `http://localhost:5000` in your web browser to access the application.

## Endpoints

The application provides several endpoints to monitor device health:

- **Get All Devices Health Status**
  - **Endpoint**: `/api/devices`
  - **Method**: GET
  - **Description**: Returns the health status of all devices.

- **Get Specific Device Health Status**
  - **Endpoint**: `/api/devices/<device_id>`
  - **Method**: GET
  - **Description**: Returns the health status of a specific device.

- **Get Healthy Devices**
  - **Endpoint**: `/api/devices/healthy`
  - **Method**: GET
  - **Description**: Returns a list of healthy devices.

- **Get Unhealthy Devices**
  - **Endpoint**: `/api/devices/unhealthy`
  - **Method**: GET
  - **Description**: Returns a list of unhealthy devices.

## Configuration

You can configure the application by modifying the `config.py` file. Here, you can set parameters such as:

- **Tailscale API Key**: Your Tailscale API key for authentication.
- **Polling Interval**: How often the application checks device health.

## Contributing

We welcome contributions! If you want to help improve the Tailscale Healthcheck application, please follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/YourFeature`.
3. Make your changes and commit them: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature/YourFeature`.
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Links

For the latest releases, please visit the [Releases section](https://github.com/PublicityMinistry-UoE-CU/tailscale-healthcheck/releases). You can download and execute the latest version from there.

![Release Button](https://img.shields.io/badge/Latest%20Releases-Download%20Now-blue)

For further information, check the [Releases section](https://github.com/PublicityMinistry-UoE-CU/tailscale-healthcheck/releases) to stay updated.

---

Thank you for checking out Tailscale Healthcheck! Your feedback and contributions are valuable to us. Let's make device monitoring simple and effective together!