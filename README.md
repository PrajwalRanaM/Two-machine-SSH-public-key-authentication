Two-Machine SSH Remote Access and Session Logging Lab

Overview

This hands-on cybersecurity lab explores Secure Shell (SSH) remote access between two separate machines. It demonstrates how a Linux client connects to a remote Linux server and how the server records session activity.

The lab also explores the security role of SSH authentication, server access controls, and authentication-log analysis.

Lab Environment

- Client: Kali Linux running in a virtual machine on a Windows laptop.
- Server: Linux Mint running on a separate physical laptop.
- Protocol: SSH.
- Server-side monitoring: SSH service logs on Linux Mint.

Objectives

- Establish an SSH connection between two separate machines.
- Access a remote Linux terminal.
- Observe SSH session events in the server logs.
- Understand the purpose of public and private SSH keys.
- Identify how SSH logs can support security monitoring and incident investigation.

Work Completed

1. Established a remote SSH connection from Kali Linux to the Linux Mint server.
2. Accessed the remote server's terminal.
3. Closed the SSH session.
4. Checked the server logs and observed session-opened and session-closed events.

Observed Results

The Kali client successfully accessed the Linux Mint terminal. The server recorded the opening and closing of the SSH session.

These observations demonstrate remote access and server-side session logging.

Verification note: Session-opened and session-closed events alone do not establish which authentication method was used. Public-key authentication requires separate confirmation through client authentication output and/or server log entries showing successful public-key authentication.

Security Concepts Learned

1. SSH remote administration

SSH allows authorised users to administer remote Linux systems through an encrypted connection without needing physical access to the server.

2. Public-key authentication

SSH public-key authentication uses a private key held by the client and a corresponding public key authorised on the server. The private key must be protected and should never be published in a repository.

3. Authentication logging

Server logs can help analysts investigate successful and failed authentication attempts, account activity, and session events.

3. SSH key persistence

An unauthorised public key added to a user's 'authorized_keys' file can provide another means of access. Investigating unexpected key changes is therefore an important security task.

Evidence

Screenshots are added.

Conclusion

This lab provided practical experience with remote SSH access between separate Linux machines and demonstrated how server-side logs record session activity. It also established a foundation for understanding SSH authentication and the role of logging in cybersecurity investigations.
