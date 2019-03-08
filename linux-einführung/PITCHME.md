Einführung Linux
---

### Inhalt
- Allgemein zu Linux
- Verbinden zu Linux
- Bedienen von Linux
- Zurechtfinden in Linux
- Informationen finden über Linux

---

### Linux
- allgemeine Bezeichnung für Unix-basierte Betriebssysteme
- Linux, BSD, Solaris usw. stammen von Unix ab
- Ubuntu (basiert auf Debian @fa[hand-o-right] basiert auf Unix)

---

### Aufbau
1. Kernel steuert Hardware (z.B. via Treiber)
2. Shell: textbasierende Benutzerschnittstelle zu Kernel (z.B. BASH /bin/bash)

---

### Benutzung
- GUI @fa[thumbs-o-down] Ressourcenverbrauch hoch
- Konsole @fa[thumbs-o-up] @fa[hand-o-right] direkte Kommunikation mit Kernel (System-Kern) (z.B. via RS232)

---

### Terminal
![Hardware Terminal](assets/terminal.jpg)

---

### Terminal

- Software/Hardware zur entfernten Bedienung des Kernels (remote Console)
- Hardware: (z.B. seriell verbundener) remote + Monitor + Tastatur
- Software: Terminal Emulator
- Ubuntu/MacOS @fa[hand-o-right] natives Terminal
- Windows @fa[hand-o-right] Putty, MobaXterm, Cygwin

---

Verbinden zu Linux

---

### Remote Zugriff
- SSH(verschlüsselt)! (**S**ecure**SH**ell)
- Passwort oder Private/Public-Key
- Verbinden: `ssh root@test.de`
- Wichtig: Standartport bzw. keine Angabe = 22
- oft verändert. dann `ssh -p 7411 test.de`

Note: Ändern der Ports ist auch Sicherheitsmaßnahme
---

### Demo

---

# Bedienen von Linux

---

### Allgemein
- Befehle auf allen Unix basierten Systemen sehr ähnlich
- Befehle = Programme (+ Zusatzoption)
- `ls` = führe `/bin/ls` aus
- Befehlsname = Abkürzung für Beschreibung

@fa[keyboard-o] 

- `ls` @fa[hand-o-right] **l**ist **d**irectory
- `pwd` @fa[hand-o-right] **p**rint **w**orking **d**irectory 

---


# Zurechtfinden in Linux

---

### Hilfe
- "manual pages" @fa[hand-o-right] `man` (**man**ual pages)
- Stichwortsuche @fa[hand-o-right] `man -k` "Stichwort"
- `man ls`

```
NAME
       ls - list directory contents
DESCRIPTION
       List information about the FILEs (the current directory by default).  Sort entries alphabetically if none of -cftuvSUX nor --sort is specified.
```

Note:
- "apropos" für Stichwortsuche.
---

### Bewegen im System

@fa[keyboard-o] 
- `ls` @fa[hand-o-right] **l**ist **d**irectory
- `cd` @fa[hand-o-right] **c**ange **d**irectory
- `pwd` @fa[hand-o-right] **p**rint **w**orking **d**irectory 
- `grep` @fa[hand-o-right] `grep "müller" adressbuch.txt`

---

### Dateien finden

- [Filesystem Hierarchy Standard](http://refspecs.linuxfoundation.org/FHS_3.0/fhs-3.0.pdf)
- Linux Dateisystem (`/` `/var` `/etc` `/var/www` usw. z.B. Apache Webordner)
- `find / -name gesuchtedatei.txt`

Note: Dateien sind allgemein ähnlich nach FHS organisiert
---

### Dateien bearbeiten und ändern

- `vi` (**vi**sual editor)
- `nano` (etwas einfacher)
- `touch` (leere Datei erstellen)
- `mkdir` (Verzeichnis erstellen)
- `rm` (**r**e**m**ove Datei)
- `chmod` (**ch**ange **mod**e -> Rechte)
- `chown` (**ch**ange **own**er)

Note: vi Tipp: ESC und dann ":q!" -> ":" -> Befehl
---

### Rechte
```
marvin@vm:~$ ls -la testfile
-rw-rw-r-- 1 marvin marvin 11 Feb 28 12:50 testfile
```

- owner - gruppe - other
- nur lesen    : 4
- nur schreiben: 2
- nur ausführen: 1
- rw-rw-r- = 664


```
chmod 766 testfile
marvin@vm:~$ ls -la testfile
-rwxrw-rw- 1 marvin marvin 11 Feb 28 12:50 testfile
```

---

# Informationen finden über Linux

---
### Log-Dateien
- `/var/log`
- `/var/log/syslog`
- `/var/log/apache2/access.log`


```
80.153.234.244 - - [13/Mar/2018:14:15:04 +0100] "GET / HTTP/1.1" 302 431 "-" "Mozilla/5.0 
(Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/64.0.3282.186 Safari/537.36"
```

- `tail -f /var/log/apache2/access.log`
- `grep "80.157.234.242" /var/log/apache2/access.log`

---

### Systeminformatioen
- `uname -a` (Hostname, Kernelversion)
- `lsb_release -a` (Distributionsname z.B. Ubuntu 16.04.4 LTS)
- `top` (Ressourcenmonitor)
- `df -h` (Festplattenspeicher)

---

### Ausblick
- Programme installieren
- Praktische Nutzung
- Workshop "Apache Webserver + Webseite installieren"