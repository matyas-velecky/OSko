# OSko
|       *comandy*                                       |
|-------------------------------------------------------|
|**vypsani_vsech_operaci**                              |
|          ps_ax                                        |
|    ps_ax \| grep \<co cheme vhledat>                                  |
|ps_ax \| grep \<co chceme vzhledat>\|'{print$<číslo>;}'                             |
|ps_ax  \| grep -m 1 \<co chceme vzhledat> \| '{print$<číslo>;}' - vyhledá PID bashe  |
|kill -9 `ps_ax \|grep -m 1 <co chceme vzhledat> \|'{print$<číslo>;}'`            |
|-------------------------------------------------------|
|**    tvorba-souboru   **                              |
|           touch                                       |
|-------------------------------------------------------|
|**   psani-do-souboru  **                              | 
|     vim nazev souboru                                 |
|-------------------------------------------------------|
|**    ukázání-IPiny    **                              |
|        if_config                                      |
|-------------------------------------------------------|
|    *práce ze soubory*                                 |
|-------------------------------------------------------|
|        **cat**                                        |
|-------------------------------------------------------|
|     vepíše do souboru                                 |
|  cat > (název souboru)                                |
|-------------------------------------------------------|
| očísluje a vypíše řádky                               |
|         cat -n                                        |
|-------------------------------------------------------|
|        **chmod**                                      |
|-------------------------------------------------------|

U = vlastník;
q = skupina;
o = ostatní;

Triplets
r = 4;
w = 2;
x = 1;

|         chmod                                        |
|------------------------------------------------------|
|  př. chmod u+x (nazev_souboru)                       |
|  chmod 752 (nazev_souboru)                           |
|------------------------------------------------------|
|        ** jak vepsat proměnou do RAM**                                       |
|export <jméno proměnné> ="<proměnná>|
|------------------------------------------------------|
|**zapnutí vscode v bashy**|
|code .bashrc|
|**změna hostname**|
|cat/etc/hostname|
|**vypsání hardware**|
|----------------------------------------------------|
|*všeho*|
|lshw|
|*v USB*|
|lsusb|
|*vypsání všeho připojeného*|
|lspci|
|**textový preprocesor**|
| awk                              |
|**vyhledávání souborů**|
|----------------------------------------------------|
|grep <název souboru>|
|*locate*|
|sudo apt-get install plocate|
|locate <název souboru>|
|*pro servery lepší*|
|find <název souboru>|
|**zjištění voleného místa na hdd/ssd**|
|----------------------------------------------------|
|df|
|**root přihlášení**|
|sudo su|
|**ssh klíče**|
|----------------------------------------------------|
|*generování*|
|ssh-keygen|
|*kopírování na klienta serveru*|
|ssh-copy-id <ip>|
|*nastavení přihlášení pouze přes ssh*|
|nano /etc/ssh/sshd_config|
|**proměné v operační paměti**|
|set|
