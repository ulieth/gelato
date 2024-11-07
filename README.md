# FAQ

## What is Gelato RaaS?

Gelato RaaS (Rollup-as-a-Service) is a specialized service that simplifies the process of running Ethereum Layer 2 rollups.

### Traditional Rollup Deployment:

1. Developer -> Set up nodes
2. Configure network
3. Manage infrastructure
4. Monitor
5. Maintain

### With Gelato RaaS:

1. Developer -> Configure via Gelato's interface
2. Gelato manages everything else.

### Gelato RaaS provides:
- Sequencer nodes (process and order transactions)
- Validator nodes (verify transaction validity)
- Block producer nodes
- Data availability services

---

## What are Execution Frameworks?

Execution frameworks are protocols that define how transactions are processed and validated on the blockchain. They determine the underlying architecture and performance characteristics of Layer 2 solutions.

---

## What aspects to consider when choosing a framework?

When choosing an execution framework, consider the following factors:

- **Performance requirements**: transaction throughput, block time needs, finality requirements
- **Security model**: optimistic vs ZK, validator requirements, proof system needs
- **Cost considerations**: gas optimization, data availability costs, operational overhead
- **Development experience**: EVM compatibility, tool support, developer ecosystem

---

## How does Gelato handle finality requirements?

Finality refers to how quickly and definitively a transaction becomes irreversible on the blockchain. Gelato’s finality handling is framework-specific:

- **OP Stack**: Uses challenge period and validator confirmations
- **Arbitrum Orbit**: Implements AnyTrust for faster finality
- **Polygon CDK**: Utilizes ZK proofs when available

---

## Which execution framework is better?

### 1. OP Stack
- **Best for**: General-purpose dApps
- **When you need**: High EVM compatibility
- **Cost optimization**: 90% lower fees

### 2. Arbitrum Orbit
- **Best for**: Fast-finality applications
- **When you need**: Custom validator sets
- **Performance**: Lower latency

### 3. Polygon CDK
- **Best for**: ZK-focused applications
- **When you need**: Customizable consensus
- **Security**: Shared with Polygon
