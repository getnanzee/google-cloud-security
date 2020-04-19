**Principle of Least Privilege**

- Use predefined roles over primitive roles.
- Grant roles at smalles scope necessary.
- When using Service Accounts, treat each app components as a separate trust boundary.
- A child resource cannot restrict access granted on its parent.
- Create a separate service account for each service.
- Restrict service account access.
- Restrict who can create and manage service accounts.
- Be cautious with owner roles.

**Service Accounts**

- Rotate user-managed service account keys (wait until creation, then delete).
- Donot delete service. accounts that are in use by running services.
- Name service keys to reflect use and permissions.
- **Don't check in service account keys into source code or leave in the Downloads directory.**

**Auditing**

- Use Cloud Audit logs to regularly audit IAM policy changes.
- Audit who can edit IAM policies on projects.
- Export audit logs to Cloud Storage for long-term retention.
- Restrict logs access with logging roles.

**Policy Management**

- To grant access to all projects in your Organization, use an organization-level policy.
- Grant roles to a Google group instead if Individual users when possible.
- When granting multiple riles to a particular job, create a Google group instead.