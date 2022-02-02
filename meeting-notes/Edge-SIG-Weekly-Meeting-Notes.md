# Centaurus - Edge + SIG Weekly Meeting
- Wednesday 3:00 - 4:00 PM
- [ZOOM](https://futurewei.zoom.us/j/93051877352?from=addon)

# 12/15

### Agenda
- Project Tracking
  - Release 1/30 items, see [project](https://github.com/CentaurusInfra/fornax/projects/2)
    - Edge communication 
      - pod to pod communication (40%)
    - Stateful Serverless 
      - stateful: Edge KV store POC (60%)
      - runtime support (WebAssembly, etc.) (70%)
  - Team allocation:
    - Shaojun: 
      - edge communication release code
        - [x] Control plane changes
        - [x] Data plane changes
        - [x] Scaled ep for edge (scraped for 1/30 release)
        - [x] Sync up edge gateway with the latest Mizar release (v0.9)
      - [ ] K3s in edge clusters (vending traffic)
    - David: 
      - [x] Edge cluster setup documentation
      - [ ] K3s in edge clusters (vending traffic)
    - Ke:
      - [ ] Research on CDN serversless solutions 
        - Blog post in writing
        - To presentation at future community meeting (time TBD)
    - Qingming:
      - CRDT based distributed storage [Anna](https://github.com/hydro-project/anna/tree/master/docs)
    - Peng:
      - Edge gateway agent release code (highest priority)
        - XDP changes & e2e flow
      - Stateful serverless
        - [x] Stateful serverless on edge talk
        - [ ] Edge serverless framework try out
          - [x] Kubeless
        - [ ] Edge serverless runtime try out
          - [ ] WASMEdge
        - [ ] Edge KV storage try out
          - [x] Anna
          - [ ] OrbitDb
        - Edge KV storage possible directions
          - CRDT & consistency fundamentals
          - CRDT based distributed KV store
          - Move data vs Move computation (regional scheduling)
          - Cross-cluster storage
          - Cross-cluster scheduling
- Scoping & Roadmap
    - Industry conferences submission
      - [ ] Deadlines for academia conference in 2022
        - Topics:
          - Edge cluster
          - Edge-edge communication
          - Performance & utilities evaluation
- Akraino Release
- Talk and outreach
  - 2nd brown bag: CRDT for A Stateful Edge (Theory, practice, edge use cases) ~ within 2 weeks
  - 3rd brown bag: [Communication & Presentation]
  - Community: 
    - UW Bothell professor to give a talk on their use cases (in 2 weeks) and possible project cooperation with grad students


# 12/22

### Agenda
- Project Tracking
  - Release 1/30 items, see [project](https://github.com/CentaurusInfra/fornax/projects/2)
    - Code track
      - Edge communication
        - Edge cluster setup documentation (100%)
        - E2E flow and agent design (100%)
        - pod to pod communication (60%)
    - Research track
      - Stateful Serverless 
        - stateful: Edge KV store research (60%), POC (30%)
  - Team allocation:
    - Shaojun: 
      - edge communication release code
        - [x] Control plane changes
        - [x] Data plane changes
        - [x] Scaled ep for edge (scraped for 1/30 release)
        - [x] Sync up edge gateway with the latest Mizar release (v0.9)
        - [x] Merge perviously POC control plane code into Mizar
        - [x] Fix Fornax Repo CI
        - [ ] Gateway agent
    - David: 
      - [x] Edge cluster setup documentation
      - [ ] K3s in edge clusters
    - Ke:
      - [x] Onboarding
      - [x] Research on CDN serversless solutions
        - Blog post in review
        - To presentation at future community meeting (time TBD)
      - Research on Serverless storage & scheduling on the Edge
    - Qingming:
      - [x] Onboarding
      - CRDT based distributed storage [Anna](https://github.com/hydro-project/anna/tree/master/docs)
    - Peng:
      - Fornax intro at TU Wien Collaboration (possible collabration on edge scheduling)  
      - Edge gateway agent release code (highest priority)
        - [x] Edge networking gateway agent e2e flow
        - [ ] Edge networking gateway XDP code

- Scoping & Roadmap
    - Industry conferences submission
      - [ ] Deadlines for academia conference in 2022
        - Topics:
          - Edge cluster
          - Edge-edge communication
          - Performance & utilities evaluation
- Akraino Release
- Talk and outreach
  - 2nd brown bag: CRDT for A Stateful Edge (Theory, practice, edge use cases) ~ within 2 weeks
  - 3rd brown bag: [Communication & Presentation]
  - Community: 
    - UW Bothell professor to give a talk on their use cases (in 2 weeks) and possible project cooperation with grad students


# 12/27

### Agenda
- Project Tracking
  - Release 1/30 items, see [project](https://github.com/CentaurusInfra/fornax/projects/2)
    - Code track
      - Edge communication
        - Edge cluster setup documentation (100%)
        - E2E flow and agent design (100%)
        - pod to pod communication
          - Control plane changes (99%)
          - XDP changes (20%)
          - user space Agent (30%)
    - Research track
      - Stateful Serverless 
        - stateful: Edge KV store research (60%), POC (30%)
      - Edge Workload Runtime
  - Team allocation:
    - Edge Communication
      - Shaojun:
        - edge communication release code
          - [x] Control plane changes
          - [x] Data plane changes
          - [x] Scaled ep for edge (scraped for 1/30 release)
          - [x] Sync up edge gateway with the latest Mizar release (v0.9)
          - [x] Merge perviously POC control plane code into Mizar
          - [x] Fix Fornax Repo CI
          - [ ] Gateway agent
      - Peng:
        - Edge gateway agent release code (highest priority)
          - [x] Edge networking gateway agent e2e flow (see slides)
          - [ ] Edge networking gateway XDP code
      - David:
        - [x] Edge cluster setup documentation
        - [ ] K3s in edge clusters
        - [ ] Gateway agent
    - Stateful storage (KV store)
      - Ke:
        - [x] Onboarding
        - [x] Research on CDN serversless solutions
          - Blog post in review
          - To presentation at future community meeting (1/10?)
        - [ ] Research on Edge KV storage
      - Peng:
        - [ ] CRDT based storage solution
    - Workload runtime
      - Qingming & Yulin
        - [ ] QuakContainer
    - Collab
      - Peng:
        - Fornax intro at TU Wien Collaboration (possible collabration on edge scheduling)  

- Scoping & Roadmap
    - Industry conferences submission
      - [ ] Deadlines for academia conference in 2022

- Akraino Release
- Talk and outreach
  - 2nd brown bag: CRDT for A Stateful Edge (Theory, practice, edge use cases) ~1/20
  - 3rd brown bag: [Communication & Presentation]
  - Community: 
    - UW Bothell professor to give a talk on their use cases (in 2 weeks) and possible project cooperation with grad students


# 1/7 2022

### Agenda
- 2022 Goals
  - Aligned with requirements (SIG, community, external collab such as TU and UWB)
  - Feature Ownership
    - One main area and one minor area per member
  - Research and POC
    - Part of the release
    - Communication at Monday meeting (research topics, paper read, feature discussion)
    - Research brown bag
  - Project exposure
    - Blog
    - Academia and industry papers
    - Local meet-up (per covid guidence)

- Project Tracking
  - Release 1/30 items, see [project](https://github.com/CentaurusInfra/fornax/projects/2)
    - Code track
      - Edge communication
        - Edge cluster setup documentation (100%)
        - E2E flow and agent design (100%)
        - pod to pod communication
          - Control plane changes (99% -> 100%)
          - XDP changes (20% -> 50%)
          - user space Agent (30% -> 40%)
    - Research track
      - Stateful Serverless 
        - stateful: Edge KV store research (80%), POC (30% -> 40%)
      - Edge Workload Runtime
        - need syncing, will join scrum
       
  - Team allocation:
    - Edge Communication
      - Shaojun:
        - edge communication release code
          - [x] Sync up edge gateway with the latest Mizar release (v0.9)
          - [x] Fix Fornax Repo CI
          - [x] Edge gateway control plane {remote subnet, gateway host in config}
          - [ ] Edge gateway metadata from user space to ebpf map on gateway host
      - Peng:
        - Edge gateway agent release code (highest priority)
          - [x] Edge networking gateway agent e2e flow (see slides)
          - [x] Edge networking gateway XDP changes (forking path on gw host)
          - [ ] Anna POC
            - [x] build anna
            - [ ] run anna
            - [ ] understand current algorithm & implementation (in C++)
      - David:
        - [x] Edge cluster setup documentation
        - [x] K3s in edge clusters
        - [x] Give a talk about KubeEdge code
        - [ ] Gateway userspace agent 
    - Stateful storage (KV store)
      - Ke:
        - [x] Research on CDN serversless solutions
          - [x] Blog post in review
          - To presentation at future community meeting (1/10?)
        - [ ] Research on Edge KV storage
    - Workload runtime
      - Qingming & Yulin
        - [ ] QuakContainer
    - Collab
      - Peng & Ke:
        - Fornax intro at TU Wien Collaboration (edge scheduling)  
        - C2C to research and work on edge cluster setup automation

- Scoping & Roadmap
    - Industry conferences submission
      - [ ] Deadlines for academia conference in 2022

- [Akraino Release blog](https://www.lfedge.org/2022/01/05/introduction-akrainos-federated-multi-access-edge-cloud-platform-blueprint-in-r5/) (Thanks Deepak and everyone else who contributed)

- Talk and outreach
  - 2nd brown bag: CRDT for A Stateful Edge (Theory, practice, edge use cases) ~1/20
  - 3rd brown bag: [Communication & Presentation]
  - Community: 
    - UW Bothell professor to give a talk on their use cases (in 2 weeks) and possible project cooperation with grad students


# 1/12 2022

### Agenda

- Project Tracking
  - Release 1/30 items, see [project](https://github.com/CentaurusInfra/fornax/projects/2)
    - Code track
      - Edge communication
        - Edge cluster setup documentation (100%)
        - E2E flow and agent design (100%)
        - pod to pod communication
          - Control plane changes (100%)
          - XDP changes (90%)
          - user space Agent (50%)
    - Research track
      - Stateful Serverless 
        - stateful: Edge KV store research (90%), POC (40%)
      - Edge Workload Runtime
        - need syncing, will join scrum (@Yulin, please invite me to the scrum for project tracking)
       
  - Team allocation:
    - Edge Communication
      - Shaojun:
        - edge communication release code
          - [x] Sync up edge gateway with the latest Mizar release (v0.9)
          - [x] Fix Fornax Repo CI
          - [x] Edge gateway control plane {remote subnet, gateway host in config}
          - [x] Edge gateway metadata from user space to ebpf map on gateway host
          - [ ] Gateway userspace agent 
      - Peng:
        - Edge gateway agent release code (highest priority)
          - [x] Edge networking gateway agent e2e flow (see slides)
          - [x] Edge networking gateway XDP changes (forking path on gw host)
          - [ ] Anna POC
            - [x] build anna
            - [ ] run anna
            - [ ] understand current algorithm & implementation (in C++)
      - David:
        - [x] Edge cluster setup documentation
        - [x] K3s in edge clusters
        - [x] Give a talk about KubeEdge code
        - [ ] Gateway userspace agent 
    - Stateful storage (KV store)
      - Ke:
        - [x] Research on CDN serversless solutions
          - [x] Blog post in review (pending Peng's section)
          - To presentation at future community meeting (1/24?)
        - [ ] Research on Edge KV storage
        - [ ] Golang, K8s, serverless runtimes
    - Workload runtime
      - Qingming & Yulin
     
    - Community Collaboration 
      - TU Wien Collaboration: scheduling roadmap
      - C2C to research and work on edge cluster setup automation (being reviewed by their team)

- Scoping & Roadmap
    - Industry conferences submission
      - [ ] Deadlines for academia conference in 2022

- Talk and outreach
  - 2nd brown bag: CRDT for A Stateful Edge (Theory, practice, edge use cases) ~1/20
  - 3rd brown bag: [Communication & Presentation]
  - Community: 
    - UW Bothell professor to give a talk on their use cases (in 2 weeks) and possible project cooperation with grad students


# 1/19 2022

### Agenda

- Project Tracking
  - Release 1/30 items, see [project](https://github.com/CentaurusInfra/fornax/projects/2)
    - Code track
      - Edge communication
        - Edge cluster setup documentation (100%)
        - E2E flow and agent design (100%)
        - pod to pod communication
          - Control plane changes (100%)
          - XDP changes (90% -> 100%)
          - User space Agent (70%), on track
            - POC to Release code change (edge gateway ingress pkt forwarding options)
    - 1/30 Research track
      - Stateful Serverless
        - stateful: Edge KV store research (90%), POC (40% -> 50%)
    - Research
      - Edge Workload Runtime
      - Edge Serverless Runtime System
 
  - Team allocation:
    - Edge Communication
      - Shaojun:
        - edge communication release code
          - [x] Sync up edge gateway with the latest Mizar release (v0.9)
          - [x] Fix Fornax Repo CI
          - [x] Edge gateway control plane {remote subnet, gateway host in config}
          - [x] Edge gateway metadata from user space to ebpf map on gateway host
          - [x] Gateway userspace agent 
      - Peng:
        - Edge gateway agent release code (highest priority)
          - [x] Edge networking gateway agent e2e flow (see slides)
          - [x] Edge networking gateway XDP changes (forking path on gw host)
          - [ ] Anna POC
            - [x] build anna
            - [ ] run anna
              - [x] single node
              - [ ] multiple node
              - [ ] in a K8s cluster
            - [x] understand current algorithm & implementation (in C++)
      - David:
        - [x] Edge cluster setup documentation
        - [x] K3s in edge clusters
        - [x] Give a talk about KubeEdge code
        - [ ] Gateway userspace agent 
    - Stateful storage (KV store)
      - Ke:
        - [x] Research on CDN serversless solutions
          - [x] Blog post in review (still pending Peng's section, ETA this Friday)
          - To presentation at future community meeting (1/24?)
        - [ ] Research on Edge KV storage
        - [ ] Golang, K8s, serverless runtimes
          - [x] K8s cluster setup
    - Workload runtime
      - Qingming & Yulin
     
    - Community Collaboration 
      - TU Wien Collaboration: scheduling roadmap (slides updated, next Tuesday)
      - C2C to research and work on edge cluster setup automation
        - [PR](https://github.com/CentaurusInfra/fornax/pull/68) in review

- Scoping & Roadmap
    - Industry conferences submission
      - [ ] Deadlines for academia conference in 2022

- Talk and outreach
  - 2nd brown bag: CRDT for A Stateful Edge (Theory, practice, edge use cases) ~early Feb
  - 3rd brown bag: [Communication & Presentation]
  - Community: 
    - UW Bothell professor to give a talk on their use cases (in 2 weeks) and possible project cooperation with grad students

# 1/27 2022

### Agenda

- Project Tracking
  - Release 1/30 items, see [project](https://github.com/CentaurusInfra/fornax/projects/2)
    - Code track
      - Edge communication
        - Edge cluster setup documentation (100%)
        - E2E flow and agent design (100%)
        - pod to pod communication
          - Control plane changes (100%)
          - XDP changes (90% -> 100%)
          - User space agent (70% -> 100%)
            - Optimization for "extra credit"
    - 1/30 Research track
      - Stateful Serverless
        - Edge storage solutions: 
          - POC (40% -> 60%)
  - Beyond 1/30 
    - Sky computing requirements for edge agent
      - Edge agent metadata P2P update
    - Fornax repo CI setup
    - Mizar repo merging
  - Long term research
      - Edge Workload Runtime
      - Edge Serverless Runtime System
 
  - Team allocation:
    - Edge Communication
      - Shaojun:
        - edge communication release code
          - [x] Sync up edge gateway with the latest Mizar release (v0.9)
          - [x] Fix Fornax Repo CI
          - [x] Edge gateway control plane {remote subnet, gateway host in config}
          - [x] Edge gateway metadata from user space to ebpf map on gateway host
          - [x] Gateway userspace agent
      - Peng:
        - Edge gateway agent release code (highest priority)
          - [x] Edge networking gateway agent e2e flow (see slides)
          - [x] Edge networking gateway XDP changes (forking path on gw host)
          - [ ] Anna POC
            - [x] build anna
            - [ ] run anna
              - [x] single node
              - [x] code deep dive 
              - [ ] multiple node
              - [ ] in a K8s cluster
            - [x] understand current algorithm & implementation (in C++)
      - David:
        - [x] Edge cluster setup documentation
        - [x] K3s in edge clusters
        - [x] Give a talk about KubeEdge code
        - [ ] Review and validate edge cluster setup scripts PR by C2C
    - Stateful storage (KV store)
      - Ke:
        - [x] Research on CDN serversless solutions
          - [x] Blog post in review (still pending Peng's section, ETA this Friday)
          - To presentation at future community meeting (1/24?)
        - [x] Research on Edge KV storage
          - [ ] IPFS deep dive (DEMO)
        - [ ] Golang, K8s, serverless runtimes
          - [x] K8s cluster setup
            - [doc](https://github.com/CentaurusInfra/fornax/wiki/Building-K8s-from-Source)
            - [Scripts](https://github.com/CentaurusInfra/fornax/tree/main/docs/setup-guide/build_k8s_from_source) 
    - Workload runtime
      - Qingming & Yulin:
        - "TCP over RDMA can work end to end"
     
    - Community Collaboration 
      - TU Wien Collaboration: scheduling roadmap (slides updated, next Tuesday)
        - Edge Intro talk at TSC meeting
        - TU meeting quick talk on scheduling (to review the final draft specification from Stefan)
      - C2C to research and work on edge cluster setup automation
        - [PR](https://github.com/CentaurusInfra/fornax/pull/68) in review

- Scoping & Roadmap
    - Industry conferences submission
      - [ ] Deadlines for academia conference in 2022

- Talk and outreach
  - 2nd brown bag: CRDT for A Stateful Edge (Theory, practice, edge use cases) ~early Feb
  - 3rd brown bag: [Communication & Presentation]
  - Community: 
    - UW Bothell professor to give a talk on their use cases (in 2 weeks) and possible project cooperation with grad students

# 2/2 2022

### Agenda

- Project Tracking
  - [Release 1/30](https://github.com/CentaurusInfra/fornax/projects/2) completed
  - [New release](https://github.com/CentaurusInfra/fornax/projects/3) (4/30?) 
    - Edge communication (Edge gateway)
      - Userspace to send packet to local XDP
      - Performance evaluation with profiling
      - Control plane metadata syncing
        - Option 1: graph algorithm
        - Option 2: ipfs
      - Sky computing rquirements (initial meeting on Friday)
    - Fornax edge cluster
      - Edge-edge communication validation (deployment of VPC, subnets on edge clusters)
      - Edge cluster setup automation
      - Repo CI setup
    - Edge storage (KV store)
      - Anna, IPFS, etc.
      - Release items to be determined
    - Edge Serverless Runtime System
      - K8s/K3s + Fornax edge cluster components + serverless framework for edge
      - Release items to be determined
    - Edge Workload Runtime (Quark)
 
  - Team:
    - Edge Communication
      - Shaojun:
        - edge communication release code
          - [ ] Edge gateway control plane
          - [ ] Edge cluster validation for edge-edge communication
      - David:
        - [ ] Review and validate edge cluster setup scripts PR by C2C
    - Stateful storage (KV store)
      - Ke:
        - [x] Research on Edge KV storage
          - [ ] IPFS deep dive (DEMO)
        - [ ] Golang, K8s, serverless runtimes
          - [x] K8s cluster setup
            - [doc](https://github.com/CentaurusInfra/fornax/wiki/Building-K8s-from-Source)
            - [Scripts](https://github.com/CentaurusInfra/fornax/tree/main/docs/setup-guide/build_k8s_from_source) 
          - [ ] K8s serverless frameworks (e.g. Kubeless)
      - Peng:
        - Edge gateway agent release code
          - Edge gateway control plane metatdata algorithms
          - Publication planning
        - [ ] Anna POC
          - [x] build anna
          - [ ] run anna
          - [x] understand current algorithm & implementation (in C++)
            - [x] CRDT Lattic templates
            - [ ] Consistent hashing tier (60%)    
      - Qingming & Yulin
     
    - Community Collaboration
      - TU Wien Collaboration: Polaris 2.0 proposal review
        - TU meeting quick talk on scheduling (to review the final draft specification from Stefan)
      - C2C to research and work on edge cluster setup automation
        - [PR](https://github.com/CentaurusInfra/fornax/pull/68) in review

- Scoping & Roadmap
    - Industry conferences submission
      - [ ] Deadlines for academia conference in 2022

- Talk and outreach
  - 2nd brown bag: CRDT for A Stateful Edge (Theory, practice, edge use cases) ~early Feb
  - 3rd brown bag: [Communication & Presentation]
  - Community: 
    - UW Bothell
