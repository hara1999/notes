# What is TCP and UDP?

## 1. TCP (Transmission Control Protocol)
TCP is a connection-oriented protocol that provides reliable communication by establishing a connection before data transfer and ensuring the data is delivered correctly and in order.

### Key Features:
1. **Connection-Oriented:**
    * A connection must be established between the sender and receiver (via a handshake) before data is sent.
2. **Reliable:**
    * Ensures data is delivered without errors, in sequence, and without duplicates.
    * Uses acknowledgments (ACKs) and retransmissions in case of data loss.
3. **Ordered Delivery:**
    * Data packets arrive in the order they were sent.
4. **Flow Control and Congestion Control:**
    * Adjusts data transmission speed based on network conditions and receiver capacity.

### Use Cases:
* Applications requiring reliability and accuracy:
    * Web browsing (HTTP/HTTPS)
    * Email (SMTP, IMAP, POP3)
    * File transfers (FTP)
    * Remote access (SSH, Telnet)

### Example of TCP in Action:
* Web browsing: TCP ensures that all parts of a webpage arrive correctly and in order.

---

## 2. UDP (User Datagram Protocol)
UDP is a connectionless protocol that provides a fast but less reliable way to send data. It does not establish a connection or guarantee delivery, making it lightweight and efficient.

### Key Features:
1. **Connectionless:**
    * No handshake or connection establishment between sender and receiver.
2. **Unreliable:**
    * No guarantees that packets will arrive, arrive in order, or be error-free.
    * No retransmissions or acknowledgments.
3. **Low Overhead:**
    * Faster and more efficient due to minimal protocol overhead.

### Use Cases:
* Applications requiring low latency and real-time data:
    * Video and audio streaming
    * Online gaming
    * VoIP (Voice over IP)
    * DNS (Domain Name System) queries

### Example of UDP in Action:
* Live streaming: UDP allows data to arrive quickly, even if some packets are lost, ensuring minimal latency.
