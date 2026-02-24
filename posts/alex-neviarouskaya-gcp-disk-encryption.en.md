<!--
.. title: The GCP 'Read-Only' Risk: Bypassing Disk Encryption in the VibeOps Era
.. slug: alex-neviarouskaya-gcp-disk-encryption
.. date: 2026-02-11 12:00:00 UTC+01:00
.. tags: GCP, cloud security, disk encryption, VibeOps, Google Cloud Platform, cybersecurity
.. category: talks
.. link:
.. description: Alex Neviarouskaya explores security risks in GCP read-only permissions and disk encryption
.. type: text
-->

## Speaker Bio

**Alex Neviarouskaya** is an Engineering Manager at NALA, an expert in building secure systems and managing technical teams. She has shaped her career path at global technology companies, including Orca Security, where as Senior Software Engineering Manager she was responsible for key software development processes in cybersecurity.

A system security engineer by training, her work combines deep technical knowledge (including Go and Python technologies) with a modern approach to leadership. She specializes in scaling engineering teams and implementing processes that combine development efficiency with rigorous security standards. At the intersection of DevOps and management, she emphasizes automation and security as the foundations of a stable product.

## Talk Abstract

The rise of AI-assisted workflows has created a dangerous over-reliance on GCP (Google Cloud Platform) basic read-only roles and policies. In this session, we will deconstruct the "Read-Only" illusion by exploring a recently rewarded Google VRP vulnerability.

We will break down how the compute.disks.useReadOnly permission allowed attackers to exfiltrate Customer-Managed Encryption Key (CMEK) disks across projects. By exploiting the Compute Engine Service Agent during the cloning process, custom encryption was silently downgraded to Google-Managed keys (GME) in an attacker-controlled environment—completely bypassing KMS restrictions.

We will go over the architecture of this exploit, examine Google's solution, and reveal a newly discovered workaround that keeps this threat alive. Attendees will leave with a practical understanding of IAM auditing techniques and specific Organization Policy constraints to prevent data leakage outside of their environment.

More about the topic [on Alex`s blog](https://aneviaro.eu/posts/the-hidden-risk-of-gcp-viewer-role-cross-project-disk-replication/)

---

**When:** April 24, 2026, 13:00 - 13:45
**Language:** English
