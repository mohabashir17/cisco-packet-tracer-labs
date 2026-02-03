## Topic
Static Route Troubleshooting

## Goal
Identify and fix static route misconfigurations to restore end-to-end connectivity
in a network with three routers.

## Topology
- Three routers connected in series
- Each router had one static route misconfiguration
- End networks located behind the edge routers

## Problem
Connectivity between the end networks was not working due to incorrect static route
configurations on all three routers.

## Troubleshooting Process
- Examined routing tables using `show ip route`
- Identified missing or incorrect static routes
- Corrected next-hop IP addresses and destination networks

## Solution
- Fixed static routes on all three routers
- Ensured each router had a correct route to the remote networks

## Verification
- Verified routing tables using `show ip route`
- Confirmed all networks are reachable
- Successful end-to-end ping after fixing the routes

## What I Learned
- Static routes must have correct destination networks and next-hop addresses
- A single wrong static route can break end-to-end connectivity
- `show ip route` is essential for troubleshooting routing issues

