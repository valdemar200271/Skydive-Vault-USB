# Skydive-Vault-USB
Skydive Vault USB er et gratis Windows-program udviklet til faldskærmsspringere. Sortér automatisk videoer efter optagedato, trim optagelser, rediger metadata og håndter videoeksport. Programmet kører direkte fra et USB-stik uden installation. Udviklet af en faldskærmsspringer til faldskærmsspringere.

SKYDIVE VAULT USB – GUIDE
Version 1.1.0 (V9)
========================

Skydive Vault USB er et Windows-program til at gennemse, trimme og organisere faldskaermsoptagelser. Programmet er lavet til at goere haandtering af mange videoer hurtigere og mere overskuelig.

1. INSTALLATION FOR BRUGERE
-------------------------
1) Download Skydive_Vault_USB_v1.1.0_Setup.exe fra:
   https://github.com/valdemar200271/Skydive-Vault-USB/releases/latest
2) Dobbeltklik paa installationsfilen paa en Windows-computer.
3) Foelg guiden. Vaelg den mappe, hvor programmet skal installeres. (USB)
4) Klik Faerdig. Start 'Skydive Vault USB' fra Start-menuen eller direkte fra installationsmappen.

BEMAERK: En installeret version kan oprette en Start-menu-genvej. Windows starter normalt ikke programmer automatisk, naar et USB-stik saettes i. Aabn derfor programmet manuelt. Paa fremmede computere kan sikkerhedsregler blokere ukendte EXE-filer.

2. SAADAN BRUGER DU PROGRAMMET
----------------------------
HJEM: Se overblik, videoer og ledig plads.
SORTER: Organiser videoer i datomapper ud fra optagelsesdato i videofilen. Hvis en fil ikke har brugbare metadata, kan sorteringen bruge en alternativ dato.
TRIM: Vaelg en video, afspil den, og traek start- og slutmarkoer paa tidslinjen. Gem et klip som en ny fil, eller vaelg at erstatte originalen.
AENDR DATO: Ret en videos dato eller navn, naar oplysningerne ikke passer.
RENS USB: Ryd op i valgte datomapper/videoer. Kontroller udvalget grundigt, inden du sletter.
EKSPORT: Foelg fremdrift og forventet resterende tid i panelet til hoejre. Eksporter kan saettes i koe, og der kan startes flere sidelobende (op til fire).
SORTER EFTER / LUK EFTER: Vaelg om programmet skal sortere filer og/eller lukke, naar eksportkoeen er faerdig.
OPDATERING: Programmet undersoeger GitHub for nye versioner ved opstart. Du kan ogsaa soege manuelt via knappen i menuen. Hvis en nyere version findes, aabnes dens GitHub-side, hvor du selv downloader den.

3. VIGTIGT OM VIDEOER
--------------------
- Tag en sikkerhedskopi af uerstattelige optagelser, foer du bruger trim, erstat eller slet.
- Test gerne programmet med et par kopier foerst.
- Eksport kan tage tid afhængigt af videolaengde og computerens hastighed.
- Ikke alle videocodecs kan nødvendigvis forhåndsvises på alle Windows-computere.
- Undlad at fjerne USB-stikket under eksport eller flytning af filer.

4. TIL UDVIKLEREN – BYG EXE OG INSTALLER
---------------------------------------
Denne del er KUN til den, der bygger programmet. Almindelige brugere behoever ikke Python eller Inno Setup.

Krav: Windows, Python 3 med 'py'-launcher, internetforbindelse og Inno Setup 6.
1) Pak byggepakken ud i en almindelig mappe paa din Windows-computer.
2) Dobbeltklik paa BYG_EXE_OG_INSTALLER.bat.
3) Scriptet installerer Python-afhaengigheder og henter FFmpeg/FFprobe, hvis de ikke allerede findes i mappen.
4) PyInstaller bygger dist\Skydive Vault USB.exe med de noedvendige FFmpeg-filer inkluderet.
5) Hvis Inno Setup 6 er installeret i standardmappen, bygges installationsfilen automatisk:
   Installer_Output\Skydive_Vault_USB_v1.1.0_Setup.exe
6) Hvis Inno Setup ikke findes automatisk, aabn Skydive_Vault_USB_Installer.iss i Inno Setup og tryk Compile.
7) Afproev installationsfilen paa en Windows-PC, foer den udgives.
8) Opret en GitHub Release med tag v1.1.0 og upload Setup.exe som vedhaeftet fil.

GITHUB OG OPDATERINGER
---------------------
Repository: https://github.com/valdemar200271/Skydive-Vault-USB
Opdateringstjekket er sat til dette repository. En ny udgivelse skal oprettes som en GitHub Release med et hoejere versionsnummer, foer programmet kan finde den.

SUPPORT
-------
Projekt: Skydive Vault USB
Udvikler: Valdemar Schmidt
