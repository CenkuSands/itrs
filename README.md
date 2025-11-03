# Kustomize Configuration for Netprobe

This directory contains a Kustomize configuration for deploying Netprobe in Kubernetes.

## Structure

- `base/`: Base Kustomize configuration
- `overlays/`: Environment-specific overlays
  - `daemonset/`: DaemonSet deployment
  - `statefulset/`: StatefulSet deployment

## Usage

To deploy using the DaemonSet overlay:

```bash
kubectl apply -k overlays/daemonset
```

To deploy using the StatefulSet overlay:

```bash
kubectl apply -k overlays/statefulset
```

## Configuration

The configuration is generated from the Netprobe Helm chart and includes all necessary resources for deployment.