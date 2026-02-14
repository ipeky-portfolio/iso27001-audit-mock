# Stichprobenverfahren und Evidenzsammlung

## 1. Grundsatz
Als Lead Auditor wende ich eine **risikobasierte Stichprobennahme** gemäß ISO 19011 an. Das Ziel ist eine repräsentative Auswahl, um Aussagen über die Wirksamkeit eines Prozesses zu treffen.

## 2. Methoden

| Methode | Anwendung | Beispiel |
| :--- | :--- | :--- |
| **Vollerhebung** | Kritische Prozesse mit geringem Volumen. | Prüfung **aller** 5 Domain-Administrator-Accounts. |
| **Zufallsstichprobe** | Prozesse mit hohem Volumen (n>100). | Prüfung von **10%** der User-Accounts aus dem Active Directory Export für Passwort-Policy-Konformität. |
| **Risikobasierte Auswahl** | Prozesse mit bekannten Schwachstellen. | Prüfung der **neu eingestellten Mitarbeiter** im Bereich "Entwicklung", da hier häufig Rechte zu großzügig vergeben werden. |

## 3. Praxisbeispiel: Prüfung "Benutzerzugangskontrolle" (Annex A 5.15)

* **Umfang:** 500 aktive Nutzer.
* **Stichprobe:**
    1.  **Technisch:** 20 zufällig ausgewählte Benutzerkonten auf Einhaltung der Komplexitätsregeln (min. 12 Zeichen, MFA aktiv) prüfen.
    2.  **Prozessual:** 5 neue Mitarbeiter des letzten Quartals prüfen (Existenz eines unterzeichneten User-Antrags & Revisionssichere Anlage).
    3.  **Fokus:** 3 Mitarbeiter prüfen, die das Unternehmen verlassen haben (Wurden Rechte innerhalb von 24h entzogen? Abgleich HR-Austrittsliste mit AD-Deaktivierung).

## 4. Dokumentation der Evidenz
Alle Stichproben werden im `Evidence_Register.md` dokumentiert, inklusive Zeitstempel, getester Datensatz und Ergebnis (Konform / Nicht-Konform).
