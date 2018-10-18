# SMB/CIFS/Samba

---

# Was ist ist was?

---

# CIFS
- Uraltversion von SMB1 (1996)
- Heute CIFS => SMB

Note:

- Common Internet File System
- Zwischen SMB1 und SMB2 als Konter zu Sun's WebNFS 


---

**S**erver**M**essage**B**lock

---

- Seit 1990 von MS für Datei-/Druckerzugriff im Netzwerk genutzt
- über TCP/IP
- **DAS** Protokoll zwischen MS Client <> Server + Server <> Server
- SMB1, SMB2, SMB3(seit Win 8)
    - z.b. server-side copy
- SMB1 seit Win 10 1803 deaktiviert
    - nötig für z.B. alte Samba4 NT4-Domäne

Note:

- SMB macht auch RPC -> Remotekommandos für Windows über Netzwerk

---

Samba

---

- freie Implementierung von SMB für Nutzung mit Unix usw.
- SMB bis 2007 closed source
- Samba ermöglicht voll funktionsfähige Windows Domänen ohne WindowsServer

Note:

- Klage da MS mit geheimhaltung von SMB Interoperabilität verhindert
- Gerichtliche für Microsoft Strafe war 860 Millionen Euro

---

## Weiterführendes
- https://www.samba.org/cifs/docs/what-is-smb.html
- https://docs.microsoft.com/en-us/windows/desktop/fileio/microsoft-smb-protocol-and-cifs-protocol-overview
- [SMB2 Reference](https://msdn.microsoft.com/en-us/library/cc246488.aspx)
- [Talk: SMB and AD protocol implementation in Samba](https://www.youtube.com/watch?v=jWJKxAHq0X8)
- [Podcast: CRE025 Samba](https://cre.fm/cre025-samba)
- [Gerichtssteit bzgl.. SMB/samba](https://fsfe.org/activities/ms-vs-eu/ms-vs-eu.de.html)

footnote : "2018 - Marvin Heimbrodt"
