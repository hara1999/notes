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

---

# What is the Difference Between SQL and NoSQL?

## 1. SQL Databases
SQL databases are relational databases that use structured schemas and tables to store and manage data. They rely on SQL for querying and managing the database.

### Characteristics:
* **Data Storage:**
    * Tabular format (rows and columns).
* **Transactions:**
    * ACID (Atomicity, Consistency, Isolation, Durability) compliance ensures strong consistency.

### Advantages:
1. **Structured Data:** Ideal for applications where the data has a clear structure (e.g., financial data, ERP systems).
2. **Strong Consistency:** Ensures data integrity through ACID compliance.

### Disadvantages:
1. **Scalability:** Vertical scaling (adding more power to a single server) is the primary scaling model, which can be costly.
2. **Rigidity:** Changing schemas or handling unstructured data can be challenging.

---

## 2. NoSQL Databases
NoSQL databases are non-relational databases designed for scalability and flexibility. They handle unstructured, semi-structured, or structured data.

### Characteristics:
* **Data Storage:**
    * Various formats: Key-Value pairs, Document, Column-family, Graph.
* **Transactions:**
    * Often follow BASE (Basically Available, Soft state, Eventual consistency), allowing for relaxed consistency models.
* **Query Language:**
    * Varies by database type (e.g., query-based on JSON or key-value lookups).

### Types of NoSQL Databases:
1. **Key-Value Store:** Data stored as key-value pairs (e.g., Redis, DynamoDB).
2. **Document Store:** JSON-like documents (e.g., MongoDB, CouchDB).
3. **Column-Family Store:** Optimized for large datasets (e.g., Cassandra, HBase).
4. **Graph Databases:** Represent relationships between data (e.g., Neo4j, ArangoDB).

### Advantages:
1. **Scalability:** Horizontal scaling (adding more servers) makes it easy to handle large datasets and high traffic.
2. **Flexibility:** Handles unstructured or semi-structured data (e.g., JSON, XML).
3. **Performance:** Optimized for specific use cases like high-speed lookups or complex graph queries.

### Disadvantages:
1. **Weaker Consistency:** Often trades off strong consistency for performance and availability.
2. **Less Mature Ecosystem:** Fewer standardized tools and practices compared to SQL.


