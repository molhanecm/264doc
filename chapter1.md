# First Chapter - inicializace

soubor: V:\SETWRK.BAT kde V: je \\etg.feld.cvut.cz\vyuka

účel: mastavit stanici tak, bay se na ní spustil autologon

podmínka: spouští uživatel s admin právy

Stručný popis:

1. **NASTAVENI AUTOLOGONU**
2. Vytvoření adresáře c:\bat, když už neexistuje a
3. Nakopírovat do něj soubor n:\auto.tpl, přejmenovaný na autoexec.bat, kde N: je \\etg.feld.cvut.cz\vyuka
4. Vytvoření klíče v registry pro LOGON script, soubor s registrem je n:\logon.reg, musí se ale nakopírovat nejdříve na lokál, do c:\bat, protože jinak nejde spustit! Vše se musí aspoň třikrát odklikat při běhu skriptu.
5. Překopíruji si pod c:\bat GroupPolicy z N: pomocí XCOPY a pak to nakopíruji pod C:\Windows\System32\GroupPolicy\User\Scripts pomocí XCOPY a ELEVATE
6. ----- poznámka, tohle ale nestačí, stejnak musím spustit gpedit -----
7. **NASTAVENI IKON V PUBLIC**
8. Nakopíruji ikony z N:\Desktops\public do C:\Users\Public\Desktop

9. Překopíruji nadbytečné ikony do c:\TMP\exdir\

10. A smažu nadbytečné v C:\Users\Public\Desktop

11. **SPUSTIM GPEDIT a odkliknu to co jsem předtím nastavil**



