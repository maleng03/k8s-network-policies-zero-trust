# Ì∫Ä Kubernetes NetworkPolicies ‚Äî Zero Trust Architecture

## Ì≥å Overview
This project demonstrates how to implement zero-trust networking in Kubernetes using NetworkPolicies.

A default deny-all policy is applied, and only required service-to-service communication is explicitly allowed.

## Ìª†Ô∏è Tech Stack
- Kubernetes (kind)
- Calico CNI
- NetworkPolicies
- Google Online Boutique microservices app

## Ì¥ê Security Model
1. Default deny all ingress and egress traffic
2. Allow DNS resolution
3. Allow only required service-to-service communication

## Ì≥Ç Policies Included
- deny-all.yaml
- allow-dns-egress.yaml
- allow-frontend-egress.yaml
- allow-productcatalog-ingress.yaml
- allow-cart-to-redis.yaml

## Ì∑™ Testing Approach
- Used debug pod (BusyBox) for connectivity testing
- Verified blocked and allowed traffic paths using telnet and nc

## ÌæØ Key Skills Demonstrated
- Kubernetes NetworkPolicies
- Zero Trust Architecture
- Microservices security
- Troubleshooting networking issues
- Working with CNI (Calico)

## Ì≥∏ Result
- Unauthorized lateral traffic blocked
- Only required services communicate
- Application remains fully functional

