# VLAN Configurations

- Core Summary Of Section
- Recall Qs
- Core Notes
    
    ### 802.1Q (VLAN) Tagging
    
    - This concept refers to the IEEE standard that enables the management of multiple VLANs on a singular network
    - VLAN TAGGING
        - This works by inserting a VLAN tag into an ethernet frame which enables our switch to identify and forward the frames to the proper VLAN associated with with the tag
        - Each tag will contain a VLAN Identifier (VID) which allows our switch to distinguish one VLAN from another. (Also allows for trunking)
        - In an enterprise environment, tagging is used to create logical separations between different departments like HR, Accounting, DEV, IT which allows for different security measures to be put into place that may be specific to their daily work
    - VLAN TRUNKING
        - Allows the transmission of traffic from different VLANs across the same physical network infrastructure while keeping the traffic from each VLAN separate, isolated and secure
        - Chat GPT response if still confused: **Trunking allows traffic from multiple VLANs — including the *same VLAN ID* across multiple switches — to be carried over the same physical link, while preserving the separation of each VLAN logically.**
        
    
    ---
    
    ### Native VLAN (Default)
    
    - Is the only VLAN on a trunk port that does not get a VLAN tag(VID) when frames are sent out and also its the VLAN that untagged frames are assigned to when frames are received on a trunk
    - Basically the default VLAN for frames that come untagged
    - Frames may come in untagged when devices don’t support VLAN tagging especially legacy systems
    - The native VLAN should be configured to route consistently between interconnected switches to avoid misrouting
    
    ```mermaid
    graph TD
      Untagged_Frame --> Trunk_Port
      Frame_VID1 --> Trunk_Port
      Frame_VID2 --> Trunk_Port
      Frame_VID3 --> Trunk_Port
      Trunk_Port --Frame_VID1--> VLAN_1
      Trunk_Port --Frame_VID2--> VLAN_2
      Trunk_Port --Frame_VID3--> VLAN_3
      Trunk_Port --> VLAN_4
      Trunk_Port --Untagged_Frame--> NATIVE_VLAN
    
    ```
    
    ---
    
    ### Voice VLAN
    
    - Specialized VLAN that is dedicated to voice traffic specifically VoIP traffic within the network
    - Segregation between voice traffic and data traffic ensures quality and reliability as voice traffic is highly sensitive to delays and packet loss
    - We can configure our switches to prioritize our voice traffic by enabling the quality of service application or QoS policies to optimize voice communications(Continuity and clarity) even when the network is under heavy load.
    
    ---
    
    ### Link Aggregation
    
    - Also known as port channeling or bonding is a method that combines multiple network connections into a single logical link
    - Link aggregation enhances bandwidth capacity and also redundancy for higher levels of network availability
    - By combining multiple network connections together we are able to distribute our data across multiple links in an organized manner so that we can utilize the combined bandwidth of all of the combined links
    - Link aggregation is commonly used for trunking lines between switches and for high-speed connectivity within data centers. For Example: if we were to aggregate four 1 Gbps links together we have a total of 4 Gbps of BW available on a single logical link.

    ---

    ### Speed and Duplex Configurations

    - These 2 configurations refer to the settings that determine the rate at which data is transmitted and also the mode of communications that will be used between the network devices
    - **SPEED →** refers to the rate of data that is being transmitted which is usually measured in Mbps or Gbps
    - **DUPLEX →** refers to how data is being sent over the connections
        - **HALF-DUPLEX →** Devices can send or receive data at any given time but cant do both simultaneously (random example: Walkie Talkies)
        - **FULL-DUPLEX →** Devices can send or receive data simultaneously
            - This will help our overall network transfer speed because it effectively doubles our network capacity when compared with half duplex mode
    - Misconfiguration of speed and duplex mode can significantly impact the networks performance and data throughput.
        
        > **For example if the a high performing server can handle 1Gbps throughput and full duplex mode but is only configured for 100Mbps and a half duplex config then there is a lot left on the table and presents potential network congestions.**
        > 

    ---

    ### Auto-Negotiation

    - A feature that allows network devices and non network devices to automatically choose the best possible speed and duplex settings when connecting to each other
        - Simply: when 2 ethernet devices are connected || Switch ←→ Server || they says heres what I support what do you? then agrees on the fastest most reliable options that both devices support
    - Manual configuration may be preferred in certain situations with legacy equipment or if theres certain performance requirements.