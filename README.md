# Projektbeschreibung
 Diese Anwendung basiert auf dem Spring-Framework und verwendet eine PostgreSQL-Datenbank, um alle wichtigen Informationen zu speichern. 
 Mit dieser App können Benutzer ihre persönlichen Aufgaben verwalten, indem sie Todos hinzufügen, ändern und löschen. Das Hauptziel des Projekts besteht darin, die Konzepte und Prinzipien verteilter Systeme zu demonstrieren.
 
 # Starten der Anwendung 
 Um das Projekt lokal ausführen zu können, muss lediglich Docker installiert sein. Mit dem Befehl docker compose up wird die Anwendung mithilfe der docker-compose Datei automatisch gestartet. Das Image für die Anwendung, sowie die Datenbank 
 werden von dem Docker Hub gedownloadet. 
 Die Web-App kann über den Browser mit der URL localhost:8080 geöffnet werden. 
 
 # Erweiterungsmöglichkeiten
 Das Frontend und Backend laufen aktuell im gleichen Container. In einem nächsten Schritt könnten Frontend und Backend getrennt werden, und für jeden Part ein seperates Image erstellt werden. Damit sie als getrennte Container laufen können.
 Außerdem müsste das Mapping der REST API nochmals überarbeitet werden. Es wurden noch nicht alle Methoden richtig angewendet. Als Beispiel hierfür müsste der API Endpunkt /delete/{id} mit der Methode GET in /todo/{id} umbenannt werden 
 und spezifiziert werden dass es sich dabei um die Methode DELETE handelt.
 
