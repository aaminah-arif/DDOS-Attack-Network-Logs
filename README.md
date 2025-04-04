# Network Traffic Dataset for KNN Classification

## Overview
This dataset contains approximately 2.1 million labeled network log entries capturing various types of network traffic and attacks. The goal is to classify network traffic using the K-Nearest Neighbors (KNN) algorithm. We will be using a short verison of the dataset.

## Dataset Description
The dataset consists of labeled network logs that categorize traffic into five classes:

- **Normal** (Benign network traffic)
- **UDP-Flood** (Denial of Service attack using UDP packets)
- **Smurf** (Denial of Service attack involving ICMP packets)
- **SIDDOS** (Simulated Distributed Denial of Service attack)
- **HTTP-FLOOD** (Denial of Service attack targeting HTTP services)

Each record in the dataset contains attributes related to network traffic, including packet details, node information, and traffic characteristics.

## Attributes
The dataset includes the following attributes:

```
- SRC_ADD (numeric): Source address of the packet
- DES_ADD (numeric): Destination address of the packet
- PKT_ID (numeric): Unique packet identifier
- FROM_NODE (numeric): Source node identifier
- TO_NODE (numeric): Destination node identifier
- PKT_TYPE (categorical): Type of packet (e.g., tcp, ack, cbr, ping)
- PKT_SIZE (numeric): Size of the packet
- FLAGS (categorical): Flags associated with the packet
- FID (numeric): Flow identifier
- SEQ_NUMBER (numeric): Sequence number of the packet
- NUMBER_OF_PKT (numeric): Total number of packets in a session
- NUMBER_OF_BYTE (numeric): Total number of bytes in a session
- NODE_NAME_FROM (categorical): Name of the source node
- NODE_NAME_TO (categorical): Name of the destination node
- PKT_IN (numeric): Incoming packets count
- PKT_OUT (numeric): Outgoing packets count
- PKT_R (numeric): Packet rate
- PKT_DELAY_NODE (numeric): Delay at the node level
- PKT_RATE (numeric): Overall packet rate
- BYTE_RATE (numeric): Byte transmission rate
- PKT_AVG_SIZE (numeric): Average packet size
- UTILIZATION (numeric): Network utilization percentage
- PKT_DELAY (numeric): Overall packet delay
- PKT_SEND_TIME (numeric): Timestamp when the packet was sent
- PKT_RECEIVED_TIME (numeric): Timestamp when the packet was received
- FIRST_PKT_SENT (numeric): Timestamp of the first packet in a session
- LAST_PKT_RECEIVED (numeric): Timestamp of the last packet in a session
- PKT_CLASS (categorical): Classification label for the packet (Normal, UDP-Flood, Smurf, SIDDOS, HTTP-FLOOD)
```

## Classification Task
We aim to use the **K-Nearest Neighbors (KNN)** algorithm to classify network traffic into one of the five categories based on the provided attributes. The dataset includes both numerical and categorical features, requiring preprocessing steps such as:

- Encoding categorical features
- Feature scaling for numeric attributes
- Handling class imbalance if necessary


## Potential Applications
- Intrusion Detection Systems (IDS)
- Network Security Analysis
- Traffic Pattern Analysis
- Cyberattack Mitigation Strategies

## Acknowledgments
This dataset is provided for research and educational purposes in cybersecurity and machine learning. Proper attribution should be given when using the dataset in projects or publications.

---
**Contact:** If you have any questions or require further details, feel free to reach out!

