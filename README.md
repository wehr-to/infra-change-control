# 🔄 infra-change-control

This repository contains a **Change Management Toolkit** designed to simulate how modern infrastructure teams safely introduce, validate, and track infrastructure changes across environments.

It includes:

- Pre-flight validation scripts
- Rollback plans
- Annotated configuration changes
- Sample change advisory records (CARs)
- Change logging and audit frameworks

## 🎯 Why This Repo Exists

Most outages aren't due to malicious actors — they're due to untested or undocumented changes.

This repo helps you:

- Practice **safe infrastructure modification**
- Create **audit trails and rollback workflows**
- Understand **change windows**, peer review, and staging
- Learn the language and processes of real-world operations

## 🧱 What's Included

| Folder                      | Description |
|-----------------------------|-------------|
| `pre-flight-checks/`         | Scripts to validate syntax, dependencies, and system state before a change |
| `rollback-plans/`            | Documented plans for reversing critical changes (infra, DNS, IAM, etc.) |
| `annotated-configs/`         | Before-and-after samples of config files with annotated diffs |
| `change-logs/`               | Example audit logs, changelogs, and review metadata |
| `car-templates/`             | Change Advisory Record (CAR) templates and mock submissions |
| `ci-pipeline-checks/`        | GitHub Actions and pre-commit examples for enforcing change safety |
| `docs/`                      | Change control policies, escalation paths, and review checklists |

## 🧪 Simulated Change Scenarios

| Scenario                          | What You’ll Learn |
|-----------------------------------|--------------------|
| `dns-cutover-rollout/`           | How to stage, validate, and back out a nameserver or load balancer change |
| `firewall-rule-update/`          | Validating rules before production apply + rollback plan |
| `terraform-ec2-resize/`          | Change justification, drift checks, and recovery if instance fails boot |
| `ansible-ssh-hardening/`         | Pre-change SSH validation + user lockout prevention plan |
| `iam-policy-tighten/`            | Detecting blast radius of an IAM change before merge |
| `s3-bucket-acl-mod/`             | S3 public access removal with pre-flight access check |

## 👥 Who Should Use This
- Infra engineers learning real-world change workflows
- Blue teamers simulating secure rollback and audit trails
- Cloud and DevOps engineers applying changes at scale


