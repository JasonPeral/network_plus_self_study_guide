### What is the session layer?

- Manages sessions, ensuring separate conversations to prevent data intermingling

### Setting up a session

- We have to check a user credentials and assign a number to the session to help identify them.
- Basically a random number that we use to negotiate services for this session with the server and we use this number to get negotiate who is going to talk first.

### Maintain the session

- Continuous data transfer between parties
- If the connection breaks we will have to re-establish the connection
- Includes acknowledgement of data

### Tearing down a session

- Ending a session once communication goals are achieved
- Mutual agreement or one party disconnects

### Layer 5 Devices and Protocols

- **H.323**
    - Used for setting up, maintaining and tearing down voice and video connections
    - Operates over the real-time transport protocol (RTP)
        - Whenever we see RTP we should think stream audio and streaming video in a 2 way format like a phone call or a facetime call
- **NetBIOS**
    - Used by computers for file sharing over a network
    - Commonly associated with windows file sharing

## Layer 5 issues involve protocols and software rather than specific devices
