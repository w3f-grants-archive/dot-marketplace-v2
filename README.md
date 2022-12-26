# Dot Marketplace v3

- **Status:** Open
- **Project Name:** Dot Marketplace
- **Team Name:** Wow Labz
- **Payment Address:** 0xF13001401396AA866E8012f31fD939C7E83B8601 (USDT - ERC20)
- **Level:** 2

## Project Overview :page_facing_up:

### **Overview**

This is phase 3 of Dot Marketplace, which is a general-purpose decentralized marketplace created as a Substrate pallet.
- Here's a link to the [approved grant proposal for the first phase](https://github.com/w3f/Grants-Program/blob/master/applications/dot_marketplace.md) and [the second phase](https://github.com/w3f/Grants-Program/blob/master/applications/dot_marketplace-phase2.md)

- Dot Marketplace can be used by any decentralized project to float projects and invite their community members to execute them for a reward. Its POC was developed during the Polkadot India Buildathon (2021).
- It would be directly integrated into Polkadot JS Apps, where such marketplaces could create bounties and projects that community members could fulfill.
- The inspiration for Dot Marketplace emerged from our own needs while building Yoda - a protocol that facilitates decentralized app development leveraging open data. Dot Marketplace would be used to create data, services, and app marketplaces on Yoda, which would motivate us to maintain this project in the long run.

### **Project Details**

The current scope of work involves **milestone-based submissions** in which a project is divided into multiple configurable milestones(min 1 and max 5) to allow parallel or sequential execution.

- This version of the marketplace handles the project by breaking it into several milestones
- Each project must have at least one milestone and can have a maximum of five milestones (configurable)
- Each milestone has its independent bidding system where multiple workers can place their bids
- The publisher can select a bid as per the requirement and ratings of the worker and other criteria that can be added to a user account.
- A worker can bid for multiple milestones of a single project based on their expertise.
- A project reaches completion only if all milestones in the project are completed and approved by the publisher.
- Since all milestones are independent, they can be completed and approved by the publisher irrespective of the overall project status.
- Based on the requirements, a publisher can add more milestones to a project even after it is pushed to the market, provided the total number of milestones does not exceed 5 (configurable)
- The [decentralized court](https://github.com/WowLabz/dot-marketplace-v2) implemented in phase 2 is functional for each milestone of a project


The flow of tasking pallet with milestone based submission 


![Tasking-Court-Flow4 drawio](https://user-images.githubusercontent.com/43837760/160392143-5ce00b53-3bb6-4c87-8fb9-d7fe8c2f0ca1.jpeg)



Dot Marketplace is being built as a Substrate pallet. It would include boilerplate code that teams can customize as per their requirements. We believe this project has the potential to transform community participation, engagement, and governance in decentralized projects.

### **Repository Hierarchy**

```bash
node
├── build.rs
├── Cargo.toml
└── src
    ├── chain_spec.rs
    ├── cli.rs
    ├── command.rs
    ├── lib.rs
    ├── main.rs
    ├── rpc.rs
    └── service.rs
scripts
├── docker_run.sh
└── init.sh
pallets
├── pallet-chat
│   ├── Cargo.toml
│   ├── README.md
│   └── src
│       ├── benchmarking.rs
│       ├── lib.rs
│       ├── mock.rs
│       └── tests.rs
└── pallet-tasking
    ├── Cargo.toml
    ├── README.md
    └── src
        ├── benchmarking.rs
        ├── lib.rs
        ├── mock.rs
        ├── utils.rs 
        └── tests.rs
runtime
├── build.rs
├── Cargo.toml
└── src
    └── lib.rs
```

The current focus is to enhance the existing Substrate pallet and allied code base to get a basic yet functional marketplace up and running.

### **Ecosystem Fit**

We believe this work could be helpful for any Polkadot para-chains/ para-threads interested in including a marketplace with an on-chain dispute resolution mechanism.

- Almost all para-chains/ para-threads would find motivation in encouraging their community members to contribute meaningfully to their roadmap. This can be achieved by utilizing a marketplace like Dot Marketplace, where technical, marketing, or governance-centric projects can be published as bounties. And community members are invited to bid for and execute them.
- A milestone-based submission will enhance the functionality of the marketplace and provide a more comprehensive user experience for both the worker and the publisher.
- The on-chain court will act as a dispute resolution mechanism between users involved in a project. A set of community members meeting specific criteria get to be a part of the jury for the dispute and cast votes, based on which a decision is reached.
- To facilitate easier communication between a customer and a worker, a one-to-one chat feature is also created.

## **Team 👥**

### **Team members**

- [**Amit Singh**](https://www.linkedin.com/in/startupamit/) [ Product Manager ]
- [**Roshit Omanakuttan**](https://www.linkedin.com/in/roshit/) [ Technical Architect ]
- [**Varun Gyanchandani**](https://www.linkedin.com/in/varunsays/) [ Backend Lead ]
- [**Loakesh Indiran**](https://www.linkedin.com/in/loakesh-indiran-8a2282140) [ Full Stack Developer ]
- [**Tejas Gaware**](http://www.linkedin.com/in/tejas-vijay-1430a3190) [ Backend Developer ]
- [**Praneeth Ratnagiri**](https://www.linkedin.com/in/praneeth-ratnagiri-772a43174/) [ Backend Developer ]
- [**Rajat Petwal**](https://www.linkedin.com/in/rajat-petwal-947440197/) [ Backend Developer ]

### **Contact**

- **Contact Name:** Amit Singh
- **Contact Email:** amit (dot) singh (@) wowlabz.com
- **Website:** [http://www.wowlabz.com](https://www.wowlabz.com/)
- **Project Website:** Dot marketplace website is under construction

### **Legal Structure**

- **Registered Address:** Wow Labz, 2Gethr Cowork, Tower B, Mantri Commercio, Outer Ring Rd, Bellandur, Bengaluru, Karnataka, India 560103
- **Registered Legal Entity:** Wow Internet Labz Private Limited

### **Team's experience**

Dot Marketplace is being built by the team at Wow Labz. Wow Labz is one of India's leading turnkey product development companies. Socialli Protocol has been conceptualized and is being produced by the team at Wow Labz. The team has previously built a decentralized storage protocol called Lake Network - [https://lakenetwork.io/](https://lakenetwork.io/) in addition to multiple dApps on Ethereum, Stellar, EOS, and Hyperledger.

A list of centralized apps published can be found [here](https://www.wowlabz.com/work/).

### **Team Code Repos**

- [https://github.com/orgs/WowLabz/projects](https://github.com/orgs/WowLabz/projects)
- [https://github.com/WowLabz/tasking_backend](https://github.com/WowLabz/tasking_backend)
- [https://github.com/WowLabz/tasking_frontend](https://github.com/WowLabz/tasking_frontend)
- [https://github.com/WowLabz/yoda_creator_economy_node](https://github.com/WowLabz/yoda_creator_economy_node)
- [https://github.com/WowLabz/dot-marketplace-v2](https://github.com/WowLabz/dot-marketplace-v2)

## **Development Status 📖**

Dot Marketplace POC was conceptualized and developed during the Polkadot India hackathon. The roadmap listed below comprises new features that would help take the POC to a minimum viable product (MVP). The first stage of the project involved creating a user registration and marketplace based on a bidding system.

- Here's a link to the [approved grant proposal for the first phase](https://github.com/w3f/Grants-Program/blob/master/applications/dot_marketplace.md) and [second phase](https://github.com/w3f/Grants-Program/blob/master/applications/dot_marketplace-phase2.md)
- We are in touch with Marcin and Raul from the Web 3 Grants and Treasuries team, respectively.

## **Development Roadmap** 🔩

****Overview****

* **Total Estimated Duration:** 4 Weeks
* **Full-Time Equivalent (FTE): 1.5**  
* **Total Costs:**  USD


### **Milestone 1**

* **Estimated duration:** 1.5 weeks
* **FTE: 1**  
* **PTE: 2**  
* **Costs:**   USD  

The main deliverable for this milestone is to facilitate the creation of a project that can accommodate multiple milestones that may or may not depend on each other.

| Sr no. | Deliverable | Description |
| --- | --- | --- |
| 0a | License | Apache 2.0 |
| 0b | Documentation | We will provide both inline documentation of the code and a tutorial that explains how a user can use DOT Marketplace and understand the flow of tasking pallet. |
| 0c | Testing Guide | Functions will be covered by unit tests, the documentation will describe how to run these tests. We will also provide scripts to help deploy, run and test the build. |
| 0d | Docker Image | Docker image of the build |
| 1 | Project Structure | The existing application only allows one milestone per project. Phase 3 modifies it to allow a publisher to add multiple milestones under the same project |
| 2 | Multiple Bidders| Multiple bidders can now bid for the same milestone, and the publisher can choose one worker based on the bidder ratings |
| 3 | Escrow  | Multiple subaccounts are created for a project to account for each milestone and make it easier to store all funds for transfer/exchange. |


### **Milestone 2**

* **Estimated duration:** 2.5 weeks
* **FTE:** 2  
* **PTE:** 0
* **Costs:**  USD  


In continuation to previous work, this milestone involves the creation of an on-chain decentralized court to handle dispute resolution. Each milestone can go into a dispute on the same scope as mentioned in the second phase of dot marketplace. The other milestones in a project are not affected by the dispute of one of the milestones.

| Sr no. | Deliverable | Description |
| --- | --- | --- |
| 0a | License | Apache 2.0 |
| 0b | Documentation | We will provide both inline documentation of the code and a tutorial that explains how a user can use DOT Marketplace and understand the flow of tasking pallet. |
| 0c | Testing Guide | Functions will be covered by unit tests, the documentation will describe how to run these tests. We will also provide scripts to help deploy, run and test the build. |
| 0d | Docker Image | Docker image of the build |
| 1 | Decentralized Court Module | An on-chain decentralized court for dispute resolution within the ecosystem. |
| 1a | Disapprove Milestone  | In the case of a customer not being satisfied with the work submitted by the service provider (worker). A set of jurors is shortlisted (court summon) to resolve the dispute and pass a verdict. |
| 1b | Disapprove Rating | The customer or the service provider, once they have received their rating for a particular milestone and are not satisfied with it. |
| 1c | General Dispute | A general dispute function for cases that do not fall under the categories mentioned in 1a and 1b. |
| 2 | Voting module | Each juror can review the dispute and cast their vote, which also includes their rating for both the customer and the worker. After two days, all the juror votes are counted, and a winner is identified. |
| 3 | Frontend App  | Supporting frontend UI to test the aforementioned functionality. |
| 4 | Website  | Dedicated one-page website for Dot Marketplace. |
| 5 | Article | Website article showing motivation behind phase 3 of dot marketplace and how to make the best use of it. |

### Rust Run

Use Rust's native `cargo` command to build and launch the template node: 
Note : The current build is supported by Rust Nightly `1.58.0-nightly` due to its dependency on a specific crate used in this codebase.
Please update the rust version accordingly to run the build.

```sh
rustup update

# installing rust version 1.58.0-nightly
rustup install nightly-2021-11-01

# setting rust default version as 1.58.0-nightly
rustup default nightly-2021-11-01

# run the node
cargo run --release -- --dev --tmp
```

### Build

The `cargo run` command will perform an initial build. Use the following command to build the node
without launching it:

```sh
cargo build --release
```

### Tests

Test cases can be run using the following command.
```sh
cargo test
``` 

### Embedded Docs

Once the project has been built, the following command can be used to explore all parameters and
subcommands:

```sh
./target/release/dot_marketplace_node -h
```

## Run

The provided `cargo run` command will launch a temporary node and its state will be discarded after
you terminate the process. After the project has been built, there are other ways to launch the
node.

### Single-Node Development Chain

This command will start the single-node development chain with persistent state:

```bash
./target/release/dot_marketplace_node --dev
```

Purge the development chain's state:

```bash
./target/release/dot_marketplace_node purge-chain --dev
```

Start the development chain with detailed logging:

```bash
RUST_LOG=debug RUST_BACKTRACE=1 ./target/release/dot_marketplace_node -lruntime=debug --dev
```

### **Additional Project Details**

* Technology stack being used
  * Rust, Substrate, React, Python, centralized cloud storage

### **Future Plans** 
Future releases of the Dot Marketplace include:

| Phase | Feature | Description |
| --- | --- | --- |
| 4 | Decentralized Storage and Advanced Search| Integration with IPFS or another decentralized storage platform. The Advanced search provides a way to filter projects and milestones based on status (open/in progress/closed) and also based on your tags|

###

## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?** Web3 Foundation Website, Polkadot India Buildathon 

* We have been working on this roadmap since we applied for the Web3 grant
