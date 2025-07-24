## Configuration: ASUS RT-AX1800S Multi-Mode Router Setup

The ASUS RT-AX1800S represents the final stage of network delivery in many VR deployments, providing WiFi 6 capabilities that are increasingly important for high-performance VR experiences. Think of the ASUS router as your VR network's specialized performance engine - it takes the internet connectivity provided by earlier stages and optimizes it specifically for VR applications.

### Understanding WiFi 6 Benefits for VR

#### Why WiFi 6 Matters for VR Applications

WiFi 6 (802.11ax) introduces several technologies that directly benefit VR deployments:

**OFDMA (Orthogonal Frequency Division Multiple Access):** Instead of serving one device at a time, WiFi 6 can serve multiple devices simultaneously by dividing channels into smaller resource units. For VR, this means multiple headsets can receive data concurrently without waiting in line.

**Target Wake Time:** This feature allows devices to schedule when they communicate with the router, reducing network congestion and improving battery life for wireless VR controllers and accessories.

**1024-QAM Modulation:** More data can be packed into each transmission, increasing throughput by up to 25% compared to WiFi 5, providing more bandwidth for high-resolution VR content.

**Improved MU-MIMO:** Multi-User MIMO technology allows the router to communicate with multiple devices simultaneously. WiFi 6 expands this from 4 simultaneous streams to 8, crucial when supporting multiple VR users.

### Hardware Specifications and Firmware

**Current Firmware Versions:**
- RT-AX1800S V1: 3.0.0.4.386_69100
- RT-AX1800S V2: 3.0.0.4.388_33911 (includes built-in WireGuard VPN support)

**Performance Specifications:**
- **Total WiFi Speed:** 1800 Mbps (574 Mbps on 2.4GHz + 1201 Mbps on 5GHz)
- **Ethernet Ports:** 4x Gigabit LAN + 1x Gigabit WAN
- **Default IP Addresses:** 192.168.1.1 (Router mode), 192.168.50.1 (Access Point mode)
- **Maximum Concurrent Users:** 100+ devices with proper configuration

### Understanding Router Operating Modes

The ASUS RT-AX1800S can operate in several modes, each serving different network architectures:

#### Router Mode (Primary Gateway Configuration)

**When to Use Router Mode:**
Router mode is appropriate when the ASUS device serves as your network's primary gateway - handling internet connectivity, DHCP services, and network security. This mode works well when you have a direct internet connection (ethernet from ISP, cable modem, or upstream router) and need full network control.

**Router Mode Benefits:**
- Complete control over network policies and security
- Advanced QoS and traffic management capabilities
- Full firewall functionality with customizable rules
- Support for VPN servers and advanced networking features

#### Access Point Mode (Network Extension Configuration)

**When to Use Access Point Mode:**
Access Point mode is ideal when you want to extend an existing network without creating additional network segments. In this mode, the ASUS device functions as a wireless access point, providing WiFi coverage while maintaining the same IP addressing scheme as the upstream network.

**Why This Mode Works Well for VR Deployments:**
Access Point mode eliminates the complexity of multiple network segments while providing WiFi 6 performance benefits. All devices - whether connected to the upstream router or the ASUS access point - can communicate directly without routing between different subnets.

**Configuration Considerations:**
When switching to Access Point mode, the router changes its IP address and disables many routing features. Plan this change carefully and ensure you can reconnect to the new IP address.

#### Repeater Mode (Range Extension)

**Understanding Repeater Limitations:**
Repeater mode extends wireless coverage by receiving a WiFi signal and retransmitting it. However, this typically reduces available bandwidth by approximately 50% because the device must use the same radio to both receive and transmit data.

**When Repeater Mode Makes Sense:**
Despite the bandwidth reduction, repeater mode can be valuable when ethernet connectivity isn't available and you need to extend coverage to areas with poor WiFi reception.

### Detailed Configuration Procedures

#### Router Mode Setup for VR Networks

1. **Initial Access and Security Setup**
Connect to the router using either http://router.asus.com or http://192.168.1.1. The router will automatically launch the Quick Internet Setup (QIS) wizard on first access. Change the default administrator password immediately - use a strong password that your deployment team can remember but that provides appropriate security.

2. **Internet Connection Configuration**
Configure the WAN (internet) connection based on your upstream connectivity:
- **DHCP:** Most common, used when connecting to another router or modem
- **Static IP:** Used when you have specific IP address assignments from the institution
- **PPPoE:** Less common in institutional environments, typically used with DSL connections

3. **VR-Optimized Wireless Configuration**
Navigate to **Wireless → Professional** for advanced wireless settings:
- **5GHz Channel Selection:** Use channels 36, 40, 44, or 48 for optimal VR performance (these channels have higher power limits and less interference from non-WiFi devices)
- **Channel Width:** Set to 80MHz for maximum throughput, but monitor for interference in congested environments
- **Beamforming:** Enable beamforming to focus wireless signals toward VR devices
- **MU-MIMO:** Ensure MU-MIMO is enabled to serve multiple VR devices simultaneously

4. **Network Segmentation with VLANs**
For advanced deployments, configure VLANs to separate different types of traffic:
- **VLAN 10:** VR devices (192.168.10.x)
- **VLAN 20:** Administrative computers (192.168.20.x)
- **VLAN 30:** Guest access (192.168.30.x)

Navigate to **Advanced Settings → LAN → VLAN** to configure these segments. Assign specific ethernet ports to VLANs and configure inter-VLAN routing policies based on your security requirements.

#### Access Point Mode Configuration

**Mode Conversion Process:**
1. Navigate to **Administration → Operation Mode**
2. Select **Access Point Mode**
3. **Important:** The router will reboot and change its IP address, typically to an address assigned by the upstream router
4. Use the ASUS Device Discovery utility or check your upstream router's client list to find the new IP address

**Post-Conversion Configuration:**
After switching to Access Point mode, many advanced routing features are disabled, but you retain:
- Wireless configuration and optimization settings
- Basic QoS capabilities
- Guest network functionality
- AiProtection security features (if supported by firmware)

**Optimizing Access Point Performance:**
- Position the router for optimal coverage of your VR area
- Configure a dedicated SSID for VR devices to simplify connection management
- Enable band steering to automatically direct capable devices to 5GHz
- Monitor channel utilization and adjust channels if interference develops

### Advanced Quality of Service Configuration

#### Understanding QoS for VR Applications

Quality of Service (QoS) manages how network bandwidth is allocated among different applications and devices. For VR deployments, QoS serves two critical functions: ensuring VR applications get the bandwidth they need and preventing background traffic from interfering with real-time VR data.

**VR Traffic Characteristics:**
VR applications generate several types of network traffic with different requirements:
- **Motion tracking data:** Small packets requiring extremely low latency
- **Video streams:** Large amounts of data requiring consistent bandwidth
- **Audio streams:** Moderate bandwidth with strict timing requirements
- **Haptic feedback:** Small packets requiring predictable delivery timing

#### Configuring Adaptive QoS

**Enable Gaming Mode for VR:**
Navigate to **Advanced Settings → QoS → Gaming Mode**. Gaming mode automatically prioritizes real-time traffic and reduces latency for interactive applications. While designed for gaming, these optimizations directly benefit VR applications.

**Device-Specific QoS Rules:**
Create specific rules for VR devices:
1. Identify VR headsets and computers by MAC address
2. Assign them to the "Gaming" or "Streaming" categories
3. Allocate minimum guaranteed bandwidth (suggest 100 Mbps per VR device)
4. Set maximum bandwidth limits to prevent any single device from consuming all available bandwidth

**Bandwidth Allocation Strategy:**
- **Reserve 60-70%** of total bandwidth for VR traffic during active use
- **Limit background applications** (updates, cloud sync) to 10-20% of bandwidth
- **Maintain 20-30%** buffer for overhead and network management traffic

### Network Security Implementation

#### WiFi Security Configuration

**WPA3-Enterprise for Institutional Environments:**
If your institution supports RADIUS authentication, configure WPA3-Enterprise:
1. Navigate to **Wireless → General**
2. Select WPA3-Enterprise authentication method
3. Configure RADIUS server settings (IP address, port, shared key)
4. Test authentication with a known device before deploying to all VR equipment

**Certificate-Based Authentication:**
For highest security, implement certificate-based authentication where each device has a unique certificate for network access. This prevents credential sharing and provides strong device identification.

**MAC Address Filtering:**
Navigate to **Wireless → MAC Filter** to implement MAC address filtering:
- **Accept Mode:** Only listed devices can connect (highest security)
- **Reject Mode:** Listed devices are blocked (useful for preventing specific devices from connecting)

Document all MAC addresses in a maintenance log for future reference.

#### Network Segmentation and Firewall Configuration

**Guest Network Isolation:**
Configure guest networks with appropriate isolation:
1. Enable guest network with separate SSID
2. Configure bandwidth limitations (suggest 25% of total bandwidth)
3. Enable access restrictions (block local network access, limit internet access times)
4. Document guest network credentials for visitor access

**Firewall Rules for VR Traffic:**
Configure firewall rules to optimize VR traffic flow:
- Allow all outbound connections from VR devices
- Configure port forwarding if VR applications require specific inbound connections
- Block unnecessary protocols (P2P, BitTorrent) that could interfere with VR performance
- Enable DDoS protection to prevent network disruption

### Why This Configuration Works Well for VR Deployments

The ASUS RT-AX1800S serves as the final optimization layer in your network architecture. While upstream routers handle connectivity and basic routing, the ASUS router focuses specifically on wireless performance and VR optimization. This approach provides several key advantages:

**Dedicated VR Optimization:** The ASUS router can be configured specifically for VR requirements without compromising upstream network policies. WiFi 6 features like OFDMA and improved MU-MIMO directly address the multi-device, high-bandwidth requirements of VR deployments.

**Network Performance Control:** Advanced QoS features allow you to guarantee bandwidth for VR applications while managing background traffic. This control is essential in institutional environments where network usage can be unpredictable.

**Security Boundary Management:** The ASUS router provides a clear demarcation between institutional network policies and VR-specific requirements. You can implement VR-appropriate security measures while respecting institutional network policies.

**Troubleshooting Simplification:** When network issues arise, having a dedicated VR router makes it easier to determine whether problems are related to upstream connectivity or VR-specific configuration. This separation significantly reduces troubleshooting time.
