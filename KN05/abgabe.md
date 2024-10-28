# a
```
#cloud-config
users:   # Erstellt eine Liste von Benutzerkonfigurationen
  - name: ubuntu   # benutzername
    sudo: ALL=(ALL) NOPASSWD:ALL   # sudo regeln für diesen nutzer - erlaubt dem nutzer alle befehle über sudo ohne passwort auszuführen
    groups: users, admin   # listet alle grupen auf zu denen der benutzer gehört
    home: /home/ubuntu   # definiert das home verzeichnis für diesen benutzer
    shell: /bin/bash   # Gibt die Standard-Shell für den Benutzer an
    ssh_authorized_keys:   # listet die shh keys auf, welche für autenifizierung für diesen nutzer verwendet können
      - ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQC0WGP1EZykEtv5YGC9nMiPFW3U3DmZNzKFO5nEu6uozEHh4jLZzPNHSrfFTuQ2GnRDSt+XbOtTLdcj26+iPNiFoFha42aCIzYjt6V8Z+SQ9pzF4jPPzxwXfDdkEWylgoNnZ+4MG1lNFqa8aO7F62tX0Yj5khjC0Bs7Mb2cHLx1XZaxJV6qSaulDuBbLYe8QUZXkMc7wmob3PM0kflfolR3LE7LResIHWa4j4FL6r5cQmFlDU2BDPpKMFMGUfRSFiUtaWBNXFOWHQBC2+uKmuMPYP4vJC9sBgqMvPN/X2KyemqdMvdKXnCfrzadHuSSJYEzD64Cve5Zl9yVvY4AqyBD aws-key       
^ # shh key der erlaubt is
ssh_pwauth: false   # Deaktiviert die Authentifizierung mit einem Passwort bei der SSH-Anmeldung
disable_root: false   # Lässt den root-Benutzer aktiviert, sonst wäre der Root-Zugang deaktiviert
package_update: true   # Erzwingt eine Aktualisierung des Paketmanagers bei der Initialisierung
packages:  # Installiert eine Liste von Paketen
  - curl   # Ein Werkzeug zur Übertragung von Daten
  - wget   # Ein Tool welches zum Herunterladen von Dateien verwendet wird

```

# b
Ein Screenshot der Details der Instanz. Scrollen Sie so weit runter, dass das Feld "Key pair 
assigned at launch", sichtbar ist.
![image](/KN05/fotos/screenshotDerInstanzB.png)

Screenshot mit dem ssh-Befehl und des Resultats unter Verwendung des ersten Schlüssels.
![image](/KN05/fotos/loginKey1.png)

Screenshot mit dem ssh-Befehl und des Resultats unter Verwendung des zweiten Schlüssels.
![image](/KN05/fotos/loginKey2.png) 

Screenshot mit dem Auszug aus dem Cloud-Init-Log. Der Befehl den Sie aufgerufen haben 
und der obere Teil des Logs sollten sichtbar sein.
![image](/KN05/fotos/CloudInitLog.png)

# c

# d

![image](/KN05/fotos/indexhtml.png)
![image](/KN05/fotos/infophp.png)
![image](/KN05/fotos/dbphp.png)
![image](/KN05/fotos/adminer.png)
