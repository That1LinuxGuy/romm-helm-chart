# RomM Helm Chart Repository

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Helm Version](https://img.shields.io/badge/Helm-v3-blue)](https://helm.sh)
[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/romm-helm-chart)](https://artifacthub.io/packages/search?repo=romm-helm-chart)

This repository contains my  Helm chart implementation for deploying [RomM](https://romm.app/) on Kubernetes.

## Quick Start

### Add Helm Repository

```bash
helm repo add romm https://That1LinuxGuy.github.io/romm-helm-chart/
helm repo update
```

### Install Chart

```bash
helm install romm romm/romm
```

For detailed installation instructions and configuration options, see the [chart README](chart/README.md).

## Repository Structure

```
.
├── chart/              # Helm chart for RomM
│   ├── Chart.yaml      # Chart metadata
│   ├── values.yaml     # Default configuration values
│   ├── README.md       # Detailed chart documentation
│   └── templates/      # Kubernetes manifest templates
├── LICENSE             # Repository license
└── README.md           # This file
```

## Documentation

- **[Chart Documentation](chart/README.md)** - Complete installation and configuration guide
- **[RomM Official Docs](https://romm.app/)** - RomM application documentation
- **[Values Reference](chart/values.yaml)** - All available configuration options

## Prerequisites

- Kubernetes 1.19+
- Helm 3.0+
- MariaDB/MySQL database (only use built in DB for test workloads)
- Persistent storage (NFS, local-path, or cloud storage)
- (Optional) Ingress controller
- (Optional) cert-manager for automatic TLS

## Features

This Helm chart provides:

- ✅ Built-in MariaDB support (optional)
- ✅ Persistent volume management
- ✅ Ingress configuration with TLS support
- ✅ Resource limits and requests
- ✅ Health checks and probes
- ✅ ConfigMap and Secret management
- ✅ Service configuration

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request, submit and issue, or send me an email!

## License

This Helm chart is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

The RomM application itself is licensed under its own terms. See the [RomM repository](https://github.com/rommapp/romm) for more information.

## Support

- 🐛 [Report Issues](https://github.com/That1LinxGuy/romm-helm-chart/issues)
- 💬 [Discussions](https://github.com/That1LinuxGuy/romm-helm-chart/discussions)
- 📖 [Documentation](chart/README.md)

Made with ❤️ for the retro gaming community
