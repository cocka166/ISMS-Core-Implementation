# ISMS-Core-Implementation

**POZNÁMKA:** Tento repozitář obsahuje **anonymizovanou a modelovou dokumentaci**. Veškerá data, názvy aktiv a scénáře rizik jsou fiktivní a slouží výhradně pro demonstrační účely a jako šablona pro implementaci GRC procesů.

Komplexní rámec pro řízení informační bezpečnosti (ISMS) v prostředí telemetrických IoT/OT řešení.

Tento repozitář představuje praktickou implementaci principů Governance, Risk & Compliance (GRC) navrženou specificky pro monitoring vozového parku a kritickou infrastrukturu. Projekt je plně v souladu s požadavky norem ISO 27001:2022 a evropské směrnice NIS2.

**Hlavní přínosy:**
Integrované řízení: Propojení evidence aktiv s analýzou rizik a konkrétními bezpečnostními politikami.

**IoT/OT specifika:** Řešení rizik spojených s telemetrickými jednotkami, integritou firmwaru a privátní konektivitou.

**Audit-Ready:** Dokumentace je strukturována tak, aby sloužila jako přímý podklad pro certifikační audity nebo kontrolu dozorových orgánů.

## Obsah repozitáře

### Registry (Excel)
* **Asset-Risk Register CORE.xlsx** – Komplexní matice obsahující:

Asset Register: Seznam aktiv, jejich vlastníci, síťové parametry a kritičnost (CIA).

Risk Register: Identifikace hrozeb, hodnocení dopadů a katalog nápravných opatření (mitigace).

### Bezpečnostní politiky (ISMS)
Tyto dokumenty definují procesní rámec pro ochranu aktiv uvedených v registru:
* [**Politika ISMS**](Policies/ISMS-Policy.pdf) – Hlavní nadřazený dokument řízení bezpečnosti.
* [**Řízení přístupu**](Policies/Access-Control.pdf) – Pravidla pro MFA, hesla a RBAC (řeší RISK-USR-01).
* [**Správa zranitelností**](Policies/Vulnerability-Management.pdf) – Cyklus skenování a SLA pro opravy (řeší RISK-VULN-01).
* [**Řešení incidentů**](Policies/Incident-Response.pdf) – Postup hlášení a eskalace (6 kroků).

## Použití
1.  **Audit aktiv:** Identifikujte kritická aktiva v `Asset Register`.
2.  **Mitigace rizik:** Aplikujte opatření definovaná v `Policies/` na konkrétní rizika.
3.  **SLA Compliance:** Sledujte lhůty pro opravy zranitelností podle technické kritičnosti.
