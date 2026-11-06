# Respack NCR Management

A React + Vite starter for internal and external Non-Conformance Reports.

## Features in this first prototype
- Dashboard KPIs and recent NCR list
- Create NCR records for Internal, Supplier and Customer cases
- Search and filter the NCR register
- Update status, root cause, corrective action and action PIC
- Import and export Excel workbooks (.xlsx, .xls, .csv)
- Browser local storage for prototype persistence

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

## Important before production use
This first version stores records in the current browser only. It is a prototype, not yet a shared multi-user system. Before operational rollout, connect Supabase (database, authentication, role-based access and row-level security), define approval authority and audit history, and confirm the official NCR template and numbering rules. Do not enter confidential production/customer data until authentication and server-side access controls are configured.
