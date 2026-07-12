# Reconnaissance Report

## Objective

Perform passive reconnaissance to understand the publicly exposed attack surface before any active testing.

---

# Target

```
dodopayments.tech
```

---

# Methodology

Only passive information gathering techniques were considered.

Tools used / evaluated:

- crt.sh
- nslookup
- dig
- whois
- subfinder
- assetfinder
- amass
- httpx
- whatweb
- testssl.sh

---

# Information Collected

## Domain

- Public website reachable over HTTPS

## DNS

Public DNS records identified through passive enumeration.

## Certificate Transparency

Certificate Transparency logs were reviewed to identify publicly known certificates and associated hostnames.

## HTTP Fingerprinting

Technology fingerprinting was performed to identify publicly visible technologies.

## TLS Configuration

TLS configuration was reviewed for protocol and certificate information.

---

# Risk Assessment

No intrusive testing was performed during the reconnaissance phase.

The primary objective was to understand the exposed attack surface while respecting the assessment scope.

---

# Recommendations

- Regular attack surface monitoring
- Continuous certificate transparency monitoring
- Periodic DNS inventory review
- Minimize unnecessary public endpoints
- Enforce modern TLS configuration

---

# Conclusion

Passive reconnaissance provides valuable insight into the external attack surface without interacting aggressively with production systems.