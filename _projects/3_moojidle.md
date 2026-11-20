---
layout: page
title: Moojidle — Course Management System
description: 2025 – 2026 · A course management system built by a 9-person Agile team, later migrated to a high-availability Kubernetes (k3s) cluster on AWS.
importance: 3
category: course projects
---

**Courses:** Introduction to Software Engineering; Distributed Systems · 2025 – 2026<br>
**Role:** Co-Lead (one of three); Course-Feature Subteam Lead; Frontend Reviewer<br>
**Tools:** Express.js, React.js, MongoDB, Nginx, Docker, GitLab CI/CD, GitHub Actions, AWS, Kubernetes (k3s), Terraform, k6<br>
**Code:** [GitLab](https://gitlab.com/jingxiang0405/moojidle) · [GitHub (k8s)](https://github.com/Jason9339/moojidle-k8s)

### Problem

Moojidle is a course management system designed to make common course operations faster than in Moodle.
In a second phase, the goal was to move it from a single server to infrastructure that is highly available and quick to redeploy.

### Initial development (2025)

- Co-led a 9-person Agile team, coordinating Jira sprint planning and task breakdown across subteams.
- Led the course-feature subteam building course pages and features; reviewed frontend code for all subteams.
- Deployed on AWS behind an Nginx reverse proxy with MongoDB Atlas, gated by GitLab CI/CD build and test checks.
- Reduced task completion time for common course operations by 40–70% compared with Moodle.

### Infrastructure upgrade (2026, 6-person team)

- Migrated a single-EC2 monolith to a 5-node high-availability k3s cluster on AWS, storing files in MongoDB GridFS.
- Codified infrastructure with Terraform and Bash, cutting full deployment from 0.5–1 hour to about 10 minutes.
- Configured horizontal pod autoscaling, rolling updates, and CloudWatch/SNS alerting; validated resilience with k6 stress tests, ranking first in the final class presentation.
