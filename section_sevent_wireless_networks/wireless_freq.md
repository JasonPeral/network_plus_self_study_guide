# Wireless Frequencies

### Core summary

- This topic refers to different frequency bands used to transmit and receive radio waves in wireless networking
- Different frequency bands have different characteristics related to speed, coverage and regulations to prevent interference

Different bands include:

1. 2.4 GHz Band - 
2. 5 GHz Band - 
3. 6 GHz Band - 

Channels that you can utilize in you 802.11 network based on your geo location 

Check with local government regulations but this is the standard below: 

- US and Canada — channels 1 - 11
- Japan — channels 1 - 14
- Rest of the world — channels 1 - 13

---

### 2.4 GHz Band

- Long range and better Penetration through solid objects
- Frequency ranges from 2.400 GHz to 2.495 GHz
- Ranges are divided into channels(given a certain channel width) which overlap in this band which causes interference
    - Can have channels of up to  11 to 14 depending on your geo location
    - When we say Channels we refer to the specific frequency ranges within the 2.4 GHz band that wireless networks use to send and receive data
        - The frequencies are actually part of the electromagnetic spectrum which is the physical medium in wireless communication.
    - Channels that don’t have overlap that are advisable to use to avoid interference:
        - Channel 1, 6 and 11
            
            ![Screenshot 2025-06-06 at 12.58.50 PM.png](attachment:861170f3-f0c2-4346-a24f-546abf221f3b:Screenshot_2025-06-06_at_12.58.50_PM.png)
            

### 5 GHz Band

- Faster data transfers and speed but with shorter range and less penetration capabilities than the 2.4 band
- Frequencies range from 5.1 to 5.7 GHz or 5.875 GHz providing up to 24 channels with no overlap with each channel being 20 MHz
    
    **Channel Bonding**
    
    - Creates wider channels by merging 2 or more neighbouring channels together to create a single wider channel
    - Increases bandwidth but has a higher chance of interference due to increased channel widths

### 6 GHz Band

- Latest spectrum for wireless network. Has more channels and bandwidth which allows for faster connection and less congestion
- Frequency ranges from 5.925 GHz to 7.125 GHz
- 1200 total MHz which allows for channels of 20, 40, 80 or 160 Mhz in width which can accommodate up to 59 channels when using the 20 MHz width and 7 channels when using the 160 MHz width

### Government regulation and standards

- GOV allocates portions of the wireless spectrum for wireless networking with it varying globally
    - These regulation are due to controlling the Frequency environment to ensure that networks are not interfering with military radars or hospital equipment

**802.11h Standard**

- Developed to comply with EU regulation
- **Dynamic Frequency Selection (DFS)**
    - Requires devices to actively monitor the environment for any radar signals
    - If radar signals are detected the device that is being used will switch channels
- **Transmit Power Control (TPS)**
    - Allows devices to adjust their transmitting power to a minimum level that allows for devices to maintain good quality.
    - This reduces interference with other frequencies and lowers power consumption

**Band Steering**

- This tech optimizes the distribution of client devices on different frequency bands
- Automatically detects devices that are able/ compatible to operate on the less congested bands like 5ghz or 6ghz and steer them over accordingly
- Can result in more efficient use of bandwidth and leaves the 2.4GHz band for the devices that can only operate there.