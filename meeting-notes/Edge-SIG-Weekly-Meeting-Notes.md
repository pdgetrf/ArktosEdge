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


# 10/27

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
- "Macro trend" & Roadmap
  - Fornax goals review (slides)
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
- 2nd brown bag
  - Communication & presentation

# 11/10

### Agenda
- Overall status
  - Release 1/30 items
    - Edge-edge communication
      - VPC, subnet deployment through edge clusters
      - Service/scaled endpoint based edge networking (POC)
    - Edge storage & serverless scoping and initial design
    - Edge scheduler scoping
  - Team allocation:
    - Qian: 
      - [x] Edge communication agent
      - [x] Knowledge transfer
        - Edge clusters
        - Edge AI application
        - Edge agent 
    - Shaojun: 
      - [x] Control plane changes
      - [ ] Data plane changes
    - David: 
      - [x] Testing, dev environment to catch up Mizar newest release
      - [x] Knowledge transfer : Edge clusters
    - Peng:
      - Roadmap & landscape planning
      - Edge gateway initial release design
      - team support
    - Edge agent demo
- "Macro trend" & Roadmap
  - Fornax goals
    - https://www.centauruscloud.io/#projects
  - Field scoping
    - Key directions:
      - Scheduling: Sina & global scheduler
      - Edge storage
      - Serverless
      - Existing & Promising Solution
    - Academia papers
      - [x] The Emerging Landscape of Edge-Computing
      - [x] Edge Intelligence- Paving the Last Mile of Artificial Intelligence With Edge Computing (60%)
      - [x] Adaptive Federated Learning in Resource Constrained Edge Computing Systems
      - [ ] Deep Learning With Edge Computing- A Review
    - Industry conferences submission
      - Deadlines for academia conference in 2022
        - Topics:
          - Edge cluster
          - Edge communication
          - Performance & utilities evaluation
- Akraino Release
- Talk and outreach
  - 2nd brown bag: Communication & Presentation
  - Information sharing: Mizar tooling for the Arktos team
  - Community: UW Bothell CSS talks on our edge, possible project cooperation with grad students. Internship opportunities too.


# 11/17

### Agenda
- Centaurus edge factors
  - Infra Framework
  - Flexibility
  - Scalability
  - Resilence
  - Usability
    - For end users
    - For developers
- Overall status
  - Release 1/30 items, see [project](https://github.com/CentaurusInfra/fornax/projects/2)
    - Edge communication (pod to pod, pod to service)
    - Serverless in a hierarchical edge environment POC
      - stateful: Edge KV store POC
      - runtime support (WebAssembly, etc.)
    - AI face recognization app on hierarchical edge clusters
      - spearate frontend with backend
      - backend "smart" scaling
  - Team allocation:
    - Shaojun: 
      - [x] Control plane changes
      - [x] Data plane changes
      - [ ] Scaled ep for edge (to sync up with Edge team, slides for scenarios)
      - [ ] edge gateway agent (together with Peng) 
    - David: 
      - [ ] Edge cluster setup documentation and automation
    - Peng:
      - Roadmap & feature scoping
      - Edge gateway agent POC -> release
    - Edge agent demo
- Scoping & Roadmap
  - Field scoping
    - Key directions:
      - Scheduling: 
      - Edge storage (KV store)
      - Serverless 
        - Overview presentation next Tuesday, need to sync up with other participants' @Mengni
        - Previous design by Casey
        - Edge Scheduling
        - New Runtime: WebAssembly
    - Academia papers
![image](https://user-images.githubusercontent.com/252020/142293582-a1956715-f34f-4522-b979-6a5ee7828671.png)
    - Industry conferences submission
      - [ ] Deadlines for academia conference in 2022
        - Topics:
          - Edge cluster
          - Edge communication
          - Performance & utilities evaluation
- Akraino Release
- Talk and outreach
  - 2nd brown bag: Communication & Presentation
  - Information sharing: Mizar tooling for the Arktos team
  - Community: UW Bothell CSS talks on our edge, possible project cooperation with grad students. Internship opportunities too.

### Notes
- Manage cluster management at the infra level (), 
- Security as a goal
- serverless design


# 11/24

### Agenda
- Overall status
  - Release 1/30 items, see [project](https://github.com/CentaurusInfra/fornax/projects/2)
    - Edge communication 
      - pod to pod
      - pod to service has feature gap from Mizar
    - Stateful Serverless 
      - stateful: Edge KV store POC
      - runtime support (WebAssembly, etc.)
    - AI face recognization app on hierarchical edge clusters
      - convert to serverless
      - spearate frontend with backend
      - backend "smart" scaling
  - Team allocation:
    - Shaojun: 
      - [x] Control plane changes
      - [x] Data plane changes
      - [ ] Scaled ep for edge (to sync up with Edge team, slides for scenarios)
      - [ ] edge gateway agent (together with Peng) 
    - David: 
      - [ ] Edge cluster setup documentation
      - [ ] Edge cluster setup automation
    - Peng:
      - Stateful serverless
        - [x] Stateful serverless on edge talk
        - [x] Basic serverless usage (Kubeless)
        - [ ] Edge storage options try out
        - [ ] Webassembly deeper dive
      - Edge gateway agent design
    - Edge agent demo
- Scoping & Roadmap
    - Industry conferences submission
      - [ ] Deadlines for academia conference in 2022
        - Topics:
          - Edge cluster
          - Edge-edge communication
          - Performance & utilities evaluation
- Akraino Release
- Talk and outreach
  - More video & streaming use cases and concrete scenarios
  - 2nd brown bag: Communication & Presentation
  - Information sharing: Mizar tooling for the Arktos team
  - Community: UW Bothell CSS talks on our edge, possible project cooperation with grad students. Internship opportunities too.


# 12/01

### Agenda
- Overall status
  - Release 1/30 items, see [project](https://github.com/CentaurusInfra/fornax/projects/2)
    - Edge communication 
      - pod to pod
      - pod to service has feature gap from Mizar
    - Stateful Serverless 
      - stateful: Edge KV store POC
      - runtime support (WebAssembly, etc.)
    - AI face recognization app on hierarchical edge clusters
      - convert to serverless
      - spearate frontend with backend
      - backend "smart" scaling
  - Team allocation:
    - Shaojun: 
      - [x] Control plane changes
      - [x] Data plane changes
      - [x] Scaled ep for edge (to sync up with Edge team, slides for scenarios)
      - [ ] Sync up edge gateway with the latest Mizar release (v0.9)
    - David: 
      - [x] Edge cluster setup documentation
      - [ ] Edge cluster setup automation
    - Peng:
      - Edge gateway agent design
      - Stateful serverless
        - [x] Stateful serverless on edge talk
        - [ ] Edge serverless framework try out
          - [x] Kubeless
          - [ ] Knative
        - [ ] Edge serverless runtime try out
          - [ ] WASMEdge
        - [ ] Edge KV storage try out
          - [ ] Anna
          - [ ] annabellaDB
          - [ ] OrbitDb
        - Edge KV storage possible directions
          - CRDT based distributed KV store
            - Pros & cons
          - "access-pattern aware key-value store"
          - Move data vs Move computation (regional scheduling)
          - Horizontal regional "spill-out" scheduling
    - Edge agent demo
- Scoping & Roadmap
    - Industry conferences submission
      - [ ] Deadlines for academia conference in 2022
        - Topics:
          - Edge cluster
          - Edge-edge communication
          - Performance & utilities evaluation
- Akraino Release
- Talk and outreach
  - 2nd brown bag: Communication & Presentation
  - Information sharing: Mizar tooling for the Arktos team
  - Community: 
    - UW Bothell professor to give a talk on their use cases (in 2 weeks) and possible project cooperation with grad students


# 12/08

### Agenda
- WasmEdge
  - Questions in mind
    - Usage, compatibility
    - Performance
    - Limitation (comparing to container based FAAS)
- Project Tracking
  - Release 1/30 items, see [project](https://github.com/CentaurusInfra/fornax/projects/2)
    - Edge communication 
      - pod to pod communication
    - Stateful Serverless 
      - stateful: Edge KV store POC
      - runtime support (WebAssembly, etc.)
    - AI face recognization app on hierarchical edge clusters
      - convert to serverless
      - spearate frontend with backend
      - backend "smart" scaling
  - Team allocation:
    - Shaojun: 
      - [x] Control plane changes
      - [x] Data plane changes
      - [x] Scaled ep for edge (scraped for 1/30 release)
      - [ ] Sync up edge gateway with the latest Mizar release (v0.9)
    - David: 
      - [x] Edge cluster setup documentation
      - [ ] K3s in edge clusters
    - Ke:
      - [ ] Research on CDN serversless solutions 
        - Presentation at the Monday community meeting (?)
    - Peng:
      - Edge gateway agent design
      - CRDT DB for the edge
      - Stateful serverless
        - [x] Stateful serverless on edge talk
        - [ ] Edge serverless framework try out
          - [x] Kubeless
          - [ ] Knative
        - [ ] Edge serverless runtime try out
          - [ ] WASMEdge
        - [ ] Edge KV storage try out
          - [x] Anna
          - [ ] annabellaDB
          - [ ] OrbitDb
        - Edge KV storage possible directions
          - CRDT based distributed KV store
            - Pros & cons
          - Move data vs Move computation (regional scheduling)
          - Region-aware horizontal scheduling
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
