# SMB CIFS
## Worüber reden wir eigentlich?

---

### Inhalt
- Definitionen
- Funktionen 

---

# CIFS

- **S**erver**M**essage**B**lock
- Samba

---

# CIFS
- Uraltversion von SMB1
- Heute CIFS => SMB

---

SMB

---

- Seit 1990 von MS für Datei-/Druckerzugriff im Netzwerk genutzt
- über TCP/IP
- **DAS** Protokoll zwischen MS Client <> Server + Server <> Server
- SMB1, SMB2, SMB3(seit Win 8)
    - z.b. server-side copy
- SMB1 seit Win 10 1803 deaktiviert
    - nötig für z.B. alte Samba4 NT4-Domäne

----

Samba

----

- freie Implementierung von SMB für Nutzung mit Unix usw.
- SMB bis 2007 closed source
- Samba ermöglicht voll funktionsfähige Windows Domänen ohne WindowsServer

----

## Weiterführendes
- https://www.samba.org/cifs/docs/what-is-smb.html
- https://docs.microsoft.com/en-us/windows/desktop/fileio/microsoft-smb-protocol-and-cifs-protocol-overview
- [SMB2 Reference](https://msdn.microsoft.com/en-us/library/cc246488.aspx)
- [Talk: SMB and AD protocol implementation in Samba](https://www.youtube.com/watch?v=jWJKxAHq0X8)
- [Podcast: CRE025 Samba](https://cre.fm/cre025-samba)
- [Gerichtssteit bzgl.. SMB/samba](https://fsfe.org/activities/ms-vs-eu/ms-vs-eu.de.html)