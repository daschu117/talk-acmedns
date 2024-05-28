# Automating DNS-01 The Less Lazy Way (with acme-dns)
### Presented at [LayerOne](https://www.layerone.org/) 2024-05-26

The ACME protocol used by Let’s Encrypt and other Certificate Authorities is used for domain ownership validation and distributing zero-cost TLS certificates.
While the HTTP-01 Challenge can be the easiest to deploy, the DNS-01 Challenge can be used to procure a certificate for non-HTTP services, internal services, or services requiring a wildcard certificate.
However, automating the DNS-01 challenge requires a compatible DNS hosting service with an API, and may require storing your password or API credentials in cleartext on every server that you automate. 

The acme-dns project provides an alternate way to automate the DNS-01 challenge with any DNS hosting service, on a per-domain basis, while eliminating the need for administrative API credentials.
It’s extremely useful for Homelab users, but may also have a place in corporate environments without public-facing services.

https://github.com/joohoi/acme-dns
