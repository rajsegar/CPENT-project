# Module 06: API and JSON Web Token Penetration Testing

## In plain language

An Application Programming Interface (API) lets software exchange structured
requests and responses. API testing checks whether each endpoint, action, and
data object is protected correctly. JSON Web Tokens (JWTs) are commonly used
to carry signed claims about identity and session context.

## Key ideas

| Term | Beginner-friendly meaning |
| --- | --- |
| Endpoint | A specific API route and method |
| Object | A record such as a user, invoice, or project |
| Claim | A named value carried in a token |
| Signature | Cryptographic proof that protected token content was issued by a trusted party |
| Expiry | The time after which a token should no longer be accepted |
| Schema | The expected shape and data types of a request or response |
| Rate limit | A control that limits repeated requests |

## A simple testing workflow

1. Confirm the API base address, version, roles, and accounts in scope.
2. Build an inventory of methods, endpoints, parameters, and objects.
3. Record normal responses for each approved role.
4. Test authentication and object/action authorization separately.
5. Check input types, size limits, errors, rate controls, and state changes.
6. Inspect JWT headers and claims without treating readable content as trusted.
7. Verify every result and remove tokens from saved evidence.

JWT content is encoded, not encrypted by default. A client can often read its
claims, but the server must verify the signature and validate issuer, audience,
expiry, and other required conditions before trusting them.

## Common mistakes

- Assuming an undocumented endpoint is out of scope.
- Testing only one user and missing object-level authorization.
- Treating a readable JWT as a data leak without considering intended design.
- Checking a token signature but ignoring expiry, issuer, or audience.
- Confusing a changed HTTP status with proven impact.
- Saving live bearer tokens in notes or screenshots.

## Defender view

Defenders should use deny-by-default authorization, validate tokens with
trusted algorithms and keys, enforce schemas and limits, rotate keys safely,
avoid sensitive token claims, log security-relevant decisions, and maintain an
accurate API inventory.

## Quiz

1. What four pieces help identify an API action precisely?
2. Why is one test account usually insufficient for authorization testing?
3. Does readable JWT content prove that the signature can be bypassed?
4. Name three token properties a server may need to validate.
5. Why must bearer tokens be redacted from evidence?

## Answer key

1. The base address or version, HTTP method, endpoint path, and relevant
   parameters or object.
2. Authorization is about differences between roles and object owners, which a
   single identity cannot demonstrate.
3. No. JWT payloads are commonly readable; trust depends on correct
   cryptographic and claim validation.
4. Examples include signature, approved algorithm, issuer, audience, expiry,
   and not-before time.
5. Anyone holding a valid bearer token may be able to act as its user until it
   expires or is revoked.

## Flashcards

**Q:** What does an API endpoint combine?  
**A:** A route with an HTTP method and its expected inputs.

**Q:** What is object-level authorization?  
**A:** A check that the current user may access the specific requested record.

**Q:** Is Base64-style encoding encryption?  
**A:** No. Encoded content may still be readable.

**Q:** What makes a JWT trustworthy?  
**A:** Correct signature and claim validation against trusted configuration.

**Q:** What is the safest evidence token?  
**A:** A redacted or expired lab token that cannot grant access.

## Safe practical exercise

Use an intentionally vulnerable local API or an assigned training lab. Create
two test users with different object ownership. Map five approved endpoints and
record:

- Method and path.
- Required role.
- Object owner.
- Expected response.
- Actual response for each user.
- Evidence with tokens replaced by REDACTED.

Do not test production APIs or undocumented public services. Delete created
objects and revoke lab tokens when finished.

## Completion checklist

- [ ] I can inventory endpoints, methods, objects, and roles.
- [ ] I understand what a JWT signature does and does not prove.
- [ ] I can separate authentication from object and action authorization.
- [ ] I completed a two-user authorization matrix in a lab.
