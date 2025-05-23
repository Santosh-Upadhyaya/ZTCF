# Container Security Framework

A comprehensive framework for monitoring and securing container deployments.

## Overview

This framework provides tools and configurations for container security scanning, policy enforcement, and posture management.

## Prerequisites

- Python 3.x
- Docker
- pip (Python package manager)

## Installation

1. Download or clone the code.
```bash
https://github.com/Santosh-Upadhyaya/ZTCF.git
cd ZTCF-container
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

## Project Structure

```
ZTCF-container/
├── server.py
├── scan_docker_image.py
├── requirements.txt
└── configuration/
    ├── policy/
    └── posture/
```

## Usage

### Main Application Server

The main application server handles the core functionality of the framework.

1. Start the server:
```bash
python3 server.py
```

2. Access the application:
- Default port: 5050
- URL: `http://localhost:5050`

### Container Image Scanner

The framework includes a continuous monitoring module for scanning Docker images.

1. Run the scanner:
```bash
python3 scan_docker_image.py
```

## Configuration

All framework configurations can be customized using the files in the `configuration` directory:

- `configuration/policy/`: Security policy definitions
- `configuration/posture/`: Security posture settings

## Monitoring

https://grafana.com/docs/grafana/latest/setup-grafana/installation/docker/
https://last9.io/blog/docker-monitoring-with-prometheus-a-step-by-step-guide/

Run Grafana via Docker Compose
first go into the directory where you have created this docker-compose.yaml file

- cd ZTCF

start the grafana container
- docker compose up -d

## Testing Method

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For support and questions, please open an issue in the GitHub repository or contact the maintainers at support@containersecurity.com.
