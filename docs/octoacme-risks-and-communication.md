# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates

### Weekly Status Update Template
```
Project: [Project Name]
Period: [Date Range]
Status: [On Track / At Risk / Blocked]

Progress This Week:
- [Key accomplishment 1]
- [Key accomplishment 2]
- [Key accomplishment 3]

Next Steps:
- [Planned activity 1]
- [Planned activity 2]
- [Planned activity 3]

Risks & Blockers:
- [Risk ID / Description] - Impact: [H/M/L] - Owner: [Name] - Status: [Active/Mitigated]
- [Blocker description] - Action needed: [What's needed to unblock]

Decisions Needed:
- [Decision 1] - By: [Date] - Stakeholders: [Who needs to decide]
- [Decision 2] - By: [Date] - Stakeholders: [Who needs to decide]

Metrics:
- Sprint velocity: [X points/items]
- Test coverage: [X%]
- Deployment frequency: [X per week]
- Incident count: [X]
```

### Risk Communication Template
```
Risk ID: [Unique identifier]
Date Identified: [Date]
Identified By: [Role/Name]

Description: [Clear description of the risk]

Impact: [High / Medium / Low]
- If High: [Describe potential project/business impact]
- Affected areas: [Scope, timeline, quality, budget, team]

Likelihood: [High / Medium / Low]
- Rationale: [Why is this likely or unlikely to occur]

Owner: [Name and role of risk owner]

Mitigation Plan:
- Action 1: [Description] - Owner: [Name] - Due: [Date]
- Action 2: [Description] - Owner: [Name] - Due: [Date]
- Contingency: [What if mitigation fails]

Status: [Identified / In Progress / Mitigated / Closed]
Last Updated: [Date]
```

### Incident Communication Template
```
Incident: [Brief title]
Severity: [Critical / High / Medium / Low]
Start Time: [Timestamp]
Detected By: [Role/Name]

Current Status: [Investigating / Identified / Mitigating / Resolved]

Triage Summary:
- Impact: [What systems/users are affected]
- Scope: [How widespread is the issue]
- Root cause (if known): [Brief description]

Actions Being Taken:
- [Action 1] - Owner: [Name]
- [Action 2] - Owner: [Name]
- [Action 3] - Owner: [Name]

Expected Timeline:
- Resolution ETA: [Timestamp or "Unknown - investigating"]
- Next update: [Timestamp]

Communication Plan:
- Stakeholders notified: [Yes/No - List]
- Customer communication: [Planned/Sent - Channel]
- Status page updated: [Yes/No]

Post-Incident Activities:
- Blameless retrospective scheduled: [Date/Time]
- Incident report owner: [Name]
- Follow-up actions tracking: [Link to tracking system]
```

### Cross-Team Dependency Communication Template
```
Dependency ID: [Unique identifier]
Requesting Team: [Team name]
Providing Team: [Team name]
Date Raised: [Date]

Description: [What is needed]

Impact on Project:
- If delivered on time: [Positive outcome]
- If delayed: [Risk and impact]

Timeline:
- Needed by: [Date]
- Provider commitment: [Date or "TBD"]
- Buffer/contingency: [X days]

Owner (Requesting Team): [Name]
Owner (Providing Team): [Name]

Status: [Requested / Committed / In Progress / Delivered / Blocked]

Communication Cadence: [How often teams will sync on this dependency]

Escalation Path (if blocked): [PM → Team Lead → Director]
```

### Stakeholder Escalation Template
```
Escalation Date: [Date]
Escalated By: [Name and Role]
Escalation Level: [Team → PM → Product Lead → Sponsor]

Issue Summary: [Brief description of what needs escalation]

Context:
- How long has this been an issue: [Duration]
- Previous attempts to resolve: [What has been tried]
- Impact if not resolved: [Business/project impact]

Decision/Action Needed:
- [Specific ask - be clear and actionable]
- By when: [Date]
- Consequences of delay: [What happens if no decision]

Recommended Approach: [Your suggested solution if any]

Supporting Information: [Links to docs, data, previous discussions]
```

### Release Communication Template
```
Release: [Version/Name]
Date: [Scheduled release date]
Status: [Planned / Ready / Deployed / Rolled Back]

What's Included:
- Feature 1: [Brief description and value]
- Feature 2: [Brief description and value]
- Bug fixes: [Count or notable fixes]

Testing Summary:
- Test coverage: [X%]
- Critical bugs: [Count and status]
- Performance impact: [Improvement or regression]

Deployment Plan:
- Deployment window: [Start - End time]
- Deployment method: [Blue-green, canary, rolling, etc.]
- Rollback plan: [Brief description]
- Monitoring plan: [Key metrics to watch]

Stakeholder Actions Required:
- [Action 1] - Owner: [Team/Person] - By: [Date]
- [Action 2] - Owner: [Team/Person] - By: [Date]

Communication:
- Internal announcement: [Planned/Sent]
- Customer notification: [Planned/Sent - if user-facing]
- Documentation updated: [Yes/No - Links]

Post-Release:
- Success criteria: [How we'll measure success]
- Monitoring period: [Duration of enhanced monitoring]
- Retrospective: [Scheduled date]
```

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call
