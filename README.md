# OSko
|       *comandy*                                       |
|-------------------------------------------------------|
|**vypsani_vsech_operaci**                              |
|          ps_ax                                        |
|    ps_ax | grep bash                                  |
| awk-textový preprocesor                               |
|ps_ax|grep bash|'{print$0;}'                           |
|ps_ax |grep -m l bash |'{print$0;}' - vyhledá PID bashe|
|kill -9 `ps_ax|grep -m l bash|'{print$0;}'`            |
|-------------------------------------------------------|
|**    tvorba-souboru   **                              |
|           touch                                       |
|-------------------------------------------------------|
|**   psani-do-souboru  **                              | 
|     vim nazev souboru                                 |
||------------------------------------------------------|
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

