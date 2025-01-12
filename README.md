# rdmafpga
RDMA for Xilinx accelerator cards

# Remote DMA for ML Clusters on Xilinx U200

This repository contains the source code and documentation for my research on leveraging Remote Direct Memory Access (RDMA) over PCIe to accelerate Machine Learning (ML) clusters using Xilinx U200 cards.

## Overview

Modern ML workloads often involve large datasets and frequent data transfers between nodes in a cluster. Traditional communication methods, such as TCP/IP, can introduce significant overhead and limit performance. This project explores the use of RDMA over PCIe as a high-performance, low-latency alternative for inter-node communication in ML clusters.

The Xilinx U200 card, with its powerful FPGA and high-bandwidth PCIe interface, provides an ideal platform for implementing and evaluating RDMA-based communication solutions. This repository showcases various techniques and optimizations for achieving efficient data transfer and improving overall cluster performance.

## Features

  * **RDMA over PCIe implementation:**  Leverages the U200's PCIe capabilities to enable direct memory access between nodes.
  * **Optimized data transfer:**  Implements various techniques to minimize latency and maximize throughput.
  * **ML workload integration:** Demonstrates the integration of RDMA with common ML frameworks and applications.
  * **Performance evaluation:** Provides benchmarks and analysis of RDMA performance in different ML cluster scenarios.

## Contents

  * **src:** Contains the SystemVerilog source code for the RDMA implementation on the U200.
  * **docs:** Contains documentation, including design specifications, implementation details, and performance reports.
  * **scripts:** Contains scripts for building, deploying, and testing the RDMA solution.
  * **examples:** Contains example applications demonstrating the use of RDMA in ML workloads.

## Getting Started

1.  **Prerequisites:**
      * Xilinx Vivado Design Suite
      * Xilinx Runtime (XRT)
      * U200 development platform
      * Basic knowledge of SystemVerilog and FPGA development
2.  **Clone the repository:**
    ```bash
    git clone https://github.com/cowboywyo/rdmafpga.git
    ```
3.  **Build the project:**
    Follow the instructions in the `docs/build.md` file to build the SystemVerilog code and generate the bitstream.
4.  **Deploy and test:**
    Refer to the `docs/deploy.md` file for instructions on deploying the bitstream to the U200 and running the test applications.

## Contributing

Contributions are welcome! Please feel free to submit bug reports, feature requests, or pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
