---
title: "What Does it Mean to Own a Service?"
date: 2020-06-20T20:37:52-07:00
weight: 30
---
In a STOSA organization, the team that owns a service is ultimately 100% responsible for all aspects of that service. That team might depend on other teams for assistance (such as an operations team for hardware), but ultimately the owning team is responsible for the service.

This includes the following, specifically:

### API design

The design, implementation, testing, and version management of all APIs, internal and external, that the service exposes.

### Service development

The design, implementation, and testing of the service’s business logic and business responsibilities.

### Data

The management of all data the service owns and maintains, its representation and schema, access patterns, and lifecycle.

### Deployments

The process of determining when and if a service update is required, and the deployment of new software to the service, including verification and rollback of all service nodes and the availability of the service during the deployment.

### Deployment windows

When it is safe and when it is not safe to deploy. This includes enforcing company/product- wide blackouts as well as service-specific windows.

### Production Infrastructure changes

All production infrastructure changes needed by the service (such as load balancer settings and system tuning).

### Environments

Managing the production environment, along with all development, staging, and pre- production deployment environments for the service.

### Service SLAs

Negotating, setting, and monitoring SLAs, along with the responsibility of keeping the service operating within those SLAs.

### Monitoring

Ensuring that monitoring is set up and managed for all appropriate aspects of the service, including monitoring service SLAs. It also is responsible for reviewing the monitoring on a regular and consistent basis.

### Incident response

Ensuring that pager notifications are generated when the system begins to function out of specification. Providing oncall rotation and pager management, as necessary, to make sure someone from the team is available to handle incidents. Handling incidents within prescribed SLA boundaries for incident responsiveness.

### Reporting

Internal reporting to other teams (consumers and dependencies) as well as management reporting on the operational health of the service.

Often, some of the above aspects are not handled directly by the owning team, but are the responsibility of a shared infrastructure, tools or operations team. Even in these cases where aspects are handled by other core teams, it is ultimately the service owner’s responsibility to make sure the activities are handled to the level required for them to meet their SLAs and customer expectations.

The following items often are handled by shared teams on behalf of the owning team:

### Servers/hardware

All hardware and infrastructure needed to run the hardware for production and all supporting environments. This is often provided by an operations team, or may be provided by a cloud provider, or both.

### Tooling

Various tooling required by the owning team is often centrally owned and managed. This can include deployment tools, compiling and code management tools, monitoring tools, oncall and incident response tools, and reporting tools.

### Databases

The hardware and database applications used to store the data used by the service is often managed by a central team. However, the data itself, the data schema, and the use of the data, is always managed by the owning team.