# Hartmann Dominik - LB 324

## Starten der Applikation
Um die Applikation zu starten, müssen folgenden Befehle eingegeben werden.
1. `pip install -r requirements.txt`
2. `flask run`

## Aufgabe 2
Erklären Sie hier, wie man `pre-commit` installiert.

1. Zuerst wird im Terminal `pre-commit install` eingegeben, um es zu installieren
2. File namens '.pre-commit-config.yaml' erstellen
  3. in diesem File muss auf Pytest verwiesen werden
4. Um es auf Push zu testen, muss `pre-commit install --hook-type pre-commit --hook-type pre-push` installiert werden.
5. Im File '.pre-commit-config.yaml' muss für den 'pytest-check' 'stages: [push]' stehen, um den Test bei push auszuführen.
6. Um das Programm, die Tests auszuführen, muss `git add .`, `git commit -m "Mitteilung"` und `git push origin precommit` eingegeben werden.

## Aufgabe 4
Erklären Sie hier, wie Sie das Passwort aus Ihrer lokalen `.env` auf Azure übertragen.

1. Einloggen in Azure: https://portal.azure.com/
2. Eine neue Web-App erstellen unter 'Ressource erstellen'
![image](https://github.com/ooDominikoo/HartmannDominikLB-324/assets/104886373/12d3fbd7-fdcf-495e-9f47-9214e21cba0f)
3. Danach unter 'Bereitstellungscenter' oder 'Deployment center'
  4. Quelle GitHub angeben und mein Benutzernamen, mein Repository und den main Branch eingeben.
![image](https://github.com/ooDominikoo/HartmannDominikLB-324/assets/104886373/b7556d19-a0b1-4e5c-979b-f45f83210318)
5. Wechseln Sie auf das Projekt auf Github.
6. Unter 'Actions' sind die verschiedenen Actions ersichtlich.
  7. Unter 'Add or update the Azure App Service build and deployment workflow config' ist der URL für die Azure ersichtlich, dass das Projekt mit Azure ausgeführt werden kann.
![image](https://github.com/ooDominikoo/HartmannDominikLB-324/assets/104886373/a1daaa9f-fc91-47f0-9b64-4ecb0840896d)

8. Um das neue Password zu erstellen und auf Azure zu übertragen, muss in Azure auf Konfiguration geklickt werden.
9. Es muss auf 'neue Anwendungseinstellung' geklickt werden und den Namen und den Wert eingegeben werden.
![image](https://github.com/ooDominikoo/HartmannDominikLB-324/assets/104886373/71c61f41-1f20-44a3-bc9b-72fc5a50e20d)
10. Sobald dieser Link ausgeführt wird, kann man sich mit den vorhin gezeigtem Password einloggen.
![image](https://github.com/ooDominikoo/HartmannDominikLB-324/assets/104886373/04b32dde-a642-41df-9950-037cb3113799)

11. Link zur Azure Website: https://hartmanndominiklb324.azurewebsites.net/
