# GRC-Core-Registers

Praktický Asset a Risk Register pro telemetrická IoT/OT řešení. Tento repozitář slouží jako ukázka implementace principů Governance, Risk & Compliance (GRC) podle ISO 27001 a NIS2.

## Obsah repozitáře

### Registry (Excel)
* **Asset-Risk Register CORE.xlsx** – Komplexní matice obsahující:

Asset Register: Seznam aktiv, jejich vlastníci, síťové parametry a kritičnost (CIA).

Risk Register: Identifikace hrozeb, hodnocení dopadů a katalog nápravných opatření (mitigace).

### Bezpečnostní politiky (ISMS)
Tyto dokumenty definují procesní rámec pro ochranu aktiv uvedených v registru:
* [**Politika ISMS**](Policies/ISMS-Policy.md) – Hlavní nadřazený dokument řízení bezpečnosti.
* [**Řízení přístupu**](Policies/Access-Control.md) – Pravidla pro MFA, hesla a RBAC (řeší RISK-USR-01).
* [**Správa zranitelností**](Policies/Vulnerability-Management.md) – Cyklus skenování a SLA pro opravy (řeší RISK-VULN-01).
* [**Řešení incidentů**](Policies/Incident-Response.md) – Postup hlášení a eskalace (6 kroků).

## 🛠 Použití
1.  **Audit aktiv:** Identifikujte kritická aktiva v `Asset Register`.
2.  **Mitigace rizik:** Aplikujte opatření definovaná v `Policies/` na konkrétní rizika.
3.  **SLA Compliance:** Sledujte lhůty pro opravy zranitelností podle technické kritičnosti.
