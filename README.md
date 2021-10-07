# datacenter-app-profiling

**Project goal:** Redesign hardware for data center applications

**Motivation:** Recently, data centers have been using heterogeneous, application-specific hardware accelerators to meet stringent performance requirements. These accelerators tend to be limited to the scope of a single operation, such as protocol-specific serialization/deserialization or ML inference. Instead of being limited to the scope of a single application, we would like to rethink how data center hardware should be designed to generically support diverse application classes. 

**Project plan:**

_Step 1:_ Use CloudLab to profile (e.g., using hardware performance counters) an open-source benchmark suite of data center applications, such as DeathStarBench (https://github.com/delimitrou/DeathStarBench).

_Step 2:_ Use the profile information to identify where these applications spend most of their cycles. Such a characterization will help determine common operations that can benefit from hardware optimizations.

_Step 3:_ After identifying hardware design optimizations and challenges, implement them using a simulator (e.g., the gem5 simulator).

_Step 4:_ Run simulations on CloudLab to determine whether the hardware optimization is beneficial.  
