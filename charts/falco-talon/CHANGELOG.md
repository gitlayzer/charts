# Change Log

This file documents all notable changes to Falco Talon Helm Chart. The release
numbering uses [semantic versioning](http://semver.org).

## 0.5.0 - 2026-09-07

- mount the rules ConfigMap as a directory (`/etc/falco-talon/rules.d`) instead of a `subPath` file, so ConfigMap updates are propagated by kubelet and picked up by the rules watcher (`watch_rules`) — see falcosecurity/falco-talon#799

## 0.4.1 - 2026-06-15

- fix missing namespace in the Secret metadata

## 0.4.0 - 2025-05-02

- Allow specifying folder annotation for grafana dashboards

## 0.3.0 - 2024-02-07

- bump up version to `v0.3.0`
- fix missing usage of the `imagePullSecrets`

## 0.2.3 - 2024-12-18

- add a Grafana dashboard for the Prometheus metrics 

## 0.2.1 - 2024-12-09

- bump up version to `v0.2.1` for bug fixes

## 0.2.0 - 2024-11-26
- configure pod to not rollout on configmap change
- configure pod to rollout on secret change
- add config.rulesOverride allowing users to override config rules

## 0.1.3 - 2024-11-08

- change the key for the range over the rules files

## 0.1.2 - 2024-10-14

- remove all refs to the previous org

## 0.1.1 - 2024-10-01

- Use version `0.1.1`
- Fix wrong port for the `serviceMonitor`

## 0.1.0 - 2024-09-05

- First release