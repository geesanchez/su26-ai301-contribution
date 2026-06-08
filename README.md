# Contribution 1: orgs: domain restrictions displays <br>

**Contribution Number:** 1
**Student:** Gabriel Sanchez
**Issue:** https://github.com/MISP/MISP/issues/4297
**Status:** Phase I Complete

---

## Why I Chose This Issue

I chose this issue because it's a well-scoped UI rendering bug with a clear expected outcome — 
making it ideal for a first open source contribution. The fix lives in the view/template layer, 
which means I can trace and understand the problem without needing deep expertise in MISP's 
security intelligence domain.

As a full-stack engineer with experience in PHP, JavaScript, and templating systems, I'm 
confident I can navigate a CakePHP codebase and implement a clean fix. I also want to practice 
the full open source contribution workflow — forking, reproducing, fixing, and submitting a PR 
to a real maintainer — which is exactly what this issue offers.

---

## Understanding the Issue

### Problem Description

When an organization has multiple domain restrictions configured, the UI displays literal `<br>` 
HTML tags as plain text instead of rendering them as line breaks.

### Expected Behavior

Multiple domain restrictions should display as separate lines in the UI.

### Current Behavior

The domain restrictions field renders `<br>` as a visible string rather than an HTML line break.

### Affected Components

The organization view templates in the MISP/MISP repository — likely a `.ctp` file in 
`app/View/Organisations/`.
