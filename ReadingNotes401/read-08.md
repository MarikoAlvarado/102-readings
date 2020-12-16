# Access Control (ACL)

**1. When is Basic Authorization used vs. Bearer Authorization?**

Basic authorization is a simple name and password input while bearer authorization requires the user to have an encrypted token.

**2. What does the JSON Web Token package do?**

 It's a library with authentication tools that add additional conditions like algorithms and expirations on a token.

**3. What considerations should we make when creating and storing a SECRET?**

The secret should be encrypted and kept in a dotenv file/away from public access.


## Terms

**encryption** - Encoding information from plain text into complex and random string that is difficult to decode.

**token** - Secure way of passing the authorization code for a user to have access to API endpoint.

**bearer** - Whoever holds a valid token

**secret** - The digital signature for a JWT [source](https://jwt.io/introduction/)

**JSON Web Token** - A way of securely storing and delivering sensitive information to and from multiple sources.

[RBAC](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)

RBAC stands for *role-based access control* and it's how system access is granted to different users based on their roles within an organization. Roles are assigned based on job duties and access need. Implementation of RBAC can be done in five steps. Inventory of systems to figure out who needs control access to what systems, creating and assigning roles, auditing and never making "one-off" changes even under special conditions.


Additional resource
- [RBAC Wiki](https://en.wikipedia.org/wiki/Role-based_access_control)