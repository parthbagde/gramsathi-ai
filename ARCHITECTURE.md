# Technical Design — GramSathi AI

## Prototype architecture
```text
User (mobile / desktop browser)
             |
             v
    index.html (UI + CSS)
             |
             v
  Vanilla JavaScript logic
   |          |           |
   v          v           v
Sample data  Filters   Rule-based FAQ
(in memory)  & modal   response handler
```

## Data flow
1. User searches or selects category/audience.
2. The browser filters illustrative sample entries.
3. The eligibility guide uses role and age-group selections to suggest discovery categories.
4. The FAQ assistant maps common keywords to safe, generic guidance.
5. No personal information is submitted to a server or stored persistently.

## Production architecture (proposed)
- Frontend: accessible responsive web app.
- Backend API: read-only scheme search and content management.
- Data store: verified scheme records with source URL, last-checked date, region, eligibility, benefits, and required documents.
- AI assistant: retrieval-grounded answers using approved official sources; always cite the source and show last-updated date.
- Admin workflow: human review before publishing updates.
- Privacy: collect minimum data, avoid storing identity documents, protect logs, and provide clear consent and deletion controls.

## Risks and mitigations
- Outdated information: official source links, last-verified timestamps, scheduled review.
- Incorrect eligibility: label suggestions as indicative; link to official eligibility criteria.
- Language errors: human review of translations.
- Privacy risks: no document upload in prototype; data minimisation in production.
