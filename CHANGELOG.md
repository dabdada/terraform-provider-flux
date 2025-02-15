# Changelog

All notable changes to this project are documented in this file.

## 0.1.1

**Release date:** 2021-03-26

This prerelease includes flux2 [v0.11.0](https://github.com/fluxcd/flux2/releases/tag/v0.11.0).

## 0.1.0

**Release date:** 2021-03-18

This prerelease includes flux2 [v0.10.0](https://github.com/fluxcd/flux2/releases/tag/v0.10.0).

## 0.0.14

**Release date:** 2021-03-17

This prerelease adds two new properties to new properties, one
for each datasource. A notable change is that the name property in
data sync no longer set the sync secret name. Instead this should
be done with the secret property.

Improvements:
* Add components extra to data sync data source
  [#115](https://github.com/fluxcd/terraform-provider-flux/pull/115)
* Make secret ref configurable
  [#113](https://github.com/fluxcd/terraform-provider-flux/pull/113)
* Add an example for GKE and Github
  [#112](https://github.com/fluxcd/terraform-provider-flux/pull/112)

## 0.0.13

**Release date:** 2021-03-09

This prerelease includes flux2 [v0.9.1](https://github.com/fluxcd/flux2/releases/tag/v0.9.1)

## 0.0.12

**Release date:** 2021-02-12

A new `toleration_keys` parameter has been added to the install
data source to enable installtion in cluster with node taints.

Improvements:
* Add tolerations parameter to install datasource
  [#96](https://github.com/fluxcd/terraform-provider-flux/pull/96)
* Fix resource name
  [#90](https://github.com/fluxcd/terraform-provider-flux/pull/90)

## 0.0.11

**Release date:** 2021-01-29

The example guides have changed to improve the upgrading experience.
The resource keys will change from being based on the content applied
to the identifier of the resource being applied. This change will
make moving from one version of Flux to another more stable.

Improvements:
* Refactor provider to reliably track changes in manifestgen output
  [#85](https://github.com/fluxcd/terraform-provider-flux/pull/85)
* Add verification and check of image versions
  [#81](https://github.com/fluxcd/terraform-provider-flux/pull/81)

## 0.0.10

**Release date:** 2021-01-15

The `arch` parameters has been removed from the `flux_install` resource
as multi-arch images are now published under the same tag.

Improvements:
* Update flux to v0.6.0
  [#77](https://github.com/fluxcd/terraform-provider-flux/pull/77)
* Add git implementation to sync datasource
  [#76](https://github.com/fluxcd/terraform-provider-flux/pull/76)
