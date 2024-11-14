---
lab:
  title: 'Lab 5.2: Eine Sequenz erstellen'
---

# Modul 5: Arbeiten mit Dynamics 365 Sales Insights und Vertriebsbeschleunigung 

## Übungslab 5.2: Eine Sequenz erstellen

### Szenario
Die Verkaufspersonen von Contoso Coffee sind der Meinung, dass der Absatz verbessert werden könnte, wenn die „Best Practices“ der Organisation leichter zu befolgen wären. Nach Prüfung hat das Vertriebsmanagement von Contoso eine ideale Sequenz von Verkaufsveranstaltungen für Verkaufspersonen festgelegt. Sie wollen bewährte Methoden durchsetzen, indem sie eine Reihe von aufeinanderfolgenden Aktivitäten festlegen, die Verkaufspersonen bei der Qualifizierung von Leads befolgen müssen. Sie sollten dafür sorgen, dass die Verkaufspersonen sie während ihres Alltags so einfach wie möglich befolgen können. Sie haben festgestellt, dass eine Sequenz die beste Möglichkeit ist, dies zu erreichen.

Nach erfolgreichem Abschluss dieses Labs werden Sie in der Lage sein:

-   Segment erstellen
-   Eine Sequenz erstellen
-   Definieren von Sequenzaktivitäten
-   Aktivieren und Verbinden von Sequenzen mit Datensätzen

## Übung 1: Erstellen und Anfügen von Sequenzen zu Datensätzen

### Aufgabe 1: Aktivieren der Vertriebsbeschleunigung

1.  Wählen Sie in der Gruppe Sales Insights die Option **Globale Einstellungen.**
2.  Wählen Sie in der Untergruppe „Vertriebsbeschleunigung“ die Registerkarte **Sequenzen** aus.
3.  Sie werden aufgefordert, den Arbeitsbereich so einzurichten, dass Sie Sequenzen verwenden können. Wählen Sie die Schaltfläche **Arbeitsbereich einrichten**.
4.  Wählen Sie die Taste **Express-Setup**.
5.  Wählen Sie im Abschnitt Datensatztypund Formular **+ Datensatztyp hinzufügen**. Wählen Sie **Verkaufschancen.**
6.  Konfigurieren Sie das Standardformular für jeden Datensatztyp wie folgt:
    -   Leads: Sales Insights
    -   Verkaufschancen: Sales Insights
7.  Wählen Sie die Schaltfläche **Veröffentlichen** aus.
    -   Hinweis: Es kann einige Minuten dauern, bis Ihre Änderungen übernommen werden.

### Aufgabe 2: Ein Segment erstellen

1.  Wenn Sie dies noch nicht getan haben, ändern Sie den Bereich in **Sales Insights-Einstellungen.**
2.  Wählen Sie in der Gruppe Sales Insights die Option **Globale Einstellungen.**
3.  Wählen Sie in der Untergruppe Verkaufsbeschleunigung die Registerkarte **Arbeitszuweisung** aus.
4.  Vergewissern Sie sich, dass der **Datensatztyp** auf **Leads** eingestellt ist, und wählen Sie die Schaltfläche **Neues Segment** aus.
5.  Geben Sie in das Feld **Name** den Text **Trade Show Leads** ein und wählen Sie dann die Schaltfläche **Weiter**.
6.  Wählen Sie auf der Registerkarte **Segmentdefinition** die Schaltfläche **Hinzufügen**.
7.  Wählen Sie im angezeigten Menü **Zeile hinzufügen** aus.
8.  Konfigurieren Sie die Bedingung wie folgt:
    1.  **Lead-Quelle** - **Gleich** - **Trade Show**
9.  Wählen Sie **Ergebnisse simulieren**.

    Sie sollten einen Bildschirm zur Simulation von Segmentmitgliedern sehen, der alle Leads enthält, die Ihren Kriterien entsprechen.

10. Schließen Sie das Fenster **Segmentmitglieder-Simulation**.
11. Wählen Sie die Schaltfläche **Speichern** aus.
12. Wählen Sie die Schaltfläche **Aktivieren**.

## Übung 2: Erstellen und Anfügen von Sequenzen an Datensätze

### Aufgabe 1: Neue Sequenz erstellen

1.  Wenn Sie dies noch nicht getan haben, ändern Sie den Bereich in **Sales Insights-Einstellungen.**
2.  Wählen Sie in der Gruppe Sales Insights die Option **Globale Einstellungen.**
3.  Wählen Sie in der Untergruppe „Vertriebsbeschleunigung“ die Registerkarte **Sequenzen** aus.
4.  Falls erforderlich, wählen Sie **Aktivieren** in der Benachrichtigung, um den Workflow zu aktivieren, damit die Sequenzen richtig funktionieren.
5.  Wählen Sie auf der Registerkarte Sequenzen **+ Neue Sequenz.**
6.  Sie haben die Möglichkeit, eine Sequenz aus einer Reihe gängiger Vorlagen zu erstellen. Sie können die verfügbaren Vorlagen erkunden. Wenn Sie bereit sind, wählen Sie **ohne Vorlage starten.**
7.  Als Nächstes vergeben Sie einen Namen, eine Beschreibung und wählen die Art der Tabelle, für die die Sequenz verfügbar sein soll. Geben Sie in das Textfeld Name der Sequenz den Namen der Sequenz ein: *Trade Show Nachverfolgungssequenz.*
8.  Geben Sie in das Textfeld Beschreibung eine Sequenzbeschreibung ein: „Dies ist eine Testsequenz für Testkaffee. Diese Sequenz wird für die Nachverfolgung potenzieller Kunden nach Messen verwendet.“
9.  Wählen Sie unter „Datensatztyp“ die Option **Lead** aus (wenn sie nicht bereits ausgewählt ist).
10. Klicken Sie auf **Weiter**.

### Aufgabe 2: Wählen Sie die erste Aktivität, die die Verkaufsperson durchführen soll

Wählen Sie den ersten Schritt für Ihre Verkaufsperson aus. Dies kann entweder das Senden einer E-Mail, ein Telefonanruf oder das Hinzufügen einer eigenen Aufgabe sein. In unserem Beispiel beginnen wir mit einer E-Mail.

1.  Wählen Sie unter der Startkachel der Sequenz die Schaltfläche **+**, um eine Aktion oder ein anderes Element hinzuzufügen.
2.  Klicken Sie auf **E-Mail senden.**
3.  Geben Sie als Titel ein: *Einführungs-E-Mail.*
4.  Geben Sie bei Beschreibung optional eine Beschreibung ein: *Einführung des Leads in das Verkaufsteam.*
5.  Wenn in Ihrer Organisation E-Mail-Vorlagen (tabellenspezifische oder globale Vorlagen) verfügbar sind, können Sie eine E-Mail-Vorlage auswählen. In diesem Fall gehen wir davon aus, dass die Verkaufsperson eine eigene Einführungs-E-Mail schreibt.
6.  Wählen Sie die Schaltfläche **X** aus, um den Aktivitätsbereich zu verlassen.
7.  Wählen Sie in der Befehlsleiste für die Sequenz **Speichern.**

### Aufgabe 3: Fügen Sie zusätzliche Aktivitäten für Ihre Verkaufsperson hinzu

Fügen Sie zusätzliche Aktivitäten hinzu, die Ihre Verkaufspersonenin geordneter Weise durchführen müssen - zum Beispiel muss die Verkaufsperson die erste Aktivität zuerst durchführen, dann die zweite und dritte und so weiter.

1.  Klicken Sie auf die Schaltfläche **+**.
2.  Wählen Sie die nächste Aktivität aus, die die Verkaufsperson durchführen soll. Sie können entweder eine E-Mail senden, einen Anruf tätigen oder eine eigene Aufgabe hinzufügen. Wählen Sie **Wartezeit einstellen**, um ein Zeitintervall zwischen den Aktivitäten festzulegen. In unserem Beispiel werden wir ein Zeitintervall von 1 Stunde hinzufügen.
3.  Klicken Sie auf Speichern.
4.  Klicken Sie auf die Schaltfläche **+**.
5.  Wählen Sie **Telefonanruf.**
6.  Geben Sie in den Titel *Nachverfolgungsanruf* ein (Wenn Sie möchten, können Sie eine Beschreibung hinzufügen.)
7.  Wählen Sie in der Befehlsleiste **Speichern** aus.

### Aufgabe 4: Aktivieren Sie die Sequenz

Um die Sequenz für Verkaufspersonen verfügbar zu machen, aktivieren Sie die Sequenz.

1.  Wählen Sie **Aktivieren** in der Befehlsleiste.
2.  Wählen Sie **Ich verstehe** und dann **Aktivieren** in dem Pop-up-Fenster.
3.  Ihre Sequenz enthält nun oben eine grüne Leiste, die Ihnen mitteilt, dass die Sequenz erfolgreich aktiviert wurde.

### Aufgabe 5: Verbinden Sie die Sequenz mit einem Segment

1.  Vergewissern Sie sich, dass Sie sich im Bereich **Sales Insights-Einstellungen** befinden.
2.  Wählen Sie über die Navigation auf der linken Seite **Sequenzen**.
3.  Öffnen Sie die Sequenz**Trade Show Nachverfolgung**, die Sie zuvor erstellt haben.
4.  Wählen Sie die Registerkarte **Verbundene Leads** aus.
5.  Wählen Sie **+ Segmente verbinden**
6.  Suchen Sie das Segment **Trade Show Leads**, das Sie zuvor erstellt haben, und wählen Sie es aus.
7.  Wählen Sie **Verbinden**.

### Aufgabe 6: Verbinden Sie die Sequenz mit dem Datensatz (vom Datensatz)

1.  Ändern Sie den Bereich in den Bereich **Vertrieb**, indem Sie das Dropdown-Menü unten links verwenden.
2.  Wählen Sie **Leads** aus dem Sitenavigations-Menü.
3.  Wählen Sie einen der zuvor erstellten Leads aus.
4.  Wählen Sie in der Befehlsleiste den **Pfeil nach unten** neben Sequenzen. Wählen Sie im angezeigten Menü **Sequenz verbinden** aus der Befehlsleiste.
5.  Wählen Sie die zuvor erstellte Sequenz und wählen Sie **Verbinden.**
6.  Unten auf der Seite wird eine Bestätigungsmeldung angezeigt, und die Sequenz wird mit dem ausgewählten Lead-Datensatz verbunden.
7.  Wenn Sie aufgefordert werden, eine Verkaufsperson zuzuweisen, wählen Sie die Schaltfläche **Zuweisen**. Jetzt können die Verkaufspersonen, die Zugriff auf den Lead-Datensatz haben, die damit verbundenen Aktivitäten sehen.
8.  Aktualisieren Sie die Seite - Sie sollten die von Ihnen erstellten Aufgaben im Abschnitt **Nächste Aufgabe** sehen.

