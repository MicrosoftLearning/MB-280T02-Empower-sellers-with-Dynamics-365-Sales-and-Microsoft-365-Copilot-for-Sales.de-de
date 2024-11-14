---
lab:
  title: "Lab\_3.2: Angebote erstellen"
---

# Modul 3: Verwalten von Bestellungen und des Produktkatalogs mit Dynamics 365

## Übungs-Lab 3.2 – Erstellen von Angeboten

### Szenario
Als Vertriebsanalyst für die Implementierung von Dynamics 365 Sales bei Contoso Coffee möchten Sie sicherstellen, dass Vertriebsmitarbeiter die Produktkatalogerweiterungen während des gesamten Vertriebslebenszyklus nutzen können. Um sicherzustellen, dass die Funktionalität ordnungsgemäß funktioniert, testen Sie den Prozess der Angebotserstellung für eine neue Verkaufschance.

Nach erfolgreichem Absolvieren dieses Labs können Sie Folgendes:
- Erstellen von Verkaufschancen und Hinzufügen von Verkaufschancenpositionen
- Erstellen eines Angebots aus einer Verkaufschance

### Übung 1 – Erstellen eines Angebots

#### Aufgabe 1 – Hinzufügen von Artikelpositionen
In dieser Aufgabe erstellen Sie eine Verkaufschance und fügen Artikelpositionen hinzu.
1. Navigieren Sie zu Ihrer Dynamics 365-Vertriebshub-Anwendung.
2. Wählen Sie im linken Menü in der Gruppe „Vertrieb“ die Option **Verkaufschancen** aus.
3. Klicken Sie auf **+ NEU**.
4. Geben Sie *Interesse an Airpot XL Zubehör* für „Thema“ ein, und wählen Sie **Max Mustermann** für Kontakt aus.
5. Wählen Sie in der Datensatzkopfzeile oben den **Abwärtspfeil** neben dem Feld „Besitzer“ aus, und wählen Sie für „Konto“ die Option **Test Coffee Shop, Inc.** aus. Wählen Sie **Speichern**.
6. Wählen Sie die Registerkarte **Produkte** aus.
7. Sie müssen eine Preisliste auswählen, bevor Sie Verkaufschancenprodukte hinzufügen können. Wählen Sie **Direkt filtern** für „Preisliste“ aus.
8. Wählen Sie **System berechnet** für „Umsatz“ aus.
9. Klicken Sie oberhalb des Unterrasters auf **+ Produkte hinzufügen.**
10. Suchen Sie in der Liste „Alle Produkte“ **Airpot XL 6 Month Filter**, geben Sie *6* für „Menge“ ein, und wählen Sie **Hinzufügen** aus.
11. Suchen Sie in der Liste der Produkte **AirpotXL Pot Extender**, geben Sie *1* für „Menge“ ein, und wählen Sie **Hinzufügen** aus.
12. Suchen Sie in der Liste der Produkte **Airpot XL Reservoir Extension**, geben Sie *1* für „Menge“ ein, und wählen Sie **Hinzufügen** aus.
13. Sie werden sehen, dass drei Produkte hinzugefügt werden. Wählen Sie **Speichern**.
14. Doppelklicken Sie auf das Produkt **Airpot XL 6 Month Filter**.
15. Suchen Sie das Feld „Mengenrabatt“. Sie werden feststellen, dass es keinen Rabatt gibt.
16. Ändern Sie die Menge zu *15*, und klickne Sie außerhalb des Feldes. Der Rabatt wird nun gestartet, und das Feld „Mengenrabatt“ zeigt den rabattierten Wert an.
17. Wählen Sie **Speichern und schließen** aus.

#### Aufgabe 2 – Erstellen eines Angebots
In dieser Aufgabe erstellen Sie ein Angebot aus der Verkaufschance, die Sie in Aufgabe 1 erstellt haben.
1. Gehen Sie zu Ihrer Dynamics 365 Sales Hub-Anwendung, falls noch nicht geschehen.
2. Öffnen Sie bei Bedarf die Verkaufschance, die Sie in der vorherigen Aufgabe erstellt haben. Sie wird **Interesse an Airpot XL Zubehör** heißen.
3. Wählen Sie die Registerkarte **Angebote** aus.
4. Klicken Sie oberhalb des Unterrasters auf **+ Neues Angebot.**
5. Das Angebotsformular wird geöffnet, und relevante Informationen werden aus der Verkaufschance kopiert.
6. Überprüfen Sie auf der Angebotsseite „Interesse an Airpot XL Zubehör“ das Unterraster „Produkte“, und stellen Sie sicher, dass Produkte und deren Mengen Ihren Erwartungen entsprechen. Sie können die Mengen ändern und den Preis der einzelnen Artikel rabattieren.
7. Wählen Sie auf der Befehlsleiste **Angebot aktivieren** aus. (Je nach Größe Ihres Browsers müssen Sie möglicherweise die Auslassungspunkte auswählen, um diese Option anzuzeigen.)
8. Klicken Sie in der Befehlsleiste auf **Als PDF exportieren** und wählen Sie **Angebot für Kunden drucken** aus. Klicken Sie auf **Download**.
9. Öffnen Sie das generierte Dokument, und sehen Sie sich an, wie das Angebot aussieht.
10. Schließen Sie das PDF.
11. Schließen Sie das Fenster „Als PDF exportieren“.

