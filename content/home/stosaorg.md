---
title: "STOSA Organization"
date: 2020-06-20T20:37:52-07:00
weight: 40
---
Figure 3 shows a typical organization hierarchy for a STOSA-based organization. Essentially, all development teams that are service-owning teams are peers, organizationally. They are all supported uniformly by a series of supporting teams, including operations, tooling, databases, and other similar teams. All of these may or may not also sit on top of other core teams that have universal responsibility for the organization, but not for individual services. This can include things like an architectural guidance team or a program management team.

<div style="padding-bottom: 20px;">
    <img src="/images/stosa-teams.png">
    <div style="font-style:italic;"><span style="font-weight:bold;">Figure 3</span>. STOSA-based organization heiarchy.</div>
</div>

Service-owning teams in a STOSA organization are the teams that are ultimately responsible for all aspects of the services they own. They might depend on the core and support teams, but it is the service-owning team that is ultimately responsible for ensuring that all issues are dealt with and the service is operating properly.

For example, let’s assume that a service fails because a deployment went bad due to a failure in the core deployment tool. The service failure is the responsibility of the service-owning team. They may have issues or concerns with the tooling team that they need to deal with, but ultimately the service-owning team is the one responsible for the failure. They cannot simply say “it was the tooling team’s fault.” Ultimately, even if that were true, it was the service that failed, and hence the service-owning team that is responsible.

With strong ownership of results also comes strong ownership of decision making affecting your service. Typically, a service-owning team is given a set of requirements they need to implement, but the details of how those requirements are implemented are their responsibility. The team might have system-wide compliance requirements they need to conform to (such as architecture guidelines or rules, tooling that must be used, language and hardware selection restrictions, or industry specific regulatory requirements), but these ultimately are part of the service requirements given to them.

Beyond these requirements, all design details and decisions are the responsibility of the owning team.

Ultimately, the owning team is making a commitment to achieve an expected set of results, and maintain an appropriate set of SLAs.