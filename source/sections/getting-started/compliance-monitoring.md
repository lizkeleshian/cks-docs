### Compliance Monitoring

#### Intrusion Detection

Datica's CKS includes a [Wazuh](https://wazuh.com/) deployment for intrusion detection. It is configured to alert Datica's security team, which triggers an internal process for evaluating and addressing events, including customer escalation if necessary.

#### Vulnerability Scanning
Datica performs external vulnerability scanning for all production CKS clusters. Datica’s security team keeps track of alerts generated by Nessus and has protocols for evaluating and addressing events that occur, including a customer escalation protocol for application-specific events.

#### Volume Snapshots
Datica creates daily snapshots of all volumes attached to instances in your CKS cluster. These snapshots are kept for a minimum of two days, and are replicated across regions for redundancy. Snapshots older than two days are pruned automatically. These snapshots are intended for maintaining compliance by providing the ability to fully restore a volume from a snapshot. We encourage customers to be aware of their specific application needs in terms of data retention which may require other methods, frequencies, and retention policies for data recovery.