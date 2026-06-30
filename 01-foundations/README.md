# How IT Support Experience Maps to Cybersecurity

Service Desk is a great place to start a career in IT. I do tell people that the service desk role opens you up to practical knowledge of different fields in tech. Fields like network admin, system admin, and even security admin. Today, we shall be talking about how IT support maps to cybersecurity.

## Understanding the CIA Triad

The daily tasks I perform in my role as a service desk subject matter expert often align with the CIA triad, and I never really knew that until I decided to pivot into cybersecurity and study it. Let's talk about these tasks.

**Confidentiality**

Confidentiality has to do with keeping data away from unauthorized access. Users are not supposed to be able to view another user's details. Customers' data should remain classified from other users. Encryption protects your data from unauthorised access. It is wrong to reset the password for someone who is not the owner of the account. I usually ask people to use the self-service option. If they can't use that option, then I can talk about resetting it in Active Directory or the identity platform the organization uses.

**Integrity**

It means data should not be altered and must be accurate till it gets to its destination. Checksum confirms that the data has not been tampered with. For instance, a digital signature is important in corporate life. It helps verify the origin of a message and shows that it has not been tampered with. It does not automatically prove that every email is safe, but it does add an important layer of trust and integrity.

**Availability**

This means that information is available to those who need it, and they get it when it is needed. Backup servers are a good example of data availability. What if there is a failure? What if you lose your files? What if there is a ransomware attack? Backup servers are underrated. Some organizations treat backup servers as an afterthought. This is wrong. It is very important for the growth and health of the organization. When it comes to backup servers, we need to take them seriously and ensure that the backups are successful. We can run BCP tests from time to time to confirm the availability of backups.

Tools like Google Drive or Microsoft OneDrive are useful for file sync and quick recovery, keeping files accessible across devices, but they're not a substitute for proper enterprise backup. Real backup resilience comes from immutable, versioned snapshots and regular BCP testing, with clear retention policies behind them. File sync solves convenience; it doesn't on its own solve regulatory or ransomware-recovery requirements.

## CIA Triad In Your Daily IT Work

The daily tasks I perform in my role as a service desk subject matter expert incorporate the CIA triad and are low-key cybersecurity tasks, and I never knew that until I decided to pivot into cybersecurity and study it. Let's talk about some of these tasks.

One day, I attempted to log in to a server that my team wasn't responsible for managing. I knew the server's IP and had a privileged account, but I had no business accessing that system. I forgot it belonged to a different team. Access was denied; the control did its job. But within a few minutes, I noticed I'd lost network access. I could still do offline tasks, but I was cut off from the internet. The failed login attempt triggered that response.

This incident touches all three pillars of the CIA Triad. It highlights **confidentiality** because I attempted to cross an access boundary I wasn't authorized to, even unintentionally; that's exactly the kind of attempt confidentiality controls exist to stop. It highlights **integrity**, because had the login succeeded, there was a real risk of unintended configuration changes or tampering on a system I had no context for. And it touches **availability**, not because the server itself was affected, but because the security response cut off my own network access; a real, narrow, and self-contained availability impact, with no disruption to my team or the organization.

When I whitelist websites, I help reduce exposure by making sure that only approved sites are accessible. I also support integrity by lowering the chance that users will be exposed to harmful content, and I support availability by ensuring that the filtering does not disrupt other users' work.

As an IT support person, I reset passwords for employees who have forgotten their passwords. I support confidentiality by making sure that the request is from the actual owner of the account. Integrity tells me to make sure the credentials are valid and controlled. And availability tells me to ensure that the user gets access as soon as possible.

I grant the necessary access request as an IT service desk. It supports confidentiality by ensuring limited data exposure. It supports integrity by ensuring that users have appropriate rights. It highlights availability by allowing users to access the resources they need to work.

## Mapping IT Support Scenarios to the Threat–Vulnerability–Exploit Model

| Scenario | Threat | Vulnerability | Exploit |
|---|---|---|---|
| Unauthorized server login | Insider risk, or an authorized user acting outside their scope | Privileged account with broader access than the role required | The user attempts to log in to a server to which they have no authorization to manage |
| Whitelisting a website | A malicious or compromised external website | Users may visit unverified sites without a filtering control in place | An attacker uses a harmful site to steal data or deliver malware |
| Password reset | An external attacker impersonating the account owner | Poor identity verification during the reset process | The attacker uses the password reset procedure to take over the account |
| Access request | A user, or attacker using compromised credentials, seeking access beyond their need | Excessive permissions granted, or weak approval checks during provisioning | The user gains access to data or systems beyond what their role requires |
| Phishing report | An external attacker running a phishing campaign | The user may trust fake messages | The attacker tricks the user into clicking a link or sharing credentials |
| Account lockout | An attacker attempting a credential compromise | Weak login controls, such as no lockout threshold or no rate limiting | The attacker keeps trying passwords until lockout or compromise |
| Malware cleanup | An attacker distributing malware via download, attachment, or removable media | Unsafe downloads or unpatched systems | The malware executes, stealing data, encrypting files, or damaging systems |

## AAA Framework: Authentication, Authorization, and Accounting

AAA is an acronym that stands for Authentication, Authorization, and Accounting. Each of them is important when it comes to cybersecurity.

**Authentication**

Authentication has to do with verifying that a user is who they claim to be before they can access a platform or system. It has to do with signing in. Authentication can use one or more factors.

One factor is something you know, like a password. This is the most common way users sign in, especially on e-commerce platforms and many other online accounts.

Another factor is something you have, like an OTP or a hardware token. Here, the platform sends or generates a one-time code that can only be used within a specific period of time. Once the time elapses, a new one is needed. Many email and social media platforms use this as an extra layer after a username and password.

A third factor is something you are, like biometrics. This is where you use your fingerprint or face to confirm your identity.

**Authorization**

Authorization deals with the kind of access you have. For instance, you can only see your account details and balance on your banking app. You cannot see that of your friend or partner, except that they permit you or the system gives you that level of access. However, the teller in the bank can see your account details and make modifications because their role is different.

**Accounting**

Accounting has to do with logs. Accounting is about tracking user actions: when, where, why, and how they happened. It audits user actions and keeps records of what took place.

## Where This Experience Points Me Next

Looking at my experience in IT as a Service Desk Subject Matter Expert, I see myself pivoting into a SOC Analyst, Incident Response Analyst, or Security Analyst role. Here is what I am working on and what I bring to each of these roles.

**SOC Analyst (Level 1)**

I already have experience handling technical issues and tickets under SLA pressure, escalating tickets that need to be escalated, and executing tasks that need to be executed. I know what it feels like to be at the receiving end of a security incident in real time. I know what it is like to innocently trigger a security response.

I am working on reading alerts, tuning detection rules, and managing a live console instead of being a subject of one. I am studying this through a Wazuh SIEM lab and a Microsoft Sentinel detection lab, both part of my current TSA coursework.

**Incident Response Analyst**

I have experience handling tickets, communicating with affected users, documenting events, and working with other teams to close a ticket under pressure. I understand the importance of urgency and risk and how to prioritize incidents so as to get the best use of my time.

I am working on a formal incident-response methodology. I am studying structured investigation against a framework like the NIST incident response lifecycle, and I plan to build a documented incident report case study as a portfolio project. I will update this when I have one.

**Security Analyst**

I have hands-on experience working on Active Directory and M365 administration. I can provision and deprovision accounts, grant or deny access requests, and perform permission scoping. This is the operational aspect of Identity and Access Management (IAM), which is a core task for a security analyst.

I am working on vulnerability management and risk assessment. I'm building this through Module 3 (offensive security and vulnerability scanning) and Module 6 (cloud security and identity access management) in my current coursework at TSA.

## Conclusion

I didn't start my career studying the CIA triad, AAA framework, or how to break down a threat into different components. Rather, I learned how to keep accounts secure, systems patched, and users productive. It turns out that these tasks have another job title, different from IT Service Desk SME.

This document is simply me looking at my career in retrospect and naming what was actually going on. The patches, server-login incident, access request, and password change request. None of them made me think of cybersecurity at the time. I felt like I was just doing my job.

I am not approaching SOC Analyst, Incident Response, or Security Analyst roles as a novice; I am approaching them as a professional who has seen the operational side of the infrastructure. These roles are designed to protect, and I'm now getting the knowledge required to work with that title.

This piece is the first of my portfolio collections on cybersecurity. More will follow as I study more through labs and projects.
