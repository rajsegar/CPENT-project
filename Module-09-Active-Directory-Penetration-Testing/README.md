# Module 09: Active Directory Penetration Testing

## In plain language

Active Directory (AD) manages identities, computers, groups, policy, and trust
for many Windows environments. AD testing looks for paths where ordinary
permissions, configuration, or credentials combine to grant unintended control.

## Key ideas

| Term | Beginner-friendly meaning |
| --- | --- |
| Domain | An administrative and security boundary for directory objects |
| Domain controller | A server that provides directory and authentication services |
| Security principal | A user, computer, group, or service identity |
| Group Policy | Central configuration applied to users and computers |
| Kerberos | A ticket-based authentication protocol used by AD |
| NTLM | An older challenge-response authentication family |
| Trust | A relationship that permits identities in one boundary to be recognized in another |
| Attack path | A chain of permissions or conditions leading to a sensitive objective |

## A safe assessment approach

1. Confirm the approved domains, forests, accounts, and systems.
2. Record the starting identity and group memberships.
3. Map directory objects, privileged groups, trusts, and administrative tiers.
4. Review delegated permissions and Group Policy relationships.
5. Identify a possible path to a defined objective.
6. Validate only the minimum link needed by the lab or rules of engagement.
7. Document the chain, affected identities, detection, and remediation.

AD risk often comes from combinations. A permission that appears harmless may
be dangerous when it controls a group, policy, computer, or service trusted by
a more privileged identity.

## Common mistakes

- Treating every domain user as equivalent.
- Looking only at direct membership in privileged groups.
- Ignoring nested groups, delegation, trusts, and service identities.
- Collecting more directory or credential data than the scope permits.
- Calling a theoretical graph path exploitable without validating assumptions.
- Changing group membership without a rollback and approval.

## Defender view

Important defenses include administrative tiering, protected privileged
accounts, managed service identities, restricted delegation, careful access
control, modern authentication, local administrator management, useful domain
controller logging, and periodic attack-path review.

## Quiz

1. Why are AD findings often described as paths rather than isolated issues?
2. What is a security principal?
3. Why can nested group membership matter?
4. Does a graph relationship automatically prove exploitation?
5. What should be recorded before changing a lab group membership?

## Answer key

1. Several individually limited permissions or conditions may chain together
   to reach a privileged objective.
2. An identity recognized by the security system, such as a user, computer,
   group, or service.
3. A user can inherit effective access through groups contained inside other
   groups.
4. No. The edge may depend on assumptions, unavailable access, mitigations, or
   stale data and should be validated safely.
5. Authorization, current membership, intended change, expected impact,
   timestamps, and exact rollback steps.

## Flashcards

**Q:** What does a domain controller do?  
**A:** It provides directory, authentication, and related policy services for a domain.

**Q:** What is an attack path?  
**A:** A chain of verified relationships that leads from starting access to a security objective.

**Q:** Why are service accounts important?  
**A:** Services may hold privileges, access resources, and depend on long-lived identity configuration.

**Q:** What does Group Policy affect?  
**A:** Central settings applied to selected users and computers.

**Q:** What is the safest claim for an unvalidated graph edge?  
**A:** It is a candidate relationship requiring verification, not proven impact.

## Safe practical exercise

Use a private, resettable AD lab. With a provided low-privilege test account,
create a diagram of:

- The domain and domain controller.
- Three users, three groups, and two computers.
- Direct and nested memberships.
- One delegated permission.
- One sensitive objective.

Explain a possible path and list the evidence needed to validate each link.
Validate only actions explicitly assigned by the lab. Revert any group or policy
change and confirm the original state.

## Completion checklist

- [ ] I can explain domains, principals, groups, policy, and trust.
- [ ] I can reason about a multi-step permission path.
- [ ] I distinguish candidate relationships from proven impact.
- [ ] I completed and restored a private AD lab.
