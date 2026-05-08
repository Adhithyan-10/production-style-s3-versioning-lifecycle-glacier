# Sample Files Folder

This folder contains the sample object files used during the implementation and testing of the S3 Versioning and Lifecycle Management project.

These files were uploaded multiple times into the version-enabled S3 bucket to demonstrate:

* object versioning
* noncurrent object versions
* lifecycle policy automation
* Glacier archival transitions

---

# Included Files

## test.txt

This file was uploaded and modified multiple times inside the S3 bucket to create multiple object versions.

The file helped demonstrate how:

* S3 preserves previous object versions
* older versions become noncurrent
* lifecycle policies automatically detect noncurrent versions
* old versions transition into Glacier storage class

---

# Purpose of This Folder

This folder demonstrates:

* practical object versioning workflow
* real object lifecycle management
* version history tracking
* automated archival workflow

---

# Key Concepts Demonstrated

## S3 Versioning

Each time the file was modified and reuploaded:

* Amazon S3 created a new object version
* previous versions remained preserved
* object history became recoverable

---

## Noncurrent Object Versions

Older versions of the file became:

```text id="e9zjlwm"
Noncurrent Versions
```

These versions were later managed using lifecycle rules.

---

## Lifecycle Policy Automation

Lifecycle rules automatically identified noncurrent object versions and transitioned them into Glacier storage.

---

## Glacier Cost Optimization

Older object versions were archived into Glacier to reduce long-term storage costs while maintaining recoverability.

---

# Learning Outcome

This implementation helped provide practical understanding of:

* object version tracking
* backup-oriented storage design
* lifecycle automation
* archival storage management
* cloud cost optimization concepts
