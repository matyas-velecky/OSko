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
|----------------------------------------------------|
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
|**installačka na server**|
| sudo apt install openssh sever |
|*generování*|
|ssh-keygen|
|*kopírování na klienta serveru*|
|ssh-copy-id <ip>|
|*nastavení přihlášení pouze přes ssh*|
|nano /etc/ssh/sshd_config|
|**proměné v operační paměti**|
|set|
**root.cz - užitečný web**
zero-day = Přes chybu programu je útočník schopen přepsat kód a dát tam nějaký virus.
|**přidání uživatele**|
|----------------------------------------------------|
|useradd|
|  -pro skripty(neinteraktivní)|
|adduser|
|  -pro terminal(interaktivní)|
|----------------------------------------------------|
|sudo usermod|
|  -pro přidání uživatele do skupin|
|sudo gruoups xxx|
|sudo gruoups -aG users xxx|
|  -přidá uživatele do skupiny xxx|
|passwd|
| -změna hesla|
|sudo cat /etc/passwd|
| -zakladní parametry uživatele|
|sudo cat /etc/shadow|
| -obsahuje stopu hesla|
|sudo cat /etc/group|
|  -ukáže skupiny|

127.0.0.1 = lokální rozhraní, lze se na něho dostat pouze ze svého počítače do ského počítače

|**syncthing**|
|-------------|
|sudo mkdir -p /etc/apt/keyrings|
|sudo curl -L -o /etc/apt/keyrings/syncthing-archive-keyring.gpg https://syncthing.net/release-key.gpg|
|echo "deb [signed-by=/etc/apt/keyrings/syncthing-archive-keyring.gpg] https://apt.syncthing.net/ syncthing stable" | sudo tee /etc/apt/sources.list.d/syncthing.list|
|sudo apt-get update|
|sudo apt-get install syncthing|
