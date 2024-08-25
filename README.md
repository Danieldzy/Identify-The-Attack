<h1>Vulnerability Scan and Risk Assessment Report</h1>

<h2>Considerations</h2>

Conducting a vulnerability scan can consume significant resources on both your host and target systems, potentially causing system downtime if not managed properly. As a Cybersecurity professional, it is crucial to understand your environment thoroughly before initiating such scans. Ensure clear communication with your manager and schedule scans for off-peak hours to reduce production impact. Begin by testing in a staging environment, and if you plan to automate scans, first conduct manual tests in a smaller production environment to verify that everything runs smoothly. It is crucial that all stakeholders are informed about the scan and understand the potential impact.

<h2>Summary</h2>
In this project, I used both Nessus and OpenVAS to scan the same target with similar settings (I scanned fewer ports with Nessus compared to OpenVAS). However, Nessus identified more vulnerabilities overall. For example, the following two critical vulnerabilities were identified by Nessus but did not appear in the OpenVAS report:<br/>
<br/>- NFS Exported Share Information Disclosure: At least one of the NFS shares exported by the remote server could be mounted by the scanning host. An attacker may be able to leverage this to read (and possibly write) files on remote host.<br/>
- Bind Shell Backdoor Detection: A shell(CLI) is listening on the remote port without any authentication being required. An attacker may use it by connecting to the remote port and sending commands directly.<br/>

<br/> I will develop a Risk Assessment Report for the client based on the findings from the Nessus scan, with a focus on delivering clear and professional communication. The Risk Assessment Report can be found in this repository.<br/> 
