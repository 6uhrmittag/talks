# SMB/CIFS, Samba
## Begriffsklärung

---

## @color[red](S)erver @color[red](M)essage @color[red](B)lock

---

- regelt seit 1990 den Datei-/Druckerzugriff in Microsoft Netzwerken
- **DAS** Protokoll zwischen MS Produkten
- SMB1, SMB2, SMB3(seit Win 8)
    - zwischen SMB1/SMB2: kurzzeitig CIFS


Note:

- SMB1 seit Win 10 1803 deaktiviert
    - nötig für z.B. alte Samba4 NT4-Domäne
- Common Internet File System
    - Zwischen SMB1 und SMB2 als Konter zu Sun's WebNFS 
---

- SMB bildet quasi alle Dateizugriffsvorgänge ab
- und mehr z.B. 
    - server-side copy
    - Hyper-V storage
    - SQL over Network

Note:
- Verwaltungsservice auf Client: LanManWorkstation
- SMB macht auch RPC(Remote Procedure Call) -> Remotekommandos für Windows über Netzwerk

---

## Samba

---

- freie Implementierung von SMB für Nutzung mit Unix usw.
- SMB bis 2007 closed source
- transparenter Ersatz für Windows Server

Note:

- Vor WindowsNT Entwickelt, ursprüngliche nicht als Microsoft-Ersatz entwickelt
- Klage da MS mit Geheimhaltung von SMB Interoperabilität verhindert
- Gerichtliche für Microsoft Strafe war 860 Millionen Euro
- Samba ermöglicht z.B.
    - SMB für kostenlose NAS Betriebssysteme
    - Bundestag AD ohne Windows Server
- Entwicklung viel durch deutsche Firma SerNet
---

## Weiterführendes
- https://www.samba.org/cifs/docs/what-is-smb.html
- https://docs.microsoft.com/en-us/windows/desktop/fileio/microsoft-smb-protocol-and-cifs-protocol-overview
- [Gerichtssteit bzgl. SMB/samba](https://fsfe.org/activities/ms-vs-eu/ms-vs-eu.de.html)
- [SMB2 Reference](https://msdn.microsoft.com/en-us/library/cc246488.aspx)
- [Talk: SMB and AD protocol implementation in Samba](https://www.youtube.com/watch?v=jWJKxAHq0X8)
- [Podcast: CRE025 Samba](https://cre.fm/cre025-samba)
