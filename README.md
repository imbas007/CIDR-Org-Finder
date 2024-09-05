The CIDR and Organization Finder is a Python script designed to retrieve CIDR (Classless Inter-Domain Routing) blocks and associated organization information for given IP addresses. 

## Features

    Retrieves CIDR blocks and organization names for IP addresses
    Uses multiple WHOIS data sources: CYMRU, ARIN, and IPWhois
    Implements a retry mechanism for resilience against temporary failures
    Provides asynchronous processing for improved performance
    Supports rate limiting to avoid overloading WHOIS servers
    Offers options for searching specific organizations and outputting raw data
    Groups and sorts results by organization and CIDR
    
## Installation
1. Clone this repository
```
git clone 
```
2. Make the script executable:
```
chmod +x cscan.py
sudo mv cscan.py /usr/bin/cscan
```

### Basic Usage

```
cat ip_list.txt | cscan
```

3. Combine with other tools:
```
subfinder -silent -d example.com | dnsx -silent -a -resp-only | cscan
```

credit: https://github.com/nullenc0de/netscan
