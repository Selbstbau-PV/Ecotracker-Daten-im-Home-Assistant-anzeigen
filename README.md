# Everhome-Ecotracker-Daten-im-Home-Assistant-anzeigen
Ein yaml Code von https://selbstbau-pv.de/ , der den aktuellen Verbrauch, die Einspeisung und den Bezug des Everhome Ecotrackers im Home Assistant anzeigt.

# Vorraussetzungen:
- Lokaler HTTP-Server im Everhome Ecotracker aktiviert (Siehe hier: [Everhome Ecotracker einrichten](https://selbstbau-pv.de/wiki/everhome-ecotracker-einrichten-smart-micro-solar/))
- Ein Addon wie z.B. File Editor im Home Assistant, damit man auf Dateien zugreifen kann

# Durchführung:
1. Über den File Editor in die configuration.yaml navigieren
   
2. [Hier klicken](http://selbstbau-pv.de/wp-content/uploads/2024/12/Ecotracker-Code.txt), alles davon kopieren und in die configuration.yaml einfügen
   
3. Im Code steht „resource: http://[IP]/v1/json“. Da wo [IP] steht,  muss die IP deines Ecotrackers drinstehen (ohne die eckigen Klammern). Da würde dann z.B. „resource: http://192.168.4.23/v1/json“ stehen
   
4. Home Assistant neustarten
   
5. Es sollten nun neue Entitäten aufgetaucht sein, die den Hausverbrauch, den Bezug und die Einspeisung anzeigen. Diese kannst du nun deinem Dashboard hinzufügen

![image](https://github.com/user-attachments/assets/2ef17906-0538-43e1-8889-02e9f2f4d398)
