# Centaurus - Edge + SIG Weekly Meeting
- Wednesday 3:00 - 4:00 PM
- [ZOOM](https://futurewei.zoom.us/j/93051877352?from=addon)

# 9/29

### Agenda
- Overall status
  - Project tracks:
    - Release
      - [ ] 930 release "Inter-cluster communication"
        - Edge-edge communication
          - Automated dev env setup for Qian and David
          - POC/Dev
            - Pod traffic e2e (to use proxy as gateway) (70%)
              - [x] Mizar control plane changes for gateway host
              - [x] Mizar data plane to 
                  1. [x] route traffic to user space on gateway host
                  2. [x] avoid ep_host_cache on divider when traffic comes from the gateway host
              - [ ] connect 2nd cluster and perform e2e test
            - Detailed gateway design, 930 release
      - New release brainstorming (next week after 27th)
  - Exposures
    - [x] OSS tutorial talk 9/27
- "Macro trend" discussion (due by 10/31)
  - 5G application
  - Cloud-cloud vs Cloud-edge
  - Serverless
  - Paper reading
    - Deep Learning With Edge Computing- A Review
    - Adaptive Federated Learning in Resource Constrained Edge Computing Systems
    - Edge Intelligence- Paving the Last Mile of Artificial Intelligence With Edge Computing
    - The Emerging Landscape of Edge-Computing
- Onboarding
- Akraino Release
  - documentation owner settled
- Notes:
  - [Edge gallery for 5G](https://gitee.com/organizations/edgegallery/projects)


# 10/06

### Agenda
- Overall status
  - Project tracks:
    - Release
      - [x] 930 release
        - Edge-edge communication
      - New release brainstorming (next week)
  - Exposures
    - [x] KubeCon virtual booth slides tutorial talk 9/27
- "Macro trend" discussion (due by 10/31)
  - 5G application
  - Cloud-cloud vs Cloud-edge
  - Serverless
  - [Edge gallery for 5G MEC](https://gitee.com/organizations/edgegallery/projects)
  - Paper reading
    - [ ] Deep Learning With Edge Computing- A Review
    - [ ] Adaptive Federated Learning in Resource Constrained Edge Computing Systems
    - [ ] Edge Intelligence- Paving the Last Mile of Artificial Intelligence With Edge Computing
    - [ ] The Emerging Landscape of Edge-Computing
- [x] Onboarding


# 10/20

### Agenda
- Overall status
  - Project tracks:
    - edge-edge communication XDP direct ping succeeded
    - myth of direct path resolved
    - "Edge Gateway" -> "Edge Portal"
  - New release planning
    - Recent conference sync-ups (ONE, KubeCon)
    - Edge network provisioning (deployment+)
    - Edge service discovery (pod migration, edge portal system control plane)
    - Exteand the AI face recognition program to multiple-cluster
    - Federated learning showcase
    - Edge benchmarking
- "Macro trend" discussion (due by 10/31)
  - 5G application
  - Cloud-cloud vs Cloud-edge
  - Serverless
  - [Edge gallery for 5G MEC](https://gitee.com/organizations/edgegallery/projects)
  - Paper reading
    - [ ] Deep Learning With Edge Computing- A Review
    - [ ] Adaptive Federated Learning in Resource Constrained Edge Computing Systems
    - [ ] Edge Intelligence- Paving the Last Mile of Artificial Intelligence With Edge Computing
    - [ ] The Emerging Landscape of Edge-Computing
- Akraino Release
  - [ ] log uploads?

### notes
- Serverless on the edge
- Distributed storage (distributed data bus across edge) "Ceph across edge", on top of edge-edge


# 10/20

### Agenda
- Overall status
  - Project tracks:
    - Qian: 
      - Research on [Submariner](https://github.com/submariner-io/submariner), [talk video](https://www.youtube.com/watch?v=fMhZRNn0fxQ)
      - Edge gateway agent POC & Dev
    - Shaojun: Control plane changes (POC code -> release code)
    - David: Testing, dev environment to catch up Mizar newest release)
    - Peng: 
      - Roadmap & landscape planning
      - Edge gateway initial release design
      - team support
- "Macro trend" & Roadmap (due by 10/31)
  - Edge team vision (slides)
  - Field scoping
    - Existing & Promising Solution
      - [x] [Edge gallery for 5G MEC](https://gitee.com/organizations/edgegallery/projects)
    - Academia Papers
      - [x] The Emerging Landscape of Edge-Computing
      - [x] Edge Intelligence- Paving the Last Mile of Artificial Intelligence With Edge Computing (60%)
      - [x] Adaptive Federated Learning in Resource Constrained Edge Computing Systems
      - [ ] Deep Learning With Edge Computing- A Review
    - Industry Conferences
      - "Global edge computing conference"
        - Short term vs long term
    - 5G & MEC
      - ETSI doc on 5G scenario
        - ["MEC in 5G networks"](https://www.etsi.org/images/files/ETSIWhitePapers/etsi_wp28_mec_in_5G_FINAL.pdf)
        - ["Mobile-Edge Computing (MEC) Service Scenarios"](https://www.etsi.org/deliver/etsi_gs/mec-ieg/001_099/004/01.01.01_60/gs_mec-ieg004v010101p.pdf)

- Akraino Release
  - [ ] log issue fix



