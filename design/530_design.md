# Centaurus Edge Design

## Abstract
The prosperity of cloud technologies, 5G and AI brings vast opportunities for edge computing where computation migrates from centralized data centers to on-prem, at-home, and remote areas. This document introduces a novel edge-computing framework design for Centaurus. Observing and honoring the requirements specific to edge environments, e.g. low latency, high survivability, and hierarchically distributed architecture, this design features 
1. running clusters on the edge, alongside with edge nodes,
2. flexible topologies where edge clusters are connected in multi-layer tree-like structures 
3. flexible flavored clusters on the edge, such as K8s and K3s, 
4. inter-cluster communication capability and, 
5. smart edge cluster formation. 

## Scenarios

- IoT, where devices such as temperature sensors and surveillance cameras are connected to edge nodes.
- Smart Factory, where cluster of nodes run on the edge site
- Multi-access edge computing (MEC), where edge nodes and/or edge applications run on edge nodes or clusters places in or close to cellular network

## Requirements 

Edge computing environments have the following key differences comparing to the cloud environments:

- Low computing power

- Low energy suply and consumption

- Unstable network connection

- Smaller or no dev-ops teams
 
## Design Principles

Centaurus edge addresses the requirements by allowing workloads on the edge to continue functioning with tolerance to the following conditions: 

1. Network disconnect

2. Edge node failure 

3. Both 1. and 2. happen Simultaneously 

Altogether, Centaurus edge is designed to run applications with the best effort against environment fluctuation and uncertainties. 

## Existing Solutions

### IoT

These solutions provide functions to manage computing nodes running on the edge environments. The control plane sits in the cloud, and an "agent" type of software components is deployed on the edges node to allow edge nodes to continue running when network disconnects. The existing solutions includes:

- [KubeEdge](https://github.com/kubeedge/kubeedge)
- [OpenYurt](https://github.com/openyurtio/openyurt)
- [SuperEdge](https://github.com/superedge/superedge)
- [BAETYL](https://github.com/baetyl/baetyl)

THese solutions meet condition 1 of the design principles.  

### Edge cluster 

These solutions have the control plane including apiserver, controllers and scheduler in the edge sites. The existing solutions includes:

- [Kubefed](https://github.com/kubernetes-sigs/kubefed)
- [Karmada](https://github.com/karmada-io/karmada)
- [TKEStack](https://github.com/tkestack/tke)
- [Cluster-registry](https://github.com/kubernetes-retired/cluster-registry), retired
- [Namespace Sameness](https://github.com/kubernetes/community/blob/master/sig-multicluster/namespace-sameness-position-statement.md)




## Models

### Single-layer vs Hierarchy

### Layered and Hierarchical Topology

## Key Features

### Robust Edge Clusters

### Flexible Edge Cluster Structure

#### Cascading Cluster

#### Supporting Multiple K8s Flavors

#### Attachment vs Self-Organizing

#### Workload Assignment

#### Status Reporting

### Inter-cluster Communication

### Autoumous Cluster Provisioning

### Modular Edge Agents

## Proof Of Concept

### Edge Cluser

### Cascading

### Status Reporting

### Flavor supports

