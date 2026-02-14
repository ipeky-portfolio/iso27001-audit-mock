# Testmodul: Zugangskontrolle (Access Control)

**Referenz:** ISO 27001:2022 Annex A 5.15, 5.16, 5.18

## 1. Testschritte
1.  **Richtlinienprüfung:** Besteht eine klare Berechtigungsrichtlinie (RBAC - Role Based Access Control)?
2.  **User Provisioning:** Prüfung des Onboarding-Prozesses für 3 Beispiel-Mitarbeiter.
3.  **Rechte-Audit:** Abgleich der Berechtigungen eines Administrators mit der Jobbeschreibung.
4.  **De-Provisioning:** Prüfung, ob Zugänge von 3 ausgeschiedenen Mitarbeitern innerhalb von 24h gesperrt wurden.

## 2. Detaillierte Beispiele für Konformität
* **A.5.15:** Alle administrativen Zugriffe erfolgen über einen **"Privileged Access Management" (PAM) Tool** mit Sitzungsaufzeichnung.
* **A.5.18:** Ein vollautomatisierter Prozess sperrt Accounts **sofort** nach Deaktivierung im HR-System.

## 3. Mögliche Abweichungen (Nonconformities)
* **Minor NC:** Ein Benutzer hat seit 6 Monaten **Leserechte** auf einen SharePoint-Ordner, der nicht mehr seiner Abteilung entspricht.
* **Major NC:** Die **MFA (Multi-Faktor-Authentifizierung)** ist für VPN-Zugriffe zwar aktiviert, aber Administratoren können diese für sich selbst umgehen.
