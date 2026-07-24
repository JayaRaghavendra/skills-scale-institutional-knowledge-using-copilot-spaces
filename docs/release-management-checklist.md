# Release Management Checklist

Purpose: Operational checklist for the Release Manager to standardize safe, repeatable deployments.

Pre-release
- [ ] Confirm all PRs merged for the release milestone
- [ ] CI: All tests passing (unit, integration) and security scans completed
- [ ] Feature flags: verify toggles for incremental rollout
- [ ] Rollback plan documented and validated
- [ ] Stakeholders informed of release window

Staging
- [ ] Deploy to staging and run smoke tests
- [ ] Verify key metrics and dashboards are reporting
- [ ] Run end-to-end smoke tests for critical flows
- [ ] Performance/quick load checks (if applicable)

Production
- [ ] Run deployment during agreed window
- [ ] Monitor CI/CD deployment logs and automated checks
- [ ] Execute post-deploy smoke tests
- [ ] Monitor error rates, latency, and key SLIs for 30–60 minutes

Post-release
- [ ] Publish release notes and known issues
- [ ] Confirm monitoring/alerts are stable
- [ ] Capture any follow-up actions (tickets) for improvements or rollbacks

Incident / Rollback
- [ ] Trigger incident response if critical degradation detected
- [ ] Rollback according to documented plan (if needed)
- [ ] Triage root cause and create follow-up action items

Owner: Release Manager
