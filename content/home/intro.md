---
title: "Single Team Oriented Service Architecture"
date: 2020-06-20T20:37:52-07:00
weight: 10
---
What is Single Team Owned Service Architecture (STOSA)? STOSA is an important guiding principle for large organizations that have many development teams that own and manage services comprising one or more applications.

What does it mean to have a STOSA application and organization? To be STOSA, you must meet the following criteria:

* Have an application that is constructed using a service-based architecture or a microservice-based architecture.
* Have multiple development teams that are responsible for building and maintaining the application.
* Each and every service in your application must be assigned to a development team, who owns that service. Who owns which service should be well documented and readily available to everyone in the organization.
* No service should be assigned to more than one development team. Individual development teams may own more than one service.
* Teams are responsible for all aspects of managing the service, from service architecture and design, through development, testing, deployment, monitoring, and incident resolution.
* Services have strong boundaries between them, including well-documented APIs.
* The service owns its own data. Data is part of the service. If a service needs to access data stored in a different service, it must use one of the well-documented APIs to access that data.
* Services maintain internal service-level agreements (SLAs) between them that are monitored and violations reported to the owning team.
A STOSA-based application is an application for which all services follow the preceding rules. A STOSA-based organization is one in which all service teams follow the preceding rules and all applications are STOSA applications.

Typically, in a STOSA-based organization, each team should be of reasonable size (typically between three and eight engineers). If a team is too small, it cannot manage a service effectively. If it’s too large, it becomes cumbersome to manage the team.

<div style="padding-bottom: 20px;">
    <img src="/images/stosaorg.png">
    <div style="font-style:italic;"><span style="font-weight:bold;">Figure 1</span>. A typical STOSA-based organization managing a STOSA application.</div>
</div>

In Figure 1, the boxes labeled A though L represent each individual service within the application. The ovals represent development teams that own the enclosed services.

This application contains 12 services managed by five teams. You’ll notice that each service is managed by a single team, but several teams manage more than one service. Every service has an owner, and no service has more than one owner.

Clear ownership for every aspect of the application exists. For any part of the application, you can clearly determine who is responsible and who to contact for questions, issues, or changes.

Figure 2 shows an example application and organization that is not a STOSA organization.

<div style="padding-bottom: 20px;">
    <img src="/images/nonstosaorg.png">
    <div style="font-style:italic;"><span style="font-weight:bold;">Figure 2</span>. Non-STOSA-based organization.</div>
</div>

You’ll notice a couple things. First, Service I does not have any owner. Yet, Services C and D are owned and maintained by more than one team.

There is no clear ownership. If you need something done in service C or D, it’s not clear who is responsible. If one of those services has a problem, who responds? What happens if you need something done to service I? Who do you contact? This lack of clear ownership and responsibility makes managing a complex application even more complicated.

