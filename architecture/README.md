# Architecture Folder

This folder contains the architecture diagram and workflow explanation for the production-style S3 versioning and lifecycle management project.

---

# Architecture Diagram

![Architecture Diagram](./archy.png)

---

# Architecture Overview

This architecture demonstrates a production-style cloud storage workflow using:
- Amazon S3
- S3 Versioning
- Lifecycle Policies
- Amazon S3 Glacier

The workflow shows how:
- files are uploaded into Amazon S3
- versioning preserves multiple object versions
- older object versions become noncurrent versions
- lifecycle policies automatically evaluate noncurrent versions
- archived versions transition into Amazon S3 Glacier
- storage costs are optimized while maintaining recoverability

This implementation represents a real-world storage lifecycle management architecture commonly used for:
- backup systems
- archival workflows
- disaster recovery
- compliance retention
- cost-optimized cloud storage

---

# Architecture Workflow

```text
User Uploads Object
        ↓
Amazon S3 Bucket
        ↓
S3 Versioning Enabled
        ↓
Multiple Object Versions Stored
        ↓
Lifecycle Policy Evaluates Noncurrent Versions
        ↓
Noncurrent Versions Identified
        ↓
Transition to Amazon S3 Glacier
        ↓
Storage Cost Optimization
