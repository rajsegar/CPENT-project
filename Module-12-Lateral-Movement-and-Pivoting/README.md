# Module 12: Lateral Movement and Pivoting

## In plain language

Lateral movement uses approved access on one system to reach or act on another.
Pivoting routes assessment traffic through an intermediate system or network
path. Both test whether segmentation, credentials, administration paths, and
monitoring limit the spread of a compromise.

## Key ideas

| Term | Beginner-friendly meaning |
| --- | --- |
| Foothold | The authorized starting access on a system |
| Lateral movement | Moving from one security context or host to another |
| Pivot | An intermediate system or path used to reach another network |
| Jump host | A managed system intended for administrative access |
| Tunnel | A connection that carries one kind of traffic through another path |
| Proxy | A service that forwards requests on behalf of a client |
| Route | A rule describing where network traffic should go |
| Double pivot | A path through two intermediate points |

## A safe assessment approach

1. Draw the approved source, destination, intermediate systems, and zones.
2. Record the foothold identity and network reachability.
3. Define the exact business objective and stopping point.
4. Test the smallest approved path.
5. Record authentication events, routes, connections, and defender telemetry.
6. Avoid unrelated systems and data encountered along the way.
7. Remove routes, tunnels, listeners, files, and credentials during cleanup.

Lateral movement and pivoting are not synonyms. You can authenticate to another
host without routing arbitrary traffic through the first host, and you can
route through a host without gaining a new identity on the destination.

## Common mistakes

- Adding a broad route when only one destination is in scope.
- Forgetting that a pivot changes the apparent network source.
- Reusing credentials outside their approved systems.
- Leaving tunnels or listeners running after the test.
- Assuming network reachability proves authorization or authentication.
- Losing track of which host produced each log and timestamp.

## Defender view

Defenses include strong segmentation, managed administrative paths,
phishing-resistant authentication, unique local credentials, restricted remote
services, endpoint telemetry, network-flow monitoring, egress controls, and
alerts on unusual authentication patterns.

## Quiz

1. What is the difference between lateral movement and pivoting?
2. Why should a route be as narrow as possible?
3. Does network reachability prove permission to access a host?
4. What should an evidence timeline record in a multi-host test?
5. Name four items that may require cleanup.

## Answer key

1. Lateral movement gains or uses access on another system; pivoting forwards
   traffic through an intermediate path.
2. A narrow route reduces unintended contact with out-of-scope systems and
   makes evidence easier to interpret.
3. No. Scope and authorization remain separate from technical reachability.
4. Host, identity, action, source and destination, timestamp and zone, result,
   and corresponding log or evidence.
5. Examples include routes, tunnels, proxies, listeners, temporary files,
   accounts, credentials, and configuration changes.

## Flashcards

**Q:** What is a foothold?  
**A:** The starting access from which the authorized assessment proceeds.

**Q:** What does a pivot change?  
**A:** The network path used to reach a destination.

**Q:** What does lateral movement change?  
**A:** The host or security context on which the tester can act.

**Q:** What is a double pivot?  
**A:** A route that passes through two intermediate points.

**Q:** What is the key cleanup principle?  
**A:** Remove every temporary path and verify the original state.

## Safe practical exercise

Use an isolated multi-VM lab with one assigned jump host and one assigned
destination. Draw the zones and complete a reachability matrix before making
changes. Follow the lab's approved method to demonstrate one narrow connection
through the jump host.

Capture endpoint and network logs, then remove the temporary path and prove it
no longer exists. Do not add routes covering unrelated subnets.

## Completion checklist

- [ ] I can distinguish reachability, pivoting, authentication, and lateral movement.
- [ ] I can draw and explain a multi-hop path.
- [ ] I can collect evidence from each side of a connection.
- [ ] I completed cleanup and verified the original lab state.
