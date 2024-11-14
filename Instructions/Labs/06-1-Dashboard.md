---
lab:
  title: 'Lab 6.1: Ein Dashboard konfigurieren'
---

# Modul 6: Analysieren von Dynamics 365 Vertriebsdaten

## Übungslab 6.1: Ein Dashboard konfigurieren

### Szenario
Die Vertriebsleitenden von Contoso Coffee möchten den Erfolg ihres Vertriebsteams besser überwachen, insbesondere im Hinblick auf geschlossene Verkaufschancen Das Vertriebsmanagement hat sich ein persönliches Dashboard gewünscht, das ihm einen Überblick über die kürzlich abgeschlossenen Verkaufschancen und die diesbezüglichen Aktionen seiner Verkaufspersonen gibt. Außerdem möchten sie, dass dieses Dashboard als Standard-Dashboard verwendet wird, wenn sie den Bereich Dashboards in der Anwendung öffnen.

Nach erfolgreichem Abschluss dieses Labs werden Sie in der Lage sein:
- Erstellen persönlicher Dashboards
- Hinzufügen von Komponenten zu Dashboards

## Übung 1 - Ein Dashboard konfigurieren 
### Aufgabe 1 - Erstellen eines Dashboards
1. Vergewissern Sie sich, dass Sie sich im Verkaufsbereich der Anwendung befinden, falls Sie das noch nicht tun. Verwenden Sie das Dropdown-Menü unten links, um den Bereich in **Vertrieb** zu ändern, wenn Sie wechseln müssen.
2. Wählen Sie in der Gruppe Meine Arbeit die Option **Dashboards** aus dem linken Navigationsmenü.
3. Standardmäßig wird das Social Dashboard Vertriebsaktivität angezeigt. Schauen Sie sich die verschiedenen Komponenten ruhig an. Zusätzlich können Sie das Dropdown-Symbol <bpt ctype="x-unknown" id="1" rid="1"><bpt xmlns="urn:oasis:names:tc:xliff:document:1. 2" id="p1">**</bpt></bpt>˅<ept id="2" rid="1"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</ept></ept> neben dem Titel des Dashboards nutzen, um die anderen System-Dashboards zu erkunden.
4. Wenn Sie bereit sind, Ihr eigenes Dashboard zu erstellen, wählen Sie **+ Neu** und dann **Dynamics 365 Dashboard.**
5. Erkunden Sie die verschiedenen Dashboardlayouts. In dieser Aufgabe werden wir ein zweispaltiges reguläres Dashboard erstellen. Wenn Sie bereit sind, wählen Sie es aus der Liste aus und wählen Sie **Erstellen.**

### Aufgabe 2 - Komponenten hinzufügen
1. Der Dashboard-Designer wird in einem neuen Fenster geöffnet. (Wenn Ihr neues Dashboard nicht in einem neuen Fenster geöffnet wird, stellen Sie sicher, dass der Popup-Blocker deaktiviert ist). Es kann eine Minute dauern, bis der Designer geladen ist.
2. Geben Sie in das Textfeld „Name“ *Vertriebsmanager-Dashboard* ein.
3. Fügen wir nun eine Komponente zum oberen linken Abschnitt hinzu. Das Vertriebsmanagement wünscht sich eine einfache Möglichkeit, um die Höhe der gewonnenen und verlorenen Einnahmen aus Verkaufschancen zu ermitteln. Diese Informationen werden in einer grafischen Ansicht angezeigt. Zu diesem Zweck fügen wir ein Chart hinzu, indem wir das Symbol **Chart einfügen** in der Mitte des oberen linken Bereichs auswählen.
4. Wählen Sie die folgenden Details für Ihr Chart aus:
   - Datensatztyp: Verkaufschance
   - Ansicht: Geschlossene Verkaufschancen
   - Chart: Erfolg vs. Misserfolg von Abschlüssen
   - Wählen Sie **Hinzufügen**.
5. Ihr Chart wird im oberen linken Bereich angezeigt.
6. Als Nächstes fügen wir eine Komponente zum oberen rechten Abschnitt hinzu. Das Vertriebsmanagement wünscht sich eine einfache Möglichkeit, die kürzlich geschlossenen Verkaufschancen einzusehen, damit sie sich mit den Verkaufspersonen über die gewonnenen Erkenntnisse austauschen können. Sie möchten, dass die Ansicht sowohl gewonnene als auch verlorene Verkaufschancen enthält, aber nur Verkaufschancen, die im laufenden Geschäftsjahr abgeschlossen wurden. Wählen Sie das Symbol **Liste einfügen** für den oberen rechten Bereich.
7. Wählen Sie die folgenden Details für Ihre Liste aus:
   - Datensatztyp: Verkaufschancen
   - Ansicht: Geschlossene Verkaufschancen im laufenden Geschäftsjahr
   - Klicken Sie auf **Hinzufügen**.

### Aufgabe 3 - Speichern und Bearbeiten des Dashboards
1. Wählen Sie **Speichern** und dann **Schließen**. Das Fenster wird geschlossen und Sie kehren zum Formular Dashboards zurück, wo Ihr neues Dashboard angezeigt wird.
2. Wählen Sie **Als Standard festlegen** in der Befehlsleiste. Dieses Dashboard wird nun Ihr Standard-Dashboard sein, wenn Sie zum Abschnitt Dashboards navigieren.
3. Klicken Sie im oberen Menü auf **Bearbeiten**. Sie kehren in einem anderen neuen Fenster zum Dashboard-Designer zurück. Fügen Sie zwei weitere Komponenten unterhalb Ihres Charts hinzu. Die von Ihnen ausgewählten Komponenten sollten die folgenden vom Vertriebsmanagement geforderten Geschäftsanforderungen erfüllen:
   - Das Vertriebsmanagement möchte ein Gefühl dafür bekommen, wie die einzelnen Verkaufspersonen auf der Grundlage des Umsatzerlöses ihrer geschlossenen Verkaufschancen abschneiden. Sie möchten ein Chart, das die Namen der Verkaufspersonen und ihren Gesamt-Umsatzerlös aus geschlossenen Verkaufschancen zeigt.
   - Das Vertriebsmanagement möchte die täglichen Aufgaben der Verkaufspersonen in ihrem Team überwachen. Sie möchten eine Liste anzeigen, in der die Aktivitäten ihrer Vertriebsteams angezeigt werden.
