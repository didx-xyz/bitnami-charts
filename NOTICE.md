# NOTICE

## About This Repository

This repository is a **redistribution fork** of the [Bitnami Charts](https://github.com/bitnami/charts) project. We provide unmodified, repackaged Helm charts from the official Bitnami open-source charts repository.

## What We Do

- **Sync**: Automatically sync with the upstream Bitnami charts repository
- **Package**: Create Helm chart packages from the synced chart sources
- **Publish**: Distribute charts via GitHub Container Registry at `oci://ghcr.io/{owner}/bitnami-oss-charts/`

## What We DON'T Do

- **Modify charts**: We make zero modifications to the Bitnami chart source code
- **Provide support**: We do not provide technical support for these charts
- **Develop features**: We do not add features or fix bugs

## 🚨 Important: Where to Get Help

### For Issues, Bugs, or Support

**Please open issues at the official Bitnami repository:**

👉 **<https://github.com/bitnami/charts>**

We cannot provide support for these Helm charts. All technical issues, feature requests, bug reports, and support questions should be directed to the official Bitnami team.

### For Build/Distribution Issues

If you encounter problems specifically with our automated builds or chart distribution (not the charts themselves), you may open an issue in this repository.

## License & Attribution

These Helm charts are redistributed under the **[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)**, as permitted by the original license.

### Original Work

- **Copyright**: Broadcom, Inc. All Rights Reserved
- **Original Repository**: <https://github.com/bitnami/charts>
- **License**: Apache License 2.0
- **Authors**: Bitnami Engineering Team

### This Distribution

- **Repository**: <https://github.com/didx-xyz/bitnami-charts>
- **Registry**: oci://ghcr.io/{owner}/bitnami-oss-charts/
- **Maintainer**: didx-xyz
- **Nature**: Unmodified redistribution

## Why This Fork Exists

Bitnami announced they will stop publishing open-source Helm charts to public registries after August 28, 2025, but continues to maintain the source code. This repository bridges that gap by:

1. Automatically syncing with upstream changes
2. Building and publishing the open-source charts
3. Providing OCI-compliant chart distribution
4. Maintaining proper attribution to the original authors

## Usage

### Installing Charts

```bash
# Install a chart
helm install my-release oci://ghcr.io/{owner}/bitnami-oss-charts/CHART_NAME

# Example: Install Keycloak
helm install keycloak oci://ghcr.io/{owner}/bitnami-oss-charts/keycloak

# Upgrade to latest version
helm upgrade my-release oci://ghcr.io/{owner}/bitnami-oss-charts/CHART_NAME
```

### Available Charts

This repository includes all charts from the official Bitnami charts repository, including popular applications like:

- PostgreSQL, MySQL, MongoDB
- Redis, Kafka, RabbitMQ
- Keycloak, Grafana, Prometheus
- And many more...

## Disclaimer

- These charts are **unofficial redistributions**
- We are **not affiliated** with Bitnami, VMware, or Broadcom
- These charts are **not supported** by Bitnami
- Use at your own risk
- For production use, consider Bitnami's official commercial offerings

## Chart Modifications

Charts are packaged as-is from the upstream repository. However, when the `rewrite_dependencies` workflow option is enabled:

- Chart dependencies pointing to Bitnami registries are updated to use this registry
- This ensures charts continue to work after Bitnami stops publishing
- Original chart functionality remains unchanged

## Trademarks

Bitnami is a trademark of VMware, Inc. or its affiliates. Use here is for identification purposes only and does not imply endorsement.

## Legal Compliance

This redistribution complies with the Apache License 2.0 terms:

- ✅ Original license and copyright notices preserved
- ✅ Original authors properly attributed
- ✅ No modifications made to chart source code
- ✅ Clear indication this is a redistribution
- ✅ Same license terms apply

---

Thank you to the Bitnami team for their excellent work on these Helm charts! 🙏
