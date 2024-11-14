---
lab:
  title: 'Lab 2.1: Verwalten von Leads und Verkaufschancen'
---

# Modul 2: Verwalten von Leads und Verkaufschancen mit Dynamics 365 Sales

## Übungs-Lab 2.1 – Verwalten von Leads und Verkaufschancen

### Szenario
Contoso Coffee möchte Dynamics 365 Sales verwenden, um ihren Verkaufsprozess zu formalisieren und einen Rückstand unbearbeiteter Leads zu adressieren, die vom Marketingteam von Messen und Kampagnen importiert wurden. Als Vertriebsanalystin bzw. -analyst bei Contoso Coffee wurden Sie gebeten, Leaddatensätze zu bewerten und zu aktualisieren, um sicherzustellen, dass die Geschäftsleitung beim bevorstehenden Leadership-Meeting mit einem korrekten Pipeline-Bericht arbeitet.

Nach erfolgreichem Absolvieren dieses Labs können Sie Folgendes:
- Erstellen und Aktualisieren von Leaddatensätzen
- Leads qualifizieren und disqualifizieren
- Reaktivieren von Leaddatensätzen

### Übung 1: Verwalten von Kundinnen und Kunden

#### Aufgabe 1 – Erstellen von Leads
In dieser Aufgabe erstellen Sie drei Leads, einen ohne Firmeninformationen und zwei mit Firmeninformationen.
1. Navigieren Sie zu Ihrer Dynamics 365-Vertriebshub-Anwendung. Stellen Sie sicher, dass Sie sich im Bereich „Vertrieb“ befinden, indem Sie das Dropdownmenü unten links verwenden.
2. Wählen Sie über die Navigation auf der linken Seite in der Gruppe „Vertrieb“ die Option **Leads** aus.
3. Wählen Sie im Bereich „Arbeitselemente“ die Option **Schreibgeschütztes Raster** aus, um den Ansichtstyp zu ändern.
4. Wählen Sie in dem angezeigten Menü die Schaltfläche **+ Neu** aus.
5. Geben Sie für Thema *Kaffeemaschinen-Lead ohne Unternehmen*, für Vorname *Erika*, für Nachname *Mustermann* ein.
6. Akzeptieren Sie den Vorschlag des **Cafeteria-Managers**, der im Feld „Position“ ausgefüllt wurde.
7. Wählen Sie die Schaltfläche **Speichern** aus. Wählen Sie auf der Befehlsleiste oben erneut **+ Neu** aus.
8. Geben Sie für Thema *Kaffeemaschinen-Lead bei Unternehmen*, für Vorname *Max*, für Nachname *Mustermann*, für Unternehmen *Mustermann Inc.* ein, und klicken Sie auf **Speichern.**
9. Wählen Sie auf der Befehlsleiste ein weiteres Mal die Schaltfläche **+ Neu** aus.
10. Geben Sie für Thema *Weiterer Kaffeemaschinen-Lead*, für Vorname *Jack*, für Nachname *Rogers*, für Unternehmen *Test Coffee Shop, Inc.* ein, und klicken Sie auf **Speichern**.

### Übung 2 – Leadqualifikationen
In dieser Übung qualifizieren/disqualifizieren Sie Leads und sehen, welche Datensätze erstellt werden, wenn ein Lead den Qualifizierungsprozess durchläuft.

#### Aufgabe 1 – Qualifizieren des Kaffeemaschinen-Leads der ohne Firmeninformationen
1. Wechseln Sie zur Vertriebshub-Anwendung.
2. Wählen Sie **Leads** aus.
3. Klicken Sie im Bereich „Arbeitselemente“ auf die Schaltfläche **Schreibgeschütztes Raster**.
4. Suchen Sie **Kaffeemaschinen-Lead ohne Unternehmen**, und wählen Sie es aus.
5. Klicken Sie im Menü oben auf **Sich qualifizieren**.
6. Der Lead wird in einen neuen Verkaufschancendatensatz qualifiziert.
   - **HINWEIS:** Wenn die neue Verkaufschance nicht automatisch geöffnet wird, wählen Sie „Verkaufschancen“ im linken Menü aus, um alle offenen Verkaufschancen anzuzeigen. Öffnen Sie dann den Kaffeemaschinen-Lead ohne Unternehmensverkaufschance.
7. Suchen Sie das Feld „Kontakt“. Sie werden feststellen, dass Erika Mustermann jetzt ein Kontaktdatensatz in der Anwendung ist, die Sie öffnen können.
8. Suchen Sie das Feld „Konto“ (im Header des Verkaufschancendatensatzes). Beachten Sie, dass das Feld leer ist.
9. Klicken Sie auf **Speichern**.

#### Aufgabe 2 – Qualifizieren des Kaffeemaschinen-Leads für das Unternehmen
1. Wechseln Sie zur Vertriebshub-Anwendung.
2. Wählen Sie **Leads** aus.
3. Suchen die Option „Kaffeemaschinen-Lead für das Unternehmen“, und öffnen Sie sie.
4. Klicken Sie im Menü oben auf **Sich qualifizieren**.
5. Der Lead wird wie der vorherige Lead qualifiziert, und Sie werden aus dem qualifizierten Lead zum neu erstellten Verkaufschancendatensatz weitergeleitet.
6. Suchen Sie das Feld „Kontakt“. Sie werden feststellen, dass Max Mustermann jetzt ein Kontaktdatensatz ist.
7. Suchen Sie das Feld „Konto“. Sie werden feststellen, dass Mustermann, Inc. jetzt ein Kontodatensatz ist.

#### Aufgabe 3 – Disqualifizieren eines Leads
1. Wechseln Sie bei Bedarf zu Ihrer Vertriebshub-Anwendung.
2. Wählen Sie **Leads** aus.
3. Suchen Sie die Option „Weiterer Kaffeemaschinen-Lead“, und öffnen Sie sie.
4. Klicken Sie auf **Disqualifizieren** (möglicherweise müssen Sie die vertikale Auslassungspunkteschaltfläche auswählen, damit sie angezeigt wird).
5. Wählen Sie im angezeigten Menü die Option **Nicht mehr interessiert** aus.
6. Der Lead wird disqualifiziert, der Status wird in „Nicht mehr interessiert“ geändert, und der Datensatz wird schreibgeschützt.

#### Aufgabe 4 – Reaktivieren eines Leads
1. Wechseln Sie bei Bedarf zu Ihrer Vertriebshub-Anwendung.
2. Wählen Sie in der Sitenavigation in der Gruppe „Vertrieb“ die Option **Leads** aus.
3. Der disqualifizierte Lead ist nicht mehr in der Ansicht „Meine offenen Leads“ vorhanden. Wählen Sie den Abwärtspfeil neben „Meine offenen Leads“ aus, und ändern Sie die Ansicht in **Geschlossene Leads.**
4. Suchen Sie einen anderen Kaffeemaschinen-Lead, und öffnen Sie ihn.
5. Klicken Sie auf **Lead reaktivieren.**
6. Der Lead wird reaktiviert, der Status wird wieder in „Neu“ geändert, und der Datensatz kann bearbeitet werden.

### Übung 3 – Arbeiten mit Verkaufschancen
In dieser Übung werden Sie den Prozess der Bearbeitung einer Verkaufschance durch den Vertriebsprozess kennenlernen.

#### Aufgabe 1 – Verwalten des Kaffeemaschinen-Leads für das Unternehmen
1. Wechseln Sie bei Bedarf zu Ihrer Vertriebshub-Anwendung.
2. Wählen Sie über die Navigation auf der linken Seite **Verkaufschancen** in der Gruppe „Vertrieb“ aus.
3. Suchen und öffnen Sie die Verkaufschance **Kaffeemaschinen-Lead für das Unternehmen**.
4. Wählen Sie im daraufhin angezeigten Bereich „Verkaufschance“ die Schaltfläche **Zum Hauptfenster wechseln** (neben der Schaltfläche X (Schließen)) aus.
5. Füllen Sie den Verkaufschancendatensatz wie folgt aus:
   - Budgetbetrag: 17.000 $
   - Kaufzeitrahmen: Dieses Quartal
   - Kaufvorgang: Komitee
   - Beschreibung: Sie möchten ihre aktuellen Kaffeemaschinen an mehreren Standorten aktualisieren.
6. Erweitern Sie die Datensatzkopfzeile oben, und füllen Sie sie wie folgt aus:
   - Gesch. Abschlussdatum – Geben Sie das Datum von morgen ein.
   - Gesch. Umsatz: 16.500 $
7. Wählen Sie auf der Zeitskala die **+** (fügen Sie einen Zeitskaladatensatz hinzu) aus.
8. Wählen Sie im nächsten Menü die Option **Telefonanruf** aus.
9. Legen Sie den Telefonanruf wie folgt an:
   - Betreff: Erstanruf an Max.
   - Fällig: Geben Sie das heutige Datum und 16:30 Uhr ein
10. Wählen Sie **Speichern und schließen** aus.
11. Wählen Sie bei göffneter Verkaufschance die **Entwicklungsphase** im Geschäftsprozessflow „Lead zu Verkaufschance“ aus. Gehen Sie wie folgt weiter vor:
   - Kundenbedarf: Sie möchten ihre Kaffeemaschinen an mehreren Standorten aktualisieren.
   - Vorgeschlagene Lösung: Empfehlen mehrerer AirPot Duo-Maschinen.
   - Stakeholder identifizieren: Abgeschlossen
   - Mitbewerber identifizieren: Abgeschlossen
12. Wählen Sie die Schaltfläche **Nächste Phase** aus.
13. Legen Sie in der Phase „Vorschlagen“ alle Felder auf **Abgeschlossen** fest.
14. Wählen Sie die Schaltfläche **Nächste Phase** aus.
15. Wählen Sie eine beliebige Stelle außerhalb der Geschäftsprozessphase aus, um sie zu schließen.
16. Wählen Sie im Abschnitt „Assistent“ unter „Benachrichtigungen“ das zuvor erstellte Element **Telefonanruf** aus, um es zu öffnen.
17. Wählen Sie **Complete** (Fertig stellen) aus. (Beachten Sie, dass das Element aus Ihren Benachrichtigungen nicht mehr angezeigt wird.)
18. Wählen Sie im Vertriebsprozess „Lead zu Verkaufschance“ die **Phase „Schließen“** aus.
19. Markieren Sie alle Elemente in der Phase „Schließen“ als **Abgeschlossen.**
20. Klicken Sie auf die Schaltfläche **Fertig stellen**.
21. Wählen Sie auf der Befehlsleiste oben die Schaltfläche **Als „Gewonnen“ schließen** aus.
22. Wählen Sie auf dem Bildschirm „Verkaufschance schließen“ die Schaltfläche **OK** aus.

Herzlichen Glückwunsch, Sie haben erfolgreich Leads und Verkaufschancen in Dynamics 365 Sales erstellt und verwaltet.
