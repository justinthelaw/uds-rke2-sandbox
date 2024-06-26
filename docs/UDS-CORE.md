# UDS Core

<!-- TODO: renovate setup -->
**Supported Version**: 0.22.0

> [!CAUTION]
> UDS Core will not deploy or function properly unless deployed as part of a UDS bundle with the proper overrides applied.

## UDS Core Overrides

### S3 Bucket

The S3 bucket being used by the UDS Core services, Loki and Velero, are pointed to the MinIO or ROok-Ceph bucket generated by default using the custom Zarf Init.

### CoreDNS

The CoreDNS service identified by the Loki Gateway must be pointed to the pre-packaged `rke2-coredns` service.

### Custom TLS Certificates

Each Istio Ingress/Egress gateway must have a valid TLS certificate. Options to point to a pre-populated certificate are provided.
