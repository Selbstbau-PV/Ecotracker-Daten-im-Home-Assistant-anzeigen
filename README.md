# Ecotracker-Daten-im-Home-Assistant-anzeigen
Ein yaml Code, der den aktuellen Verbrauch, die Einspeisung und den Bezug des Ecotrackers im Home Assistant anzeigt.

# Vorraussetzungen:
- Lokaler HTTP-Server im Ecotracker aktiviert (Siehe hier: [Everhome Ecotracker einrichten](https://selbstbau-pv.de/wiki/everhome-ecotracker-einrichten-smart-micro-solar/))
- Ein Addon wie z.B. File Editor im Home Assistant

# Durchführung:
1. Über den File Editor in die configuration.yaml navigieren
   
2. [Hier klicken](https://selbstbau-pv.de/wp-content/uploads/2024/08/Ecotracker-Code.txt), alles davon kopieren und in die configuration.yaml einfügen
   
3. Im Code steht „resource: http://[IP]/v1/json“. Da wo [IP] steht, muss die IP deines Ecotrackers drinstehen (ohne die eckigen Klammern). Da würde dann z.B. „resource: http://192.168.4.23/v1/json“ stehen
   
4. Home Assistant neustarten
   
5. Es sollten nun neue Entitäten aufgetaucht sein, die den Hausverbrauch, den Bezug und die Einspeisung anzeigen. Diese kannst du nun deinem Dashboard hinzufügen
