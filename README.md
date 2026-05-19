# DNS Server

A Python implementation of a DNS server that handles UDP-based DNS queries. Built as part of NYU Tandon's Introduction to Computer Networking coursework.

## What it does

- Listens for incoming DNS queries over UDP
- Parses the DNS query header and question section
- Constructs and returns a DNS response with the appropriate answer records
- Implements core DNS protocol fields (transaction ID, flags, question/answer counts, TTL, etc.) according to RFC 1035

## How to run

```bash
python DNSServer.py
```

The server listens on a UDP socket and responds to incoming DNS queries from a DNS client.

## What I learned

- DNS message format at the byte level (header, question, answer, authority, additional sections)
- UDP socket programming in Python
- Encoding and decoding binary network protocols
- How recursive vs iterative DNS resolution works in practice

## Tech stack

- Python 3
- `socket` library (UDP)
- `struct` library (binary packing/unpacking)
