## Configuration: Combined Opal + ASUS Cascaded Setup

The combination of GL.iNet Opal and ASUS RT-AX1800S creates a powerful two-tier network architecture that leverages each router's strengths while addressing the specific challenges of institutional VR deployments. This configuration represents a sweet spot between complexity and capability, providing professional-grade networking features without requiring extensive networking expertise.

### Understanding the Two-Tier Architecture

#### Why Cascaded Routers Improve VR Performance

Think of the cascaded setup as a specialized assembly line for network traffic. The Opal handles the complex task of connecting to institutional networks, dealing with authentication, VPN requirements, and network policy compliance. The ASUS router then takes that connectivity and optimizes it specifically for VR applications, providing WiFi 6 performance, advanced QoS, and VR-specific network features.

This division of labor provides several advantages:
- **Specialized Optimization:** Each router focuses on what it does best
- **Fault Isolation:** Problems can be isolated to either connectivity (Opal) or performance (ASUS)
- **Scalability:** VR requirements can grow without affecting upstream connectivity
- **Maintenance Simplification:** Each tier can be maintained and updated independently

#### Network Segmentation Benefits

The cascaded configuration creates natural network segmentation:
- **Tier 1 (Opal):** Handles institutional network compatibility and security requirements
- **Tier 2 (ASUS):** Provides VR-optimized local network services
- **Traffic Flow:** All VR traffic is aggregated through the Opal, simplifying institutional network monitoring

### Network Architecture Design

#### Physical Connection Topology

The physical connection between routers is crucial for optimal performance:
- **Opal LAN Port → ASUS WAN Port:** This creates a proper LAN-to-WAN cascade
- **Cable Requirements:** Use CAT6 or better ethernet cable for gigabit performance
- **Cable Length:** Keep connections under 100 meters for optimal signal integrity

#### IP Addressing Strategy for Cascaded Setup

**Tier 1 (GL.iNet Opal) - 192.168.8.x:**
- **Router IP:** 192.168.8.1
- **DHCP Range:** 192.168.8.100 - 192.168.8.150 (limited range for ASUS router and management devices)
- **Upstream Connection:** Receives IP from institutional network via DHCP or static assignment

**Tier 2 (ASUS Router) - 192.168.10.x:**
- **WAN IP:** 192.168.8.100 (assigned by Opal)
- **LAN IP:** 192.168.10.1
- **VR Device Range:** 192.168.10.100 - 192.168.10.200
- **Administrative Range:** 192.168.10.20 - 192.168.10.50

This addressing scheme ensures no IP conflicts while maintaining clear separation between network tiers.

### Step-by-Step Configuration Process

#### Phase 1: Opal Configuration (Tier 1 Setup)

1. **Institutional Network Connection**
Configure the Opal in repeater mode to connect to the institutional WiFi network following the procedures outlined in Configuration 2. Verify stable connectivity before proceeding to ASUS configuration.

2. **IP Address Adjustment**
While the Opal defaults to 192.168.8.1, verify this doesn't conflict with the institutional network. If the institution uses the 192.168.8.x range, change the Opal to an alternative like 192.168.5.1.

3. **DHCP Configuration for Cascade**
Navigate to **NETWORK → DHCP** and configure:
- **DHCP Range:** 192.168.8.100 - 192.168.8.150
- **Lease Time:** 24 hours (provides stability for the ASUS router)
- **Gateway:** 192.168.8.1 (the Opal itself)
- **DNS Servers:** 8.8.8.8 and 8.8.4.4 (or institutional DNS if required)

4. **Quality of Service Pre-configuration**
Configure QoS to prioritize traffic from the ASUS router:
- Identify the ASUS router by its MAC address
- Assign it to the highest priority class
- Allocate 80-90% of available bandwidth to the ASUS router

#### Phase 2: ASUS Router Configuration (Tier 2 Setup)

1. **Physical Connection Establishment**
Connect an ethernet cable from any LAN port on the Opal to the WAN port on the ASUS router. The ASUS should automatically detect the connection and attempt to obtain an IP address via DHCP.

2. **Initial ASUS Setup**
Access the ASUS router at its default IP (192.168.1.1) initially. Run the Quick Internet Setup wizard, which should automatically detect the internet connection through the Opal.

3. **Network Addressing Configuration**
To prevent IP conflicts and improve network organization:
- Navigate to **Advanced Settings → LAN → LAN IP**
- Change the LAN IP to 192.168.10.1
- Set subnet mask to 255.255.255.0
- The router will reboot; reconnect using the new IP address

4. **DHCP Configuration for VR Devices**
Configure DHCP to serve VR devices:
- **DHCP Range:** 192.168.10.100 - 192.168.10.200
- **Default Gateway:** 192.168.10.1 (the ASUS router)
- **DNS Servers:** 8.8.8.8 and 8.8.4.4 (or institutional requirements)
- **Lease Time:** 12 hours (appropriate for devices that may power off overnight)

### Advanced Integration Optimization

#### Wireless Channel Coordination

To minimize interference between the two routers:

**Opal Channel Configuration:**
- **2.4GHz:** Use channel 1, 6, or 11 based on institutional network environment
- **5GHz:** Use lower channels (36-48) for institutional connectivity

**ASUS Channel Configuration:**
- **2.4GHz:** Use a different channel from the Opal (if Opal uses 6, ASUS uses 1 or 11)
- **5GHz:** Use higher channels (149-165) for VR devices

This separation reduces interference and improves overall wireless performance.

#### Quality of Service Coordination

**Opal QoS Configuration:**
Focus on ensuring the ASUS router gets consistent, high-priority access:
- **ASUS Router Priority:** Highest available priority
- **Bandwidth Allocation:** Reserve 80-90% of available bandwidth for ASUS router
- **Traffic Shaping:** Enable traffic shaping to smooth data flow

**ASUS QoS Configuration:**
Focus on VR-specific optimization:
- **Gaming Mode:** Enable for low-latency VR traffic
- **Device Prioritization:** Assign VR devices to highest priority categories
- **Bandwidth Management:** Allocate bandwidth based on VR device requirements

#### Performance Monitoring and Optimization

**Expected Performance Characteristics:**
- **Wireless Throughput:** 400-600 Mbps to VR devices (depending on institutional connectivity)
- **Latency Overhead:** 5-10ms additional latency through the cascade
- **Concurrent VR Users:** 4-8 simultaneous VR sessions depending on content complexity

**Performance Monitoring Points:**
1. **Opal Performance:** Monitor connection stability to institutional network
2. **Inter-Router Performance:** Monitor ethernet connection between routers
3. **ASUS Performance:** Monitor VR device connectivity and performance
4. **End-to-End Performance:** Test complete path from VR device to internet

### Troubleshooting the Cascaded Configuration

#### Common Issues and Solutions

**Problem: ASUS Router Cannot Access Internet**
- **Check Physical Connection:** Verify ethernet cable from Opal LAN to ASUS WAN
- **Verify IP Assignment:** ASUS WAN should receive IP in 192.168.8.x range
- **Test Opal Connectivity:** Ensure Opal can access internet independently

**Problem: VR Devices Have Poor Performance**
- **Check Wireless Channels:** Ensure ASUS uses different channels from Opal
- **Verify QoS Configuration:** Confirm VR devices have priority on ASUS router
- **Monitor Bandwidth Usage:** Use router statistics to identify bandwidth consumers

**Problem: Cannot Access Router Management Interfaces**
- **Document IP Addresses:** Keep clear records of each router's IP address
- **Use Correct Subnets:** Connect to each router from appropriate network segment
- **Browser Cache Issues:** Clear browser cache if switching between router interfaces

#### Maintenance and Updates

**Firmware Update Strategy:**
- **Update Opal First:** Ensure institutional connectivity remains stable
- **Test Connectivity:** Verify internet access before updating ASUS router
- **Update ASUS Second:** Update during low-usage periods to minimize VR disruption
- **Rollback Planning:** Keep previous firmware versions available for rollback if needed

**Configuration Backup Procedures:**
- **Export Configurations:** Save configurations from both routers monthly
- **Document Changes:** Keep log of all configuration changes with dates and reasons
- **Test Restoration:** Periodically test configuration restoration procedures

### Why This Configuration Works Well for VR Deployments

The Opal + ASUS cascaded setup addresses the fundamental challenge of institutional VR deployments: balancing institutional network requirements with VR performance needs. The Opal handles the "diplomatic" work of connecting to institutional networks with their various authentication, security, and policy requirements. Meanwhile, the ASUS router focuses entirely on creating the optimal environment for VR applications.

This separation of concerns provides several key benefits:

**Institutional Compliance:** The Opal presents a single, manageable connection point to the institutional network, making it easier to comply with institutional policies while maintaining the flexibility needed for VR operations.

**VR Performance Optimization:** The ASUS router can be configured specifically for VR requirements without compromising institutional network compatibility. WiFi 6 features provide the multi-device, high-bandwidth capabilities essential for quality VR experiences.

**Troubleshooting Clarity:** When issues arise, the two-tier architecture makes it easier to determine whether problems are related to institutional connectivity (Opal tier) or VR performance (ASUS tier). This separation significantly reduces the time needed to identify and resolve network issues.

**Scalability and Future-Proofing:** As VR requirements evolve or institutional network policies change, each tier can be upgraded independently. The modular design allows for technology refresh without complete network reconfiguration.
