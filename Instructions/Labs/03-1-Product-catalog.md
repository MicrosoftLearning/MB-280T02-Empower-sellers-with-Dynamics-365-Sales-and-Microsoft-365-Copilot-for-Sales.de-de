---
lab:
  title: 'Lab 3.1: Konfigurieren eines Produktkatalogs'
---

# Modul 3: Verwalten von Bestellungen und des Produktkatalogs mit Dynamics 365

## Übungs-Lab 3.1: Verwalten des Produktkatalogs

### Szenario
Da Contoso Coffee wächst, möchte das Unternehmen sein Preisstruktur standardisieren und die Erstellung von Angeboten, Bestellungen und Rechnungen mit genaueren Preisen und Produktdetails vereinfachen. Contoso Coffee hat vor Kurzem seine neueste intelligente Kaffeemaschine herausgebracht. Als Functional Consultant für die Implementierung von Dynamics 365 Sales wurden Sie gebeten, den Produktkatalog zu konfigurieren.

Nach erfolgreichem Absolvieren dieses Labs können Sie Folgendes:
- Erstellen von Einheitengruppen
- Definieren von Preislisten
- Erstellen von Rabattlisten
- Definieren von Produkten und Produktfamilien

### Übung 1 – Produktkatalog

#### Aufgabe 1 – Erstellen einer Einheitengruppe
In dieser Aufgabe erstellen Sie Einheitengruppen für eine Reihe von Kaffeemaschinenfiltern.
1. Navigieren Sie zu Ihrer Dynamics 365-Vertriebshub-Anwendung.
2. Klicken Sie in das Menü "Bereich ändern" (unten links auf dem Bildschirm). Standardmäßig wird „Vertrieb“ unten im linken Menü angezeigt.
3. Wählen Sie im angezeigten Menü **App-Einstellungen** aus.
4. Wählen Sie **Einheitengruppen** im Abschnitt „Produktkatalog“ im linken Menü aus.
5. Klicken Sie auf **+ NEU**.
6. Geben Sie **Filter** für Name ein, geben Sie **Jede** für primäre Einheit ein, und klicken Sie auf **OK.**
7. Sobald die Einheitengruppe geöffnet wird, wählen Sie die Registerkarte „Verwandt“ und dann **Einheiten** aus.
8. Sie werden feststellen, dass Sie jetzt nur über die Standardeinheit „Jede“ verfügen; Sie fügen drei weitere Einheiten hinzu. Klicken Sie auf **+ Neue Einheit**
9. Geben Sie <bpt ctype="x-unknown" id="1" rid="1"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">*</bpt></bpt>Filter<ept id="2" rid="1"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">*</ept></ept> fürr Name, <bpt ctype="x-unknown" id="3" rid="2"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p2">*</bpt></bpt>1<ept id="4" rid="2"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p2">*</ept></ept> für Menge, wählen Sie <bpt ctype="x-unknown" id="5" rid="3"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p3">**</bpt></bpt>Jede<ept id="6" rid="3"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p3">**</ept></ept> für Basiseinheit, und klicken Sie auf <bpt ctype="x-unknown" id="7" rid="4"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p4">**</bpt></bpt>Speichern & Neu erstellen<ept id="8" rid="4"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p4">**</ept></ept> indem Sie das Dropdownsymbol <bpt ctype="x-unknown" id="9" rid="5"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p5">**</bpt></bpt>˅<ept id="10" rid="5"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p5">**</ept></ept> rechts neben der Schaltfläche „Speichern und Schließen“ auswählen.
10. Geben Sie *Paket* für Name, *2* für Menge ein, wählen Sie **Filter** für Basiseinheit aus, und klicken Sie auf **Speichern und Neu erstellen.**
11. Geben Sie *Value Pack* für Name ein, *2* für Menge, wählen Sie **Paket** für Basiseinheit aus, und klicken Sie auf **Speichern und schließen.**
12. Sie sollten jetzt vier Einheitengruppen in der Liste haben.

#### Aufgabe 2 – Erstellen einer Rabattliste
In dieser Aufgabe erstellen Sie eine Rabattliste für Personen, die 15, 20 oder mehr Filter kaufen. Die 15 Filter erhalten einen Rabatt von 15 % und 20 bis 50 Filter erhalten einen Rabatt von 25 %.
1. Wählen Sie **Rabattlisten** im Abschnitt „Produktkatalog“ im linken Menü aus.
2. Klicken Sie auf **+ NEU**.
3. Geben Sie *Mengenrabatt* für den Namen ein, wählen Sie **Prozentsatz** für Typ aus, und klicken Sie auf **Speichern**.
4. Klicken Sie auf **Verwandt**, und wählen Sie **Rabatte** aus.
5. Klicken Sie auf **+ Neuer Rabatt.**
6. Stellen Sie sicher, dass „Mengenrabatt“ für „Rabatttyp“ ausgewählt ist, geben Sie *15* für „Anfangsmenge“, *19* für „Endmenge“, *15* für „Prozentsatz“ ein, und klicken Sie auf **Speichern**.
7. Klicken Sie erneut auf **+ Neu**.
8. Wählen Sie **Mengenrabatt** für den Rabatttyp aus. Geben Sie dann * 20* für „Anfangsmenge“, *50* für „Endmenge“ ein, geben Sie *25* für „Prozentsatz“ ein, und klicken Sie auf **Speichern**.

#### Aufgabe 3 – Erstellen einer Preisliste
In dieser Aufgabe erstellen Sie eine Preisliste für die Filter.
1. Wählen Sie **Preislisten** im Abschnitt „Produktkatalog“ im linken Menü aus.
2. Klicken Sie auf **+ NEU**.
3. Geben Sie *Filter Direct* für Name ein, wählen Sie **US-Dollar** für Währung aus, und klicken Sie auf **Speichern und Schließen.**

#### Aufgabe 4 – Erstellen von Produkten
In dieser Aufgabe erstellen Sie Produkte.
1. Klicken Sie auf den Bereich **App-Einstellungen ändern**.
2. Wählen Sie **Sales** aus.
3. Wählen Sie im Abschnitt „Sicherheiten“ des linken Menüs **Produkte** aus.
4. Klicken Sie auf **Produkt hinzufügen.**
5. Geben Sie *Airpot XL 6 Monatsfilter* für „Name“ ein, geben Sie *AXL6MF-1234* für „Produkt-ID“ ein, wählen Sie **Filter** für „Einheitsgruppe“ aus, wählen Sie **Filter** für „Standardeinheit“ aus, geben Sie *2* für „Unterstützte Dezimalstellen“ ein und klicken Sie auf **Speichern**. (Möglicherweise müssen Sie das blaue Häkchen neben den unterstützten Dezimalstellen aktivieren, um den Vorschlag anzunehmen.)
6. Wählen Sie die Registerkarte **Zusätzliche Details** aus.
7. Klicken Sie oben rechts im Abschnitt „Preislistenelemente“ auf die **vertikalen Auslassungspunkte**. Klicken Sie auf das Element **+ Neue Preisliste**.
8. Wählen Sie **Direkt filtern** für „Preisliste“, wählen Sie **Mengenrabatt** für „Rabattliste“ und dann **Ganzes** für „Mengenverkaufsoption“ aus.
9. Wählen Sie die Registerkarte **Preisinformationen** aus, geben Sie *25* für „Betrag“ ein, und wählen Sie **Speichern und Schließen** aus.
10. Wenn die automatische Veröffentlichung aktiviert ist, überspringen Sie diesen Schritt. (Die Veröffentlichung wird nicht auf der Befehlsleiste angezeigt). Wählen Sie andernfalls **Veröffentlichen** und **Bestätigen** aus, um das Produkt zu veröffentlichen.
11. Wählen Sie im linken Menü **Produkte** in der Gruppe „Sicherheiten“ aus.
12. Klicken Sie auf **Produkt hinzufügen.**
13. Geben Sie *Airpot XL Reservoir Extension* fürr „Name“ ein, geben Sie *AXLRE-4321* für „Produkt-ID“ ein, wählen Sie **Standardeinheit** für „Einheitengruppe“ aus, wählen Sie **Primäre Einheit** für „Standardeinheit“ aus, wählen Sie das blaue Häkchen neben der 2 für „Unterstützte Dezimalstellen“ aus und klicken Sie auf **Speichern**.
14. Wählen Sie die Registerkarte **Zusätzliche Details** aus.
15. Klicken Sie oben rechts im Abschnitt „Preislistenelemente“ auf die **vertikalen Auslassungspunkte**. Klicken Sie auf **+ Neues Preislistenelement.**
16. Wählen Sie **Direkt filtern** für „Preisliste“ aus. Wählen Sie **Ganzes** für „Mengenverkaufsoption“ aus.
17. Wählen Sie die Registerkarte **Preisinformationen** aus, geben Sie *299 $* für „Betrag“ ein, und wählen Sie **Speichern und Schließen** aus.
18. Wenn die automatische Veröffentlichung aktiviert ist, überspringen Sie diesen Schritt. Wählen Sie andernfalls **Veröffentlichen** und **Bestätigen** aus, um das Produkt zu veröffentlichen.
19. Wählen Sie im linken Menü **Produkte** aus.
20. Klicken Sie auf **Produkt hinzufügen.**
21. Geben Sie *Airpot XL Pot Extender* für „Name“ ein, geben Sie *AXPLE-7894* für „Produkt-ID“ ein, wählen Sie **Standardeinheit** für „Einheitengruppe“ aus, wählen Sie **Primäre Einheit** für „Standardeinheit“ aus, aktivieren Sie das blaue Häkchen neben der 2 für „Unterstützte Dezimalstellen“ und klicken Sie auf **Speichern.**
22. Wählen Sie die Registerkarte **Zusätzliche Details** aus.
23. Klicken Sie oben rechts im Abschnitt „Preislistenelemente“ auf die **vertikalen Auslassungspunkte**. Klicken Sie auf **+ Neues Preislistenelement.**
24. Wählen Sie **Direkt filtern** für „Preisliste“ aus. Wählen Sie **Ganzes** für „Mengenverkaufsoption“ aus.
25. Wählen Sie die Registerkarte **Preisinformationen** aus, geben Sie *199* für „Betrag“ ein, und wählen Sie **Speichern und Schließen** aus.
26. Wenn die automatische Veröffentlichung aktiviert ist, überspringen Sie diesen Schritt. Wählen Sie andernfalls **Veröffentlichen** und **Bestätigen** aus, um das Produkt zu veröffentlichen.
27. Wählen Sie im linken Menü **Produkte** aus.
28. Die von Ihnen erstellten Produkte sollten in der Ansicht „Alle Produkte, Familien und Bundles“ angezeigt werden. Sie können zu dieser Ansicht wechseln, indem Sie das Dropdownsymbol <bpt ctype="x-unknown" id="1" rid="1"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</bpt></bpt>Dropdownsymbol ˅<ept id="2" rid="1"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</ept></ept> neben dem Titel der Standardansicht auswählen. 
