# SMB, Samba
## Begriffklärung

---

## **S**erver**M**essage**B**lock

---

- regelt seit 1990 den Datei-/Druckerzugriff in Microsoft Netzwerken
- **DAS** Protokoll zwischen MS Client <> Server + Server <> Server
- SMB1, SMB2, SMB3(seit Win 8)
    - zwischen SMB1/SMB2: kurzzeitig CIFS


Note:

- SMB1 seit Win 10 1803 deaktiviert
    - nötig für z.B. alte Samba4 NT4-Domäne
- SMB macht auch RPC -> Remotekommandos für Windows über Netzwerk
- Common Internet File System
    - Zwischen SMB1 und SMB2 als Konter zu Sun's WebNFS 
---

- SMB bildet quasi alle Dateizugriffsvorgänge ab
- und mehr z.B. 
    - server-side copy
    - Hyper-V storage
    - SQL over Network
- RPC (remote Kommandos)

Note:
- Verwaltungsservice: LanManWorkstation
---

## Samba

---

- SMB bis 2007 closed source
- freie Implementierung von SMB für Nutzung mit Unix usw.
- ermöglicht voll funktionsfähige Windows Domänen ohne WindowsServer

Note:

- Klage da MS mit geheimhaltung von SMB Interoperabilität verhindert
- Gerichtliche für Microsoft Strafe war 860 Millionen Euro

---

## Weiterführendes
- https://www.samba.org/cifs/docs/what-is-smb.html
- https://docs.microsoft.com/en-us/windows/desktop/fileio/microsoft-smb-protocol-and-cifs-protocol-overview
- [Gerichtssteit bzgl. SMB/samba](https://fsfe.org/activities/ms-vs-eu/ms-vs-eu.de.html)
- [SMB2 Reference](https://msdn.microsoft.com/en-us/library/cc246488.aspx)
- [Talk: SMB and AD protocol implementation in Samba](https://www.youtube.com/watch?v=jWJKxAHq0X8)
- [Podcast: CRE025 Samba](https://cre.fm/cre025-samba)
