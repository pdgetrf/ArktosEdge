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
        - [ ] Merge perviously POC control plane code into Mizar
    - David: 
      - [x] Edge cluster setup documentation
      - [ ] K3s in edge clusters
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

