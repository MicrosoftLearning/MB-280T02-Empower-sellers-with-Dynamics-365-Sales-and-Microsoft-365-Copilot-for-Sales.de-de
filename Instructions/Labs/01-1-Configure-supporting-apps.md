---
lab:
  title: 'Lab 1.1: Konfigurieren von unterstützenden Anwendungen'
---

# Modul 1: Konfigurieren von Dynamics 365 Sales

## Übungs-Lab 1.1: Konfigurieren von unterstützenden Anwendungen

## Szenario

Die Verkaufsmitarbeitenden von Contoso Coffee berichten, dass Dynamics 365 Sales zwar sehr hilfreich ist, um die Produktivität der Verkaufsmitarbeitenden zu steigern, dass sich die Anwendung in Bezug auf ihren täglichen Arbeitsablauf sehr isoliert anfühlt. Sie haben die folgenden Anforderungen an ihre IT-Abteilung:

-   Die Verkaufsmitarbeitenden möchten vertriebsbezogene E-Mail-Korrespondenz in CRM nachverfolgen und verwalten.
-   Die Verkaufsmitarbeitenden möchten Dokumente, die mit Verkäufen in Zusammenhang stehen (wie Artikel zu Produktwissen, Kundenforschung und Markttrendberichte), im CRM speichern. Sie möchten direkt über die Vertriebs-App auf diese Dokumente zugreifen, sie freigeben und verwalten können.
-   Die Verkaufsmitarbeitenden möchten bei der Verfolgung ihrer Verkaufschancen gerne mit anderen Abteilungen wie Lagerverwaltung, Auftragsabwicklung und Marketing zusammenarbeiten. Sie möchten, dass diese anderen Abteilungen in einem Teams-Chat oder -Kanal an einem Kundendatensatz zusammenarbeiten können.
-   Die Verkaufsmitarbeitenden haben viel über die Copilot-Features in Dynamics 365 Sales gehört, darunter das Zusammenfassen von Datensätzen, das Nachverfolgen von Änderungen an Datensätzen, das Vorbereiten von Besprechungen und das Verfassen von Korrespondenz. Sie möchten sicherstellen, dass Copilot-Features in ihrer Umgebung aktiviert sind, damit sie mit der Nutzung von KI innerhalb der App beginnen können, um ihre Produktivität zu verbessern.

In dieser Übung aktivieren und konfigurieren wir die Features, die unserer CRM-Organisation helfen, die Anforderungen dieser Verkaufsmitarbeitenden zu erfüllen.

## Übung 1: Konfigurieren der E-Mail-, SharePoint- und OneDrive-Integration

### Aufgabe 1: Konfigurieren der E-Mail-Integration

1.  Navigieren Sie in einem Webbrowser zu [admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com/).
2.  Wählen Sie auf der linken Seite des Bildschirms in der Sitenavigation die Option **Umgebungen** aus.
3.  Wählen Sie die Umgebung **Vertriebstestversion** aus, um sie zu öffnen.
4.  Suchen und wählen Sie **Einstellungen** aus den oben aufgeführten Befehlen aus.
5.  Wählen Sie die E-Mail-Überschrift aus, um sie zu erweitern, und wählen Sie die Option **Postfächer** aus.
6.  Öffnen Sie den Postfachdatensatz für **MOD-Administrator**.
7.  Konfigurieren Sie das **MOD-Administratorpostfach** wie folgt:
    -   **Serverprofil**: Microsoft Exchange Online
    -   **Eingehende E-Mail**: Serverseitige Synchronisierung oder E-Mail-Router
    -   **Ausgehende E-Mail**: Serverseitige Synchronisierung oder E-Mail-Router
    -   **Termine, Kontakte und Aufgaben**: serverseitige Synchronisierung
8.  **Speichern** Sie die Änderungen. Klicken Sie dann auf **E-Mail genehmigen**. (**Hinweis:** Sie müssen das Postfach genehmigen, bevor Sie E-Mails senden und empfangen können).
9.  Sie werden gefragt, ob Sie die primäre E-Mail genehmigen möchten. Wählen Sie **OK** aus.
10. Klicken Sie auf **Postfach testen und aktivieren**
11. Vergewissern Sie sich auf dem Pop-up-Bildschirm „Testen und Aktivieren“, dass dieses Postfach, wenn es zuvor für die Synchronisierung mit einer anderen Organisation konfiguriert wurde, durch Aktivieren dieser Option zur Synchronisierung mit dieser Organisation wechselt.
12. Wählen Sie **OK** aus.

**WICHTIG:** Navigieren Sie nicht von dieser Seite weg, während die Tests abgeschlossen werden. Wenn Sie an Aufgabe 2 arbeiten möchten, während die Tests abgeschlossen werden, können Sie eine neue Registerkarte oder einen neuen Browser öffnen.

## Aufgabe 2: Aktivieren der serverbasierten SharePoint-Integration

In dieser Aufgabe aktivieren Sie die serverbasierte SharePoint-Integration für Ihre Dynamics 365 Organisation.

1.  Navigieren Sie in einem Webbrowser zu [admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com/).
2.  Wählen Sie auf der linken Seite des Bildschirms in der Sitenavigation die Option **Umgebungen** aus.
3.  Öffnen Sie die Umgebung **Vertriebstestversion**, in der Sie gearbeitet haben, um sie zu öffnen.
4.  Suchen und wählen Sie **Einstellungen** aus den oben aufgeführten Befehlen aus.
5.  Wählen Sie unter der Überschrift „Integration“ **Einstellungen für die Dokumentverwaltung** aus.
6.  Es sollte eine Option zum **Aktivieren der serverbasierten SharePoint-Integration** angezeigt werden. (Wenn sie nicht angezeigt wird, wurde die SharePoint-Integration bereits aktiviert, und Sie können mit Schritt 11 fortfahren).
    -   Wenn die SharePoint-Integration nicht konfiguriert ist, wählen Sie **Serverbasierte SharePoint-Integration aktivieren** aus.
7.  Klicken Sie in der Anzeige „Serverbasierte SharePoint-Integration aktivieren“ auf die Schaltfläche **Weiter**.
8.  Wählen Sie **Online** für den Bereitstellungstyp aus, und klicken Sie auf die Schaltfläche **Weiter**.
9.  Geben Sie die URL der SharePoint-Seite ein, die Sie verwenden möchten. (Beispiel: https://"Orgname".sharepoint.com), klicken Sie auf die Schaltfläche **Weiter**.

    **Hinweis:***Sie können Ihre SharePoint-URL finden, indem Sie in der oberen linken Ecke des Bildschirms das App-Überprüfung-Symbol auswählen. (Sieht wie ein 3 x 3 Quadrat aus). Halten Sie die STRG-TASTE gedrückt, und wählen Sie SharePoint aus.*

10. Nachdem die Website überprüft wurde, klicken Sie auf die Schaltfläche **Aktivieren**.
11. Klicken Sie auf **Dokumentverwaltungseinstellungen**.
12. Wählen Sie alle Entitäten aus, für die die Dokumentverwaltung aktiviert werden soll, z. B. Leads, Konten, Verkaufschancen, und klicken Sie auf **Weiter**.
    -   **WICHTIG**: Wenn Sie planen, E-Mail-Engagement in Sales Insights zu konfigurieren, wählen Sie die E-Mail-Entität aus.
13. Geben Sie im Feld „URL der SharePoint-Website“ die URL der SharePoint-Website ein, die Sie in der vorherigen Aufgabe verwendet haben.
14. Klicken Sie auf die Schaltfläche **Weiter**.
15. Klicken Sie auf die Schaltfläche **Fertig stellen**, um die Einrichtung abzuschließen.

### Aufgabe 3: Einrichten von OneDrive for Business Integration

In dieser Aufgabe richten Sie die OneDrive Integration für Ihre Dynamics CRM-Organisation ein. (Zum Zeitpunkt der Veröffentlichung dieses Kurses waren die Dokumentverwaltungseinstellungen nicht im Power Platform Admin Center verfügbar. Sie müssen die OneDrive for Business-Integration über den klassischen Bereich „Dynamics 365 Einstellungen“ konfigurieren.)

1.  Navigieren Sie in einem Webbrowser zu [admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com/).
2.  Wählen Sie auf der linken Seite des Bildschirms in der Sitenavigation die Option **Umgebungen** aus.
3.  Öffnen Sie die Umgebung **Vertriebstestversion**, in der Sie gearbeitet haben, um sie zu öffnen.
4.  Suchen und wählen Sie **Einstellungen** aus den oben aufgeführten Befehlen aus.
5.  Wählen Sie unter der Überschrift „Integration“ **Einstellungen für die Dokumentverwaltung** aus.
6.  Klicken Sie auf das Symbol **OneDrive for Business aktivieren**.
7.  Wählen Sie das Kontrollkästchen **OneDrive for Business aktivieren** aus und klicken Sie dann auf **OK**.
8.  Klicken Sie nach dem Aktualisieren des Bildschirms auf die **OneDrive for Business-Ordnereinstellungen**.
9.  Akzeptieren Sie den Standardordnernamen, oder geben Sie einen Namen Ihrer Wahl ein, und wählen Sie dann **OK** aus.

## Übung 2: Konfigurieren von Teams und Copilot

### Aufgabe 1: Konfigurieren der Teams-Integration

1.  Öffnen Sie bei Bedarf die Sales Hub-App.
2.  Wählen Sie in der Navigation links den Bereich **Vertrieb** aus (unten links).
3.  Wählen Sie im angezeigten Menü **App-Einstellungen** aus.
4.  Wählen Sie in der Gruppe „Allgemeine Einstellungen“ die Option **Chat und Zusammenarbeit**.
5.  Setzen Sie **Verknüpfung von Dynamics 365-Datensätzen mit Microsoft Teams-Kanälen aktivieren** auf **Ja**.
6.  Setzen Sie **Erweiterte Microsoft Teams Integration aktivieren** auf **Ja**. (Möglicherweise müssen Sie Ihr MOD-Administratorkonto auswählen. Wenn Sie nach Berechtigungen gefragt werden, wählen Sie **Annehmen** aus).
7.  Wählen Sie unter **Microsoft Teams-Chats in Dynamics 365 aktivieren** die Option **Für alle Dynamics 365 Apps aktivieren** aus.
8.  Wählen Sie die Schaltfläche **Speichern** aus.  
    **WICHTIG**: Es kann mehrere Minuten dauern, bis die Änderungen gespeichert werden.

### Aufgabe 2: Konfigurieren von Copilot

1.  Stellen Sie sicher, dass Sie sich im Bereich **App-Einstellungen** befinden.
2.  In der Gruppe „Allgemeine Einstellungen“ wählen Sie **Copilot**.
3.  Wählen Sie das Kontrollkästchen neben **Testen Sie unseren neuesten Vorschaufeatures, bevor sie für alle verfügbar werden**, um es zu aktivieren.
4.  Ändern Sie unter **Copilot-Features** wie folgt die Option **Alle Dynamics 365 Sales-Apps** :
    -   **Chat**: Ein
    -   **E-Mail (Vorschau):** Ein
5.  Wählen Sie die Schaltfläche **Speichern** aus.

