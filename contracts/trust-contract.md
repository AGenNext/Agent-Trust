# Trust Contract

## Governing Principle

```text
No trust without evidence.
No evidence without provenance.
No provenance without traceability.
```

## Trust Dimensions

Every artifact, decision, and workflow should be assessable across:

1. Provenance
2. Evidence
3. Traceability
4. Policy Compliance
5. Security Posture
6. Evaluation Results
7. Human Approval
8. Freshness
9. Reproducibility
10. Explainability

## Required Trust Metadata

```yaml
trust_id: string
subject_type: objective | task | handoff | artifact | model_selection | evaluation | approval
subject_id: string
trust_score: number
trust_status: trusted | conditional | untrusted
provenance_refs: []
evidence_refs: []
policy_refs: []
evaluation_refs: []
audit_refs: []
reviewed_by: []
reviewed_at: datetime | null
risks: []
assumptions: []
limitations: []
```

## Trust Rules

An output should not be considered fully trusted unless:

- provenance is available
- evidence is linked
- policy checks pass
- evaluation checks pass
- material risks are disclosed
- freshness is acceptable
- required approvals are complete

## Final Rule

If a claim cannot be traced, it should not be trusted.
