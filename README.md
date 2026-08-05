
# Cross-Tenancy Boot Volume Backup Migration Between Oracle Cloud Infrastructure (OCI) Tenancies

A practical guide demonstrating one approach to migrate Oracle Cloud Infrastructure (OCI) compute instances between two different OCI tenancies using Boot Volume Backups.

> This repository accompanies the Medium article:
>
> **Cross-Tenancy Boot Volume Backup Migration: One Approach to Migrating Compute Instances Between OCI Tenancies**

---

## Overview

Organizations may need to migrate compute workloads between OCI tenancies due to:

- Cloud environment separation
- Business mergers
- Organizational restructuring
- Managed service provider changes
- Landing Zone redesign

This guide demonstrates how to migrate an OCI Compute Instance by restoring a Boot Volume Backup into another tenancy.

---




## Architecture


<img width="2400" height="1260" alt="linkedin-cross-tenancy-migration" src="https://github.com/user-attachments/assets/099367be-0a44-4f61-997a-edbd7853fc83" />

---

## Migration Workflow

Source Tenancy

↓

Create Boot Volume Backup

↓

Configure Cross-Tenancy IAM Policies

↓

Restore Backup into Target Tenancy

↓

Create Boot Volume

↓

Launch New Compute Instance

↓

Validate Migration

---

## Repository Contents

| Folder | Description |
|---------|-------------|
| diagrams | Architecture diagrams |
| policies | Cross-tenancy IAM policies |
| cli | OCI CLI examples |
| screenshots | Step-by-step screenshots |
| docs | Detailed documentation |

---

## Prerequisites

- Source and target OCI tenancies
- Appropriate IAM permissions
- OCI CLI configured
- Network connectivity in target tenancy
- Compatible availability domain

---

## Migration Steps

1. Create Boot Volume Backup
2. Configure Cross-Tenancy Policies
3. Restore Backup in Target Tenancy
4. Create Boot Volume
5. Launch Compute Instance
6. Validate the Instance
7. Clean up unused resources

---

## Advantages

- Native OCI functionality
- No third-party tools
- Minimal downtime
- Secure migration
- Preserves operating system and configuration

---

## Limitations

- Region limitations apply
- Requires IAM configuration
- Network configuration must be recreated
- Public IPs are not preserved

---

## Related Documentation

- Oracle Documentation
- OCI Volume Migration Guide

---

## Medium Article

Read the complete walkthrough on Medium:
https://medium.com/@sayeedamodix/cross-tenancy-boot-volume-backup-migration-one-approach-to-migrating-compute-instances-between-oci-84c0b2c96773

---

## Author

**Sayeed Al Amodi**

Oracle Cloud Infrastructure (OCI)

Oracle ACE Apprentice

Medium: https://medium.com/@sayeedamodix

LinkedIn: https://linkedin.com/in/sayeedamodi

---

## License

MIT
