# Lab: Basic LAN Configuration

## Lab Objective
Configure a simple Local Area Network (LAN) with one WRT300N wireless router, a Linux laptop, a gaming computer, a smartphone and a CCTV webcam.

## Topology Diagram
![Alt text](images/diagram.png)

## IP Address Table

| Device           | Interface | IP Address     | Subnet Mask      | Default Gateway |
|------------------|-----------|----------------|------------------|-----------------|
| Wireless Router0 | N/A       | 192.168.0.1    | 255.255.255.0    | N/A             |
| PC-PT            | FASTETHO  | 192.168.0.103  | 255.255.255.0    | 192.168.0.1     |
| Laptop-PT        | WPC300N   | 192.168.0.104  | 255.255.255.0    | 192.168.0.1     |
| Webcam           | Wireless0 | 192.168.0.101  | 255.255.255.0    | 192.168.0.1     |
| Smartphone       | Wireless0 | 192.168.0.102  | 255.255.255.0    | 192.168.0.1     |

## Step-by-Step Configuration
### Step 1: Assign IP Addresses
**PC-PT: 192.168.0.103**

**Laptop-PT: 192.168.0.104**

**Webcam: 192.168.0.101**

**Smartphone: 192.168.0.102**

### Step 2: Connect Devices
- Use Copper Straight-Through cables
- Connect PC-PT → Router

- Use WPC300N(Wireless adapter)
- Connect Laptop-PT → Router

- Use Wireless0(Wireless interface)
- Connect Webcam → Router

- Use Wireless0(Wireless interface)
- Connect Smartphone → Router

### Step 3: Verify Connectivity
- From Laptop-PT, open Command Prompt:
```bash
ping 192.168.0.103
![Alt text](images/ping_gamingpc.png)

ping 192.168.0.104
![Alt text](images/ping_laptop.png)

ping 192.168.0.101
![Alt text](images/ping_cctv.png)

ping 192.168.0.102
![Alt text](images/ping_smartphone.png)