---  
title: "Microsoft 365 Connection Blockers in the Microsoft 365 admin center"  
description: Understanding Connection Error Rate and WSS Error Rate in Microsoft 365 Network Connectivity
author: kelleyvice-msft
ms.author: kvice  
manager: scotv
ms.date: 11/08/2024  
ms.topic: conceptual
ms.service: microsoft-365-enterprise  
ms.subservice: network  
ms.localizationpriority: medium
ms.collection:
- scotvorg
- Ent_O365
- Strat_O365_Enterprise
- must-keep
ms.custom: QuickDraft
ms.reviewer: roshanp  
search.appverid: MET150  
f1.keywords:  
audience:  
ai-usage: ai-assisted  
---  

# Microsoft 365 Connection Blockers in the Microsoft 365 admin center

In the network connectivity space, understanding error rates is crucial for maintaining optimal performance and enhancing user experience. This article aims to explain two significant error rates: the Connection Error Rate and the WSS Error Rate. Both metrics will be prominently displayed on the new Connection Blockers page in the Microsoft 365 admin center under Network Connectivity.

:::image type="content" source="../media/m365-mac-perf/m365-mac-perf-connection-blockers-main.png" alt-text="Microsoft 365 network connectivity connection blockers tool":::
 
## Connection Error Rate

The Connection Error Rate represents the percentage of connection attempts that fail when attempting to reach a specific domain. This metric is critical as it highlights the reliability and accessibility of resources hosted in a specific domain. A high connection error rate can indicate underlying issues that require prompt attention.

Understanding and monitoring the Connection Error Rate is vital for several reasons:

- Network Reliability: A high connection error rate can signal potential problems in the network infrastructure, such as DNS resolution failures, or misconfigurations that result in connections being blocked.
- User Experience: Frequent connection failures can lead to a poor user experience, affecting productivity and satisfaction.
- Performance Monitoring: Regular tracking allows administrators to identify trends and address issues proactively.

### Calculating Connection Error Rate

The Connection Error Rate is calculated using the formula:

- Connection Error Rate (%) = (Number of Failed Connections / Total Connection Attempts) x 100
For instance, if there are 50 failed connections out of 1000 attempts, the connection error rate would be:
- (50 / 1000) x 100 = 5%

### Common Causes of High Connection Error Rate

Various factors can contribute to a high connection error rate, including:

- DNS Issues: Problems with domain name resolution can prevent successful connections.
- Network Congestion: Overloaded networks can result in dropped packets and failed connections.
- Firewall Restrictions: Incorrectly configured firewalls can block legitimate traffic.
- Server Unavailability: Target servers being offline or experiencing outages.

### Mitigating Connection Error Rate

To reduce the connection error rate, consider the following strategies:

- DNS Configuration: Ensure DNS servers are correctly configured and reliable.
- Load Balancing: Use load balancers to distribute traffic evenly across servers.
- Network Optimization: Implement Quality of Service (QoS) policies to manage traffic effectively.
- Regular Monitoring: Continuously monitor network performance and address issues promptly.

## WSS Error Rate

The WSS (WebSocket Secure) Error Rate refers to the percentage of failed attempts to upgrade a connection to a WebSocket, a protocol that provides full-duplex communication channels over a single TCP connection. This metric is essential for applications relying on real-time data transmission.

Monitoring the WSS Error Rate is crucial for:

- Real-Time Applications: Applications such as chat systems, live updates, and online gaming rely heavily on WebSocket connections for real-time communication.
- Performance Insight: A high WSS error rate can indicate issues with the network or server configurations affecting real-time data flow.
- Security: WebSocket connections need to be secure (WSS) to ensure data integrity and privacy.

### Calculating WSS Error Rate

The WSS Error Rate is calculated similarly to the connection error rate:

- WSS Error Rate (%) = (Number of Failed WebSocket Upgrades / Total WebSocket Upgrade Attempts) x 100
For example, if there are 30 failed WebSocket upgrades out of 600 attempts, the WSS error rate would be:
- (30 / 600) x 100 = 5%

### Common Causes of High WSS Error Rate

Several factors can lead to a high WSS error rate, such as:

- SSL/TLS Issues: Problems with SSL/TLS certificates can prevent secure WebSocket connections.
- Firewall Restrictions: Firewalls blocking WebSocket traffic can cause upgrade failures.
- Network Latency: High latency can disrupt the WebSocket handshake process.
- Server Configuration: Incorrect server settings may reject WebSocket upgrade requests.

### Mitigating WSS Error Rate

To lower the WSS error rate, consider these approaches:

- SSL/TLS Configuration: Ensure SSL/TLS certificates are valid and correctly configured.
- Firewall Settings: Configure firewalls to allow WebSocket traffic.
- Latency Optimization: Reduce network latency by optimizing routes and using CDN services.
- Server Tuning: Adjust server settings to support WebSocket connections.

## Using Connection Blockers Page in Microsoft 365 Admin Center

The new Connection Blockers page in the Microsoft 365 Admin Center under Network Connectivity is designed to provide administrators with a comprehensive view of connection error rates and WSS error rates. This tool allows for proactive monitoring and troubleshooting.

### Navigating the Connection Blockers Page

To access the Connection Blockers page:

- Sign in to the Microsoft 365 Admin Center.
- Navigate to the Network Connectivity section.
- Select Connection Blockers from the menu.

### Interpreting the Data

The Connection Blockers page displays:

- Connection Error Rate: Visual representation of connection failure rates to specific domains.
- WSS Error Rate: Graphs and charts showing the rate of WebSocket upgrade failures.

Use this data to identify patterns, diagnose issues, and implement corrective measures.

## Conclusion

Both Connection Error Rate and WSS Error Rate are critical metrics for ensuring robust and reliable network performance. By understanding these rates and actively monitoring them through the Microsoft 365 Admin Center, administrators can enhance network reliability, improve user experience, and maintain secure, real-time communications. Proactive management and timely troubleshooting of these error rates will help in maintaining the health and efficiency of network operations.
