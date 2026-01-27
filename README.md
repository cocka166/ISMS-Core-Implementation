# ISMS-Core-Implementation

> [!IMPORTANT]
> **POZNÁMKA:** Tento repozitář obsahuje **anonymizovanou a modelovou dokumentaci**. Veškerá data, názvy aktiv a scénáře rizik jsou fiktivní a slouží výhradně pro demonstrační účely jako šablona pro implementaci GRC procesů.

Komplexní rámec pro řízení informační bezpečnosti (ISMS) v prostředí telemetrických **IoT/OT řešení**. Tento projekt představuje praktickou implementaci principů **Governance, Risk & Compliance (GRC)** navrženou specificky pro monitoring vozového parku a kritickou infrastrukturu. 

Projekt je plně v souladu s požadavky norem **ISO 27001:2022** a evropské směrnice **NIS2**.

---

## Hlavní přínosy

* **Integrované řízení:** Propojení evidence aktiv s analýzou rizik a konkrétními bezpečnostními politikami.
* **IoT/OT specifika:** Řešení rizik spojených s telemetrickými jednotkami, integritou firmwaru a privátní konektivitou (APN).
* **Audit-Ready:** Dokumentace je strukturována tak, aby sloužila jako přímý podklad pro certifikační audity.

---

## Obsah repozitáře

### Registry (Excel)
* **Asset-Risk Register CORE.xlsx** – Komplexní matice obsahující:

Asset Register: Seznam aktiv, jejich vlastníci, síťové parametry a kritičnost (CIA).

Risk Register: Identifikace hrozeb, hodnocení dopadů a katalog nápravných opatření (mitigace).

**Statement of Applicability (SoA):** Klíčový dokument pro audit, který mapuje opatření normy ISO 27001:2022 na konkrétní politiky v tomto repozitáři a zdůvodňuje jejich (ne)použití.

### Bezpečnostní politiky, procesy a směrnice (ISMS)
Tyto dokumenty definují procesní rámec pro ochranu aktiv uvedených v registru:

| Dokument | Popis | Cílová oblast |
| :--- | :--- | :--- |
| [**Politika ISMS**](Policies/ISMS-Policy.pdf) | Hlavní nadřazený dokument řízení bezpečnosti. | Strategie & Governance |
| [**Řízení přístupu**](Policies/Access-Control.pdf) | Pravidla pro MFA, hesla a RBAC. | Identita (RISK-USR-01) |
| [**Správa zranitelností**](Policies/Vulnerability-Management.pdf) | Cyklus skenování a SLA pro opravy. | Technický dluh (RISK-VULN-01) |
| [**Řešení incidentů**](Policies/Incident-Response.pdf) | Postup hlášení a eskalace (6 kroků). | Reakce na hrozby |
| [**Zásady přijatelného užití (AUP)**](Policies/Acceptable-Use.pdf) | Pravidla bezpečného chování pro zaměstnance. | Lidský faktor |
| [**Anti-Malware Politika**](Policies/Anti-Malware.pdf) | Ochrana před škodlivým kódem a ransomwarem. | Endpoint Security |
| [**Zálohování a obnova**](Policies/Backup-Recovery.pdf) | Strategie kontinuity a obnovy dat. | Business Continuity |
| [**Řízení změn**](Policies/Change-Management.pdf) | Proces schvalování a testování změn v infrastruktuře. | Provozní stabilita |
| [**Likvidace médií**](Policies/Media-Disposal.pdf) | Postupy pro bezpečné ničení datových nosičů. | Fyzická bezpečnost |
| [**Ochrana soukromí (Privacy)**](Policies/Privacy.pdf) | Zpracování osobních údajů v souladu s GDPR. | Compliance |
| [**Kryptografická politika**](Policies/Cryptographic-Policy.pdf) | Pravidla pro šifrování dat (at rest/in transit) a správu klíčů. | Data Protection |
| [**Clear Desk & Clear Screen**](Policies/Clear-Desk-Clear-Screen.pdf) | Pravidla pro čistý stůl a zamykání obrazovek na pracovišti. | Fyzická bezpečnost |
| [**Práce na dálku (Home Office)**](Policies/Home-Office.pdf) | Bezpečnostní standardy pro práci mimo zabezpečené prostory firmy. | Vzdálený přístup |
| [**Mobilní zařízení a koncové body**](Policies/Mobile-Device-Endpoint.pdf) | Zabezpečení mobilů, notebooků a BYOD (řeší RISK-MDM-01). | Endpoint Security |
| [**Bezpečnost provozu (Ops-Sec)**](Policies/Operations-Security.pdf) | Postupy pro bezpečný provoz IT systémů a logování aktivit. | Provozní bezpečnost |
| [**Business Continuity Plan (BCP)**](Policies/BCP.pdf) | Strategie zachování kritických funkcí firmy při rozsáhlém výpadku. | Kontinuita provozu |
| [**Disaster Recovery Plan (DRP)**](Policies/DRP.pdf) | Technické postupy obnovy IT infrastruktury po havárii. | Obnova systémů |
| [**Správa klíčů (Key Management)**](Policies/Key-Management.pdf) | Životní cyklus šifrovacích klíčů a certifikátů (HSM, rotace). | Kryptografie |
| [**Bezpečné CI/CD (DevSecOps)**](Policies/Secure-CI-CD.pdf) | Integrace bezpečnosti do vývojového cyklu a nasazování kódu. | Bezpečnost vývoje |
| [**Threat Intelligence Process**](Policies/Threat-Intelligence-Process.pdf) | Metodika sběru a analýzy informací o aktuálních kyberhrozbách. | Proaktivní obrana |

---

## Použití

1.  **Audit aktiv:** Identifikujte kritická aktiva v listu `Asset Register`.
2.  **Mitigace rizik:** Aplikujte opatření definovaná v `Policies/` na konkrétní rizika v registru.
3.  **SLA Compliance:** Sledujte lhůty pro opravy zranitelností podle technické kritičnosti aktiva.

---

## Přispívání a úpravy
Tento repozitář slouží jako "živý" základ. Při úpravách pro vlastní potřebu doporučujeme revidovat matici rizik alespoň jednou ročně nebo při významné změně infrastruktury.
