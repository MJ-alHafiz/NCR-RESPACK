# Respack NCR Management

A React + Vite NCR register prototype using one standard form for all departments and all internal/external non-conformances.

## NCR categories
- Internal: Production, QA, Warehouse, Maintenance, Engineering, Planning, Logistics, HR, Administration and any other department.
- Supplier: raw material, packaging, service, delivery or supplier process issues.
- Customer: complaints, returns, rejected goods and customer-reported issues.

## Standard NCR form sections
A. NCR identification, reporting party, department, source and related references.
B. Product/material, code, batch/lot, machine, quantity affected/inspected and traceability dates.
C. Non-conformance description, requirement/specification reference, evidence, detection method, severity and impact.
D. Immediate containment, material disposition, approvals and risk assessment.
E. Investigation, root-cause method, confirmed root cause and contributing factors.
F. Correction, corrective action, preventive/recurrence prevention, owner, department, due date and resources.
G. Completion, verification criteria/results, verifier and effectiveness review.
H. Status, approvals, closure date, closure remarks and attachment references.

Fields not relevant to a particular NCR may be left blank. The same form and workflow applies to all categories.

## Prototype features
- Dashboard and NCR register
- Automatic NCR number generation
- Search and category filters
- Edit/update NCR investigation and action details
- Excel import and full-field export

## Run locally
```bash
npm install
npm run dev
```

## Build
```bash
npm run build
npm run preview
```

## Important production-readiness notes
This first version stores records in the current browser only. It is not yet a shared multi-user company system. Before operational rollout, connect a secure shared database and authentication (for example Supabase), configure role-based access and row-level security, implement audit history and approval controls, and confirm Respack's document-control rules. Attachment fields currently record file references only; file upload/storage is not implemented. This is a general quality-management template inspired by common ISO 9001 nonconformity/corrective-action practices; it is not a certification or compliance guarantee.
