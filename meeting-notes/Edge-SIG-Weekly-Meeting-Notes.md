# Centaurus - Edge+AI SIG Weekly Meeting
- Wednesday 3:00 - 4:00 PM
- [ZOOM](https://futurewei.zoom.us/j/93051877352?from=addon)


## 02/17

### Agenda:

- Tracks
  - Research
  - Code (Extend Arktos to deploy to Edge https://github.com/pdgetrf/ArktosEdge/issues/3)
- Edge project tracking repo
  - [Project Tracking](https://github.com/pdgetrf/ArktosEdge/projects/1)
- KubeEdge discussion
  - Setup & play ([same network](https://github.com/pdgetrf/ArktosEdge/wiki/KubeEdge-Setup-(Same-Network)), [cloud in GCP, edge in AWS](https://github.com/pdgetrf/ArktosEdge/wiki/KubeEdge-Setup-(Different-Network)))
  - Code walkthrough & deep(er) dive
- Research
  - [AWS Innovate](https://aws.amazon.com/events/aws-innovate/machine-learning/?sc_channel=em&sc_campaign=APAC_FIELD_T1_en-innovate-aiml_20210224_7014z000001MMP3&sc_publisher=aws&sc_medium=em_aws_innovate_aiml&sc_content=field_t1event_field&sc_country=mult&sc_geo=mult&sc_category=mult&sc_outcome=field&trkCampaign=innovate-ml&trk=em_regconfirmed_innovateml21)
  - [State of AI 2020 Report](https://www.stateof.ai), also a [discussion of it](https://youtu.be/o2fYsrV-YlQ)
  - Topics:
    - Scheduling, PolarisCloud
    - Model deployment ([A good demo using GCP](https://youtu.be/fw6NMQrYc6w))
    - Scalability
    - K3s vs KubeEdge

### Notes:
- [x] Global scheduling vs Edge scheduling & placement
  - Scheduling algorithm
- [x] Collect list of ideas for discussion
- [x] Schedule a meet about PolarisCloud 
- [x] Edge models : KubeEdge vs Light mode KubeEdge vs K3s
- [ ] Security vs latency, websocket or better options.
- [ ] Scale up from 2,3k 
- [x] KubeFlow & https://github.com/kubeflow/kfserving

## 02/24

### Agenda
- Edge solution survey (tracking by https://github.com/pdgetrf/ArktosEdge/issues/9)
  - Single node edge
  - Autonomous cluster at Edge (see slides)
  - Features
    - cloud <-> edge tunnel/proxy
    - edge anomomy
      - edge-side apiserver/caching layer
      - edge node and pod health check / stay alive
      - resource grouping (node group, cluster group, deploymet/service group)
    - edge cluster
      - deployment and management
      - self-managing cluster, master migration on power loss

- Other tracking topics
  - KubeEdge MEC Architectur (Mizar into EdgeMesh, gateway, Edge-edge comm, Deepak 3/3 talk)
  - RAINBOW Fog-aware Scheduler


- New Finds
  - [CNCF Cloud Native Interactive Landscape](https://landscape.cncf.io/)
  - [LF AI & Data Foundation Interactive Landscape](https://landscape.lfai.foundation/)
  - [Looks familiar?](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.alamy.com%2Fstock-photo-rear-of-a-subaru-imprezza-wrx-wagon-covered-in-bumperstickers-with-19518801.html&psig=AOvVaw3uMN5aEUxpywIhzk69H26W&ust=1614118138974000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCJiRl-XA_u4CFQAAAAAdAAAAABAO)


### Notes
- [ ] lite edge vs full fledged

## 03/03

### Agenda
- EdgeCluster feature
  - Edge capability: survive both network and node failure
  - Locality is important
  - Self-managing cluster
  - EdgeCluster as a custom resource

## 03/10

### Agenda
- n-ary tree based Arktos Edge topology

### Notes
- [x] complexity worth it?
- [ ] local firewall preventing clusters to connect to their root clusers
- [x] local node vs gloal management
- [x] multi-tenancy at edge node (in recursive case, there's a conflict case to discuss)
- [x] use case scenario for hireachy structure
  - [x] kube MEC meeting
- [x] centralized controls over de-centralized control
- [x] schedule meeting with Deepak about network and security


## 03/18

### Agenda
- hireachy model & use cases
- cluster connector demo
- multi-tenancy EdgeCluster
- EdgeCluster provisioning model
- EdgeCluster components initial thoughts (cut short due to time limit)

### Notes
- EdgeCluster as first release goal
- VPC in EdgeCluster needs further looked into
