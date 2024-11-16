---
lab:
  title: 'Lab 5.1: Anpassen eines Geschäftsprozessflows'
---

# Modul 5: Arbeiten mit Dynamics 365 Sales Insights und Vertriebsbeschleunigung 

## Übungslab 5.1: Anpassen eines Geschäftsprozessflows

## Szenario

Contoso Coffee möchte seinen bewährten Geschäftsprozess für den Vertrieb um ein paar zusätzliche Schritte erweitern. Obwohl Verkaufspersonen in der Vergangenheit mit diesem Framework erfolgreich waren, berichten sie, dass einige neue Vorschläge helfen würden, Leads zu fördern und Verträge mit hohem Wert abzuschließen.

Die Verkäufer möchten die folgenden Schritte in ihren Geschäftsprozess aufnehmen:

-   Bei hochwertigen potenziellen Kunden mit einem Budget von mehr als \$1.000.000 sollte der Vertriebslead persönlich Kontakt aufnehmen, um das Interesse zu bestätigen, bevor er zur Qualifizierung übergeht.
-   Stellen Sie in der Entwicklungsphase sicher, dass die Verkauspersonen bestehende Kundenprobleme verfolgen, um potenzielle Bereiche für Add-On Vertrieb zu identifizieren, die zuvor möglicherweise übersehen wurden.

In diesem Lab werden wir den Geschäftsprozessflow an die Anforderungenn unserer Verkaufspersonen anpassen.

## Übung 1 – Geschäftsprozessflow anpassen

### Aufgabe 1 – Erstellen eines Geschäftsprozessflows

In dieser Aufgabe erstellen Sie einen neuen Geschäftsprozessflow aus dem Verkaufschancen-Verkaufsprozess und testen dann den neuen BPF.

1.  Navigieren Sie zu [https://make.powerapps.com](https://make.powerapps.com/).
2.  Vergewissern Sie sich, dass Sie sich in der Umgebung**Vertriebs-Testversion**befinden.
3.  Wählen Sie **Lösungen** aus.
4.  Wählen Sie in der oberen Befehlsleiste die Schaltfläche **+ Neue Lösung**.
5.  Geben Sie in das Feld **Anzeigename** **Contoso** ein.
6.  Wählen Sie **+ Neuer Herausgeber**.
7.  Konfigurieren Sie den neuen Herausgeber wie folgt.
    1.  **Anzeigename:** Contoso
    2.  **Name:** Contoso
    3.  **Präfix:** Contoso
    4.  **Auswahlwertpräfix:** 10000
8.  Wählen Sie **Speichern**.
9.  Wählen Sie unter Herausgeber den neuen Herausgeber **Contoso**, den Sie gerade erstellt haben.
10. Klicken Sie auf **Erstellen**.
11. Wählen Sie in der **Befehlsleiste** **Hinzufügen** vorhanden.
12. Wählen Sie im angezeigten Menü **Automatisierung**\>**Prozess**.
13. Jetzt finden wir den **Verkaufsprozess** in der Liste der Prozesse. (Sie können jetzt das Suchfeld in der oberen rechten Ecke verwenden.) Wenn Sie es gefunden haben, wählen Sie es aus.
14. Wählen Sie die Schaltfläche **Hinzufügen** aus.
15. Wählen Sie den **Verkaufsprozess**, um ihn zu öffnen.
16. Eine neue Registerkarte öffnet den BPF-Editor. (Lassen Sie die alte Registerkarte mit der Lösungsliste geöffnet.) Fügen wir nun die Schritte hinzu, die unsere Verkaufspersonen angefordert haben.
17. Zunächst fügen wir eine Bedingung hinzu, um das Budget der Kundschaft zu prüfen und unsere potenziellen hochwertigen Kunden mit Budgets über \$1.000.000 zu identifizieren. Ziehen Sie **Bedingung** von der Registerkarte **Komponenten** und platzieren Sie es zwischen den Stufen **Qualifizieren** und **Entwickeln**.
18. Wählen Sie die **Bedingung**, gehen Sie zur Registerkarte **Eigenschaften** und geben Sie **Budget prüfen** für **Anzeigename** ein.
19. Wählen Sie unter **Regeln,** **Budgetbetrag** für **Feld**.
20. Wählen Sie **Ist größer als oder gleich** für **Operator**.
21. Wählen Sie **Wert** für **Typ**.
22. Geben Sie **1.000.000** für **Wert** ein und klicken Sie auf **Anwenden**.
23. Jetzt müssen wir eine neue Phase hinzufügen, um die Bedingung abzuschließen. Fügen Sie im Bereich Komponenten rechts neben der Bedingung eine neue Stufe hinzu.
24. Klicken Sie auf die Registerkarte **Eigenschaften**.
25. Geben Sie **Interesse bestätigen** für **Anzeigename** ein. Wählen Sie **Übernehmen**.
26. Klicken Sie auf die Schaltfläche **Details** in der Phase **Interesse bestätigen**.
27. Wählen Sie das **Eingabekriterium \#1 Neuer Schritt** innerhalb der Stufe**Interesse bestätigen** aus.
28. Öffnen Sie auf der Registerkarte **Eigenschaften** das Dropdown-Menü für **Datenfeld.** Wählen Sie **Interesse bestätigen**. Der Schrittname wird automatisch aktualisiert.
29. Aktivieren Sie das Kontrollkästchen **Erforderlich** und klicken Sie auf **Anwenden**.
30. Als Nächstes werden wir einen neuen Schritt hinzufügen, um in der Entwicklungsphase nach den Problembereichen der Kundschaft zu fragen, wie von unseren Verkaufspersonen gewünscht. Wählen Sie die Stufe **Entwickeln** und erweitern Sie **Details.**
31. Ziehen Sie im Fensterbereich Komponenten einen **Datenschritt** unter den Datenschritt \#4.
32. Wählen Sie in der Dropdown-Liste Datenfeld die Option **Problembereiche der Kundschaft.** Es wird nun vorgeschlagen, in der Entwicklungsstufe die Problembereiche der Kundschaft zu identifizieren. Dieses Feld wird nicht als erforderlich markiert.
33. Wählen Sie **Übernehmen**.
34. Klicken Sie auf **Validieren**, um sicherzustellen, dass die von Ihnen vorgenommenen Änderungen gültig sind und dass die BPF wie erwartet funktioniert.
35. Wenn es keine Probleme gibt, klicken Sie auf **Aktualisieren.**
36. Schließen Sie die Registerkarte mit dem Geschäftsprozessflow-Editor.
37. Kehren Sie zur vorherigen Registerkarte zurück und klicken Sie im Popup-Fenster im Bereich Standardlösung auf **Fertig**. Wählen Sie im oberen Menü **Alle Anpassungen veröffentlichen.** (Möglicherweise müssen Sie die Suche nach „Verkaufschancen“ im Textfeld oben rechts löschen, um diese Schaltfläche sehen zu können).
38. Warten Sie auf die **Veröffentlichung** Ihrer Anpassungen.

### Aufgabe 2 – Testen des Geschäftsprozessflows

1.  Kehren Sie zur Vertriebshub-App zurück.
2.  Navigieren Sie zum Abschnitt **Verkaufschancen** und klicken Sie auf **+Neu**, um eine neue Verkaufschance zu erstellen. Geben Sie ein Thema wie etwa **Interessiert an neuen Maschinen** ein.
3.  Wählen Sie einen bestehenden Kontakt für das Kontaktfeld aus.
4.  Öffnen Sie die Stufe **Qualifizieren** des Geschäftsprozessflows im Vertriebsprozess. Geben Sie *\$800.000* als geschätztes Budget ein.
5.  Der Geschäftsprozessflow sollte vier Stufen umfassen: **Sich qualifizieren**, **Entwickeln**, **Vorschlagen** und **Schließen**. Die Stufe Interesse bestätigen ist nicht Teil des Prozesses, wenn der Budgetbetrag weniger als \$1.000.000 beträgt.
6.  Ändern Sie den **Budgetbetrag** in *\$1.200.000.*
7.  Der Geschäftsprozessflow sollte nun fünf Stufen umfassen: **Sich qualifizieren**, **Interesse bestätigen**, **Entwickeln**, **Vorschlagen** und **Schließen**. Gehen Sie von der Qualifizierungsstufe zur nächsten Stufe über.
8.  Die Verkaufschance**Speichern**.
9.  Wählen Sie die Stufe **Qualifizieren** und dann die Schaltfläche **Nächste Stufe** aus, um zur Stufe **Interesse bestätigen** zu gelangen.
10. Bestätigen Sie Ihr Interesse, indem Sie **Nein,** dann **Ja.** wählen.
11. Wählen Sie die Schaltfläche **Nächste Stufe**, um zur Stufe **Entwickeln** zu gelangen.
12. Vergewissern Sie sich, dass das Feld Problembereiche der Kundschaft unten in der Entwicklungsstufe angezeigt wird.
13. Geben Sie *Die aktuellen Maschinen können das Kundenaufkommen nicht bewältigen* in das Feld Problembereiche der Kundschaft ein.
14. Wählen Sie **Nächste Phase** aus.
15. **Speichern** Sie den Datensatz.

