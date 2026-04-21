## 🚀 Project Overview

This project demonstrates the implementation of a Software Defined Networking (SDN) Learning Switch Controller using the Ryu controller framework.
The controller dynamically learns MAC addresses from incoming packets and installs forwarding rules in the switch to enable efficient communication between hosts.

The network topology is emulated using Mininet, and the communication between the controller and switch is managed using the OpenFlow protocol.

This project provides practical exposure to SDN architecture, network virtualization, and traffic management concepts.

---

## 🏗️ System Architecture

The system consists of the following components:

* **SDN Controller** – Implements learning switch logic
* **OpenFlow Switch** – Forwards packets based on flow rules
* **Hosts** – End devices generating network traffic
* **Mininet Topology** – Simulated network environment

---

## 🔑 Key Features

* Dynamic MAC address learning
* Automated flow rule installation
* Centralized network control
* Efficient packet forwarding
* Network traffic performance testing using iperf
* Flow table inspection using OpenFlow tools

---

## 🧠 Technical Highlights

* Implemented a Layer-2 Learning Switch Controller
* Used event-driven packet handling in Ryu
* Simulated custom network topology using Mininet
* Verified network connectivity using ping tests
* Measured bandwidth using iperf
* Monitored flow entries using ovs-ofctl

---

## 📈 Performance Evaluation

The network performance was evaluated using iperf to measure bandwidth between hosts.
The controller successfully installed flow rules dynamically, reducing broadcast traffic and improving packet forwarding efficiency.

---

## 🧪 Testing and Validation

The following tests were performed:

* Connectivity test using `pingall`
* Bandwidth measurement using `iperf`
* Flow table verification using `ovs-ofctl`
* Controller-switch communication validation

All tests confirmed correct functionality of the learning switch controller.

---

## 📚 Skills Demonstrated

* Software Defined Networking (SDN)
* Computer Networking Fundamentals
* Python Programming
* Network Simulation and Virtualization
* Linux Command-Line Usage
* Debugging and Performance Analysis

---

## ⚙️ How to Run

1. Start the Ryu controller
ryu-manager learning_switch.py

2. Run the Mininet topology
sudo python3 topo.py

3. Test network connectivity
pingall

4. Check flow table entries
sudo ovs-ofctl -O OpenFlow13 dump-flows s1
