# Schachspiel

Dies ist ein einfaches Schachprojekt, das grundlegende Schachregeln enthält und eine benutzerfreundliche Schnittstelle für Spieler bietet. Unten finden Sie eine kurze Erklärung, wie Schach gespielt wird.

![Chessboard](https://i.postimg.cc/5NFWBj5j/Screenshot-2025-04-14-2-02-26-PM.png)

## Grundlegende Schachregeln

1. **Ziel**: Das Ziel des Schachspiels ist es, den **König** des Gegners schachmatt zu setzen. Das bedeutet, dass der König bedroht ist und nicht entkommen kann.
   
2. **Schachbrett**: Das Spiel wird auf einem 8x8 Schachbrett mit abwechselnd hellen und dunklen Feldern gespielt.

3. **Figurenzüge**:
   - **König**: Zieht ein Feld in eine beliebige Richtung.
   - **Königin**: Bewegt eine beliebige Anzahl von Feldern in eine beliebige Richtung.
   - **Turm**: Bewegt eine beliebige Anzahl von Feldern in vertikaler oder horizontaler Richtung.
   - **Läufer**: Bewegt eine beliebige Anzahl von Feldern in diagonaler Richtung.
   - **Pferd**: Zieht in einer „L“-Form (zwei Felder in eine Richtung, dann ein Feld in eine senkrechte Richtung).
   - **Bauer**: Zieht ein Feld vorwärts, kann aber beim ersten Zug zwei Felder vorrücken. Sie schlägt diagonal.

4. **Schach**: Wenn der König eines Spielers bedroht ist, nennt man das „Schach“. Der Spieler muss seinen König schützen, indem er ihn entweder bewegt, eine andere Figur zwischen ihn und die Bedrohung stellt oder die bedrohte Figur schlägt.

5. **Schachmatt**: Wenn der König eines Spielers schachmatt gesetzt wird, ist das Spiel vorbei, und der andere Spieler gewinnt.

## Wie man das Projekt benutzt

### 1. Laden Sie das Projekt herunter
Laden Sie zunächst die Projektdateien herunter, indem Sie entweder das Repository mit Git klonen oder die ZIP-Datei herunterladen.

#### Option 1: Klonen mit Git
Führen Sie den folgenden Befehl in Ihrem Terminal oder in der Eingabeaufforderung aus:

```bash
git clone https://github.com/FireAnimationStudios/Web-Chess.git
```

#### Möglichkeit 2: Herunterladen als ZIP
Rufen Sie das GitHub-Repository auf und klicken Sie auf die Schaltfläche „ZIP herunterladen“. Entpacken Sie die ZIP-Datei in ein Verzeichnis auf Ihrem Rechner.

### 2. Einrichten des Projekts unter Windows und Linux (Server)

#### Windows:

1. **Installieren Sie einen Webserver (optional, aber empfohlen)**:
   - Sie können Software wie **XAMPP** oder **WampServer** verwenden, um schnell einen lokalen Webserver einzurichten.
   - Wenn Sie die HTML-Datei ohne einen Webserver öffnen möchten, können Sie auch einfach auf die Datei „index.html“ doppelklicken, um sie in Ihrem Standard-Webbrowser anzuzeigen.

2. **Starten Sie das Projekt**:
   - **Mit XAMPP/WampServer**: Nachdem Sie XAMPP oder WampServer installiert haben, legen Sie den Projektordner im Stammverzeichnis des Webservers ab (z. B. „C:\xampp\htdocs“ für XAMPP). Starten Sie dann den Webserver und navigieren Sie zu `http://localhost` in Ihrem Webbrowser, um die Schachpartie zu sehen.
   - **Ohne Webserver**: Doppelklicken Sie auf `index.html`, um es in einem Webbrowser zu öffnen.

#### Linux (Server):

1. **Installieren Sie einen Webserver**:
   - Wenn Sie noch keinen Webserver installiert haben, können Sie **Apache** (oder **Nginx**) installieren. Hier ist die Anleitung für Ubuntu (Sie können sie für andere Distributionen anpassen):

   - **Apache** installieren:
     ```bash
     sudo apt update
     sudo apt install apache2
     ```

   - **Apache starten**:
     ```bash
     sudo systemctl start apache2
     sudo systemctl enable apache2
     ```

2. **Projektdateien in das Webserver-Verzeichnis verschieben**:
   - Auf den meisten Linux-Servern ist das Standardverzeichnis des Webservers `/var/www/html`. Sie können Ihre Projektdateien mit dem folgenden Befehl dorthin verschieben:
     ```bash
     sudo cp -r /pfad/zu/ihrem/projekt/* /var/www/html/
     ```

3. **Zugriffsrechte festlegen** (falls erforderlich):
   - Vergewissern Sie sich, dass der Webserver die richtigen Berechtigungen für den Zugriff auf die Dateien hat:
     ```bash
     sudo chown -R www-data:www-data /var/www/html/
     sudo chmod -R 755 /var/www/html/
     ```

4. **Zugriff auf das Projekt**:
   - Öffnen Sie einen Webbrowser und gehen Sie zur IP-Adresse des Servers oder zu `localhost` (wenn Sie vom Server selbst zugreifen), um das Schachspiel zu sehen:
     ```
     http://localhost
     ```

---

### 3. Genießen Sie das Spiel!
Nach der Einrichtung können Sie nun mit dem Schachspiel beginnen. Wenn Sie einen Server einrichten, können andere über die öffentliche IP-Adresse oder den Domainnamen des Servers auf das Spiel zugreifen.

## Demnächst verfügbar

- **Online-Mehrspieler**: Fordern Sie Spieler aus der ganzen Welt zu einer Schachpartie in Echtzeit heraus.
- **KI mit verschiedenen Schwierigkeitsgraden**: Spielen Sie gegen einen Computergegner mit einstellbaren Schwierigkeitsgraden, die von Anfänger bis Experte reichen.

---

© 2025 Fabi & FireAnimationStudios. Alle Rechte vorbehalten.
