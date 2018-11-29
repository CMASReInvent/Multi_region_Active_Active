# Active Active is hard
- Insight: You can get four 9s of availability with AZs only
- Insight: Before choosing Active Active Consider other arch and business needs


# Reasons for Active Active:
- Business Continuousity / Disaster Recovery
- Geographically distribution customer
-- Improve latency
-- Legal Requirements
-- Temporary Active Active because of Blue/Green

# Multi-region Architectures options:
- Backup & Restore -- Under 24 hours
- Pilot Light --> Allows for redundant failure (DNS Failover) -- downtime is in hours
- Warm Standby --> Smaller scale architecture -- downtime is in minutes
- Active Active --> No downtime

# Active Active Pattern
- Read local, Write global
- Read local, write Partition
- Read local, write local

# Managed Services that help networking
Route 53
-- health checks
-- traffic routing
AWS Global Accelerator
-- Static Global IP
-- Intelligent Traffic Distribution
-- Enhanced Fault Tolerance
-- TCP & UDP
-- Instance region Failover
Multi-region VPC
Control Tower

# Management Tooling
AWS Cloudformation StackSets
AWS Config
AWS System Manager

