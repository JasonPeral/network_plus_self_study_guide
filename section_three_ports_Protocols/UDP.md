# User Datagram Protocol (UDP)

### Communication Protocol
- Used for time-sensitive transmissions on the internet
- Ideal for applications prioritizing speed over error checking
- Low latency and reduced processing overhead
- Lacks error checking and recovery services like TCP

### Transport Layer Operation
- Operates at the transport layer, similar to TCP
- Uses a connectionless communication model

## Packet Structure

### Datagrams
- Term for data packets in UDP
- Sent without prior setup of transmission channels
- Contains:
  - Source and destination port numbers
  - Length field
  - Checksum
- Smaller and simpler headers (8 bytes) compared to TCP (20-60 bytes)

## UDP’s Stateless Nature
- Does not maintain connection state or track packets
- Often referred to as a "fire and forget" protocol
- No waiting for acknowledgments, leading to faster transfer rates

## Reliability Trade-off
- Less reliable due to lack of packet tracking
- Suitable for scenarios where speed is crucial, and packet loss is acceptable

## Use Cases
- Used in applications like:
  - Live broadcasts
  - Online gaming
  - VoIP calls
- Effective for simple request-response communications (e.g., DNS lookup)

## Additional Notes
- UDP utilizes ports to differentiate between multiple services on the same client/server
- UDP relies on application-level error handling due to lack of built-in error recovery
- Contains a checksum in the header for minimal protection against data corruption
- Not as robust as TCP in ensuring data integrity and delivery
