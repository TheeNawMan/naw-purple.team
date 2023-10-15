# Active Directory (AD)

## Introduction

**Active Directory (AD)** is a directory service developed by Microsoft for Windows domain networks. It's primarily used for centralized domain management, and it provides authentication and authorization functions, among other services.

## Key Components

1. **Domains**: AD is organized into one or more domains. A domain is a collection of objects (like users, computers, and groups) that share the same AD database.
2. **Domain Controllers (DC)**: These are the servers that run AD. They manage user login processes, directory queries, and changes to the directory.
3. **Forest**: A collection of one or more AD domains that share a common schema, configuration, and global catalog. Domains within a forest trust each other.
4. **Organizational Units (OU)**: Subdivisions within a domain, used to group related objects for administrative purposes.
5. **Global Catalog**: A distributed data repository that contains information about every object in a domain. It helps in finding objects in a large AD setup.

## How AD Works

1. **Authentication**: When a user logs in, AD checks the entered credentials against its database to authenticate the user.
2. **Authorization**: After authentication, AD determines the resources a user can access and the operations they can perform based on permissions.
3. **Replication**: Changes to the directory (like adding users or changing passwords) are replicated across all Domain Controllers to ensure consistency.
4. **Policies**: Group Policy Objects (GPO) allow administrators to implement specific configurations for users and computers within a domain (like setting password policies or configuring desktop settings).

## Features of AD

- **Single Sign-On (SSO)**: Users only need to authenticate once to access multiple services and applications.
- **Hierarchical Organizational Structure**: Allows for organized management of domain objects.
- **Scalability**: AD can manage millions of objects.
- **Extensibility**: The AD schema can be extended to add new types of objects or new properties to existing objects.
- **Security**: Provides features like LDAP over SSL, Kerberos-based authentication, and SID (Security Identifier) for uniquely identifying users.

## Common AD Services

- **AD Domain Services (AD DS)**: The core service that stores directory information and handles user and computer authentication.
- **AD Lightweight Directory Services (AD LDS)**: A lighter version of AD DS that provides directory storage and LDAP directory services.
- **AD Federation Services (AD FS)**: Provides single sign-on across organizational boundaries.
- **AD Certificate Services**: Issues and manages public key certificates.
- **AD Rights Management Services**: Protects digital information from unauthorized use.

## Conclusion

Active Directory is a cornerstone of many corporate networks around the world. It simplifies user and resource management while providing robust security features, making it an indispensable tool for many IT administrators.

