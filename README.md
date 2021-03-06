![klevr_logo.png](./src/klevr_logo.png)
# Kloud-native everywhere
## Interconnector for every SaaS delivery.
 * Asynchronous distributed infrastructure management console and agent for separated networks.
 * Supports for:
   * Baremetal server in the On-premise datacenter
   * PC/Workstation in the Office/intranet
   * Laptop at everywhere
   * Public-cloud

## Kickstart for webconsole & KVstore
* docker-compose command
```
git clone https://github.com/ralfyang/klevr.git
docker-compose up -d
```

## Diagram Overview
 * Image click to Youtube:
 * [![Diagram Overview](./src/Klevr_diagram_overview.png)](https://youtu.be/o_Ua3WhAPaU)

## Features
 * **[Agent](./agent/)**
   * Provisioning: Docker, Micro K8s, Vagrant, VirtualBox
   * Get & Run: Hypervisor(via libvirt container), Terraform, Prometheus, Beacon
   * Metric data aggregate & delivery
  * **[Web console](./webconsole/)**
   * Host pool management
   * Resource management
   * Primary host management 
   * Task management 
   * Service catalog management
   * Service delivery to Dev./Stg./Prod.
 * **Docker images**
   * [Webconsole](./Dockerfile/klevr_websonsole)(Webserver): [klevry:webconsole:latest](https://hub.docker.com/repository/docker/klevry/webconsole)
   * ~~[Beacon](./Dockerfile/beacon)(Primary agent health checker): [klevry/beacon:latest](https://hub.docker.com/repository/docker/klevry/beacon)~~
   * [Libvirt](./Dockerfile/libvirt)(Hypervisor): [klevry/libvirt:latest](https://hub.docker.com/repository/docker/klevry/libvirt)
   * Prometheus(Container monitoring)
   * Metric crawler
   * Task manager
 * **KV store([Consul](https://github.com/hashicorp/consul))**
   

## Requirement for use
 * [ ] Docker/Docker-compose/Docker-registry
   * [x] ~~Beacon~~
   * [x] Libvirt
   * [ ] Task manager to terraform
 * [ ] Terraform of container
 * [x] KVM(libvirt)
 * [ ] Micro K8s
 * [x] Consul
 * [ ] Prometheus 
 * [x] ~~Vagrant~~
 * [ ] Halm
 * [ ] Vault(maybe)
 * [ ] Packer(maybe)


