# Change log

## [0.6.0] - 2024-12-19

- Update OSRM to version 6.0.0. This major release includes:
  - Obstacle Support: Generic support for obstacles enhances routing flexibility
  - Pedestrian Routing: Routes now include highways marked as platforms
  - Performance Boosts: Micro-optimizations improve API performance across Route, Table, Trip, and Match
  - Modernized Build System: Upgraded to Clang 15, Conan 2.x, and Debian Bookworm for better compatibility
  - NodeJS Updates: Transitioned to Node-API, dropping support for older Node versions
  - Enhanced Testing: Comprehensive CI updates and new unit tests ensure reliability

## [0.5.0] - 2022-06-07

- Update Ingress to `networking.k8s.io/v1`. Note that this requires Kubernetes API v1.19+.

## [0.4.1] - 2020-09-08

- Set Ingress apiVersion to `networking.k8s.io/v1beta1` if supported.

  **NOTE:** the change itself is not breaking, however, it may cause a small downtime on `helm upgrade`.

- Add `extraLabels` option to Ingress.

## [0.4.0] - 2020-02-28

- Add a new map source provider: Google Cloud Storage. This allows downloading maps
from gcs bucket.
- Add versioning support for HTTP source provider.
- Add [examples](examples/) of OSRM deployments with various options.

## [0.3.0] - 2020-02-26

- **BREAKING:** map configuration in `values.yaml` changed, see [diff]() to migrate.
- Expose more configuration options: extra volumes, init container, etc.

## [0.2.0] - 2020-01-22

- Add `extraArgs` option to provide additional arguments to osrm.

## [0.1.0] - 2020-01-21

First public release.
