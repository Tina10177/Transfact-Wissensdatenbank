# Fertigungsübersicht
### 📊 Modulübersicht

Die **Fertigungsübersicht** im Transfact PPS-Modul bietet eine zentrale Echtzeitansicht aller Fertigungsbereiche (Produktionsbereiche) und deren Ressourcen (Arbeitsplätze). Sie dient der Visualisierung des Fertigungsfortschritts, der Aufgabenverteilung sowie der Ressourcenverfügbarkeit und Priorisierung.

Zugriffspfad: **PPS > Fertigungsübersicht**

## 🔍 Feldbeschreibung

Jeder Fertigungsbereich (FB) enthält mehrere Ressourcen (Arbeitsplätze). Jede Ressource zeigt folgendes Format: L: x / P: y / z h

| Feld | Bedeutung                                                                          |
| ---- | ---------------------------------------------------------------------------------- |
| `L`  | Anzahl der aktuell auf dieser Ressource **zu bearbeitenden Fertigungslosen (Los)** |
| `P`  | Anzahl der **priorisierten Lose** unter den offenen Losen                          |
| `h`  | Geplante Gesamtbearbeitungszeit dieser Lose auf der Ressource (in Stunden)         |

**Beispiel:** L: 4 / P: 2 / 1h → 4 offene Lose auf dieser Ressource, davon 2 mit hoher Priorität, geplante Bearbeitungszeit 1 Stunde.

---

## 🚪 Navigationspfade


### ▶ 1. Anzeige der Abarbeitungsliste eines Fertigungsbereichs

Durch Klicken auf den **Namen eines Fertigungsbereichs** (z. B. `TF15-01 Montage`) 

![PPS_Fertigungsübersicht_Von Fertigungsübersicht zu Abarbeitungsliste des FBs](./images/PPS_Fertigungsübersicht_Von Fertigungsübersicht zu Abarbeitungsliste des FBs.png)
gelangt man zur **Abarbeitungsliste** dieses Bereichs:
![[PPS_Fertigungsübersicht_Abarbeitungsliste des FBs..png]]
- Anzeige aller Los-Aufträge in diesem Bereich;
    
- Filtermöglichkeiten nach Losnummer, FA-Nummer, Artikel, Projekt usw.;
    
- Tabellarische Darstellung aller Auftragsdaten wie Schritt, Status, Anweisung etc.
    

### ▶ 2. Anzeige der Abarbeitungsliste einer Ressource

Durch Klicken auf eine bestimmte **Ressourcennummer** (z. B. `1WP1`) 
![[PPS_Fertigungsübersicht_Von Fertigungsübersicht zu Abarbeitungsliste einer Ressource.png]]gelangt man zur **Abarbeitungsliste dieser Ressourcen (Arbeitsplatz)**;
![[PPS_Fertigungsübersicht_Abarbeitungsliste der Ressource.png]]
- Anzeige aller Lose, die dieser Ressource zugeordnet sind.

### ▶ 3. Detailansicht eines einzelnen Loses

Ist ein Los aktuell auf einer Ressource angemeldet (Bearbeitung aktiv), wird es in der Liste **fett markiert**.
![[PPS_Fertigungsübersicht_an Ressource angemeldete Los.png]]Durch Klicken auf die **Losnummer** (z. B. 460341) öffnet sich die:
![[PPS_Fertigungsübersicht_Losdetailansicht.png]]
- **Detailansicht des Fertigungsloses** mit:
    
    - Grunddaten (Artikel, Auftrag, Kunde, Projekt);
        
    - Bearbeitungsstatus, Verzugstage;
        
    - Arbeitsschritte, Ressourcenzuweisung, Qualitätsstatus usw.
        

---

## 🛠 Verwaltung des Ressourcenstatus

Durch Klicken auf das **Zahnrad-Symbol** neben einer Ressource öffnet sich die:
![[PPS_Fertigungsübersicht_Ressourcen Status einzustellen.png]]
 **Ressourcen-Status-Seite**;
![[PPS_Fertigungsübersicht_Ressource Status Pop Fenster.png]]
- Möglichkeit, den Status zu ändern (z. B. `Reparatur`);
    
- Eingabe von voraussichtlicher Dauer und Bemerkung;
    
- Nach Klick auf **Speichern** wird der neue Status (z. B. rot markiert) in der Fertigungsübersicht angezeigt.

![[PPS_Fertigungsübersicht_Ressource Status geändert.png]]
## 🛠️ Layoutanpassung der Fertigungsübersicht

### Zugang: Button **Fertigungsübersicht verändern** (oben rechts)
![[PPS_Fertigungsübersicht_Fertigungsübersicht verändern.png]]
Im Bearbeitungsmodus:
![[PPS_Fertigungsübersicht_Fertigungsübersicht Einstellungen.png]]
- Auswahl der Spaltenanzahl: `1-spaltig` bis `8-spaltig`
    Spaltenanzahl: Bildschirmabhängige Empfehlung
    **3–4 Spalten** für schmale Bildschirme (z. B. Laptops)
    **6–8 Spalten** für breite Bildschirme (z. B. große Monitore)
    
- Jeder FB zeigt 3 Symbole:
    
    - ⬆️ nach oben verschieben
        
    - ⬇️ nach unten verschieben
        
    - ☑️ sichtbar / unsichtbar schalten
        

### Sichtbarkeit

- Wird der Sichtbarkeits-Haken deaktiviert, verschwindet der FB aus der Ansicht
    
- Reaktivierung durch erneutes Anhaken

### Sortierung

- Per ⬆️ / ⬇️ Symbole die Reihenfolge der Bereiche anpassen

![[PPS_Fertigungsübersicht_Fertigungsübersicht anzeigen.png]]
- **Wichtig**: Anschließend **Fertigungsübersicht anzeigen** klicken, um neue Anordnung zu übernehmen
## 🔄 Zusammenfassung der Schritte

```
Fertigungsübersicht
│
├─▶ Fertigungsbereich klicken → Abarbeitungsliste des FBs
│
├─▶ Ressource klicken → Abarbeitungsliste der Ressource
│
├─▶ Los klicken → Losdetailansicht
│
├─▶ Zahnrad klicken → Ressourcenstatus setzen (z. B. Reparatur)
│
└─▶ "Fertigungsübersicht verändern" klicken
    ├─▶ Spaltenanzahl, Reihenfolge und Sichtbarkeit anpassen
    └─▶ "Fertigungsübersicht anzeigen" klicken zur Übernahme
```

---

Diese Anleitung unterstützt Sie bei der effektiven Nutzung der Fertigungsübersicht zur Produktionsplanung, Ressourcensteuerung und Auftragsverfolgung im Transfact PPS-System.