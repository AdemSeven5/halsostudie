# Hälsostudie – del 1

Författare: Adem Seven  
Pythonversion: 3.14.7

## Om projektet

I projektet analyserar jag ett dataset med 800 deltagare.
Syftet är att beskriva deltagarnas hälsodata och öva på
statistik, visualisering, simulering och hypotestest.

[Öppna rapporten med kod, diagram och förklaringar](halsostudie_arbete.ipynb)

## Vad innehåller analysen?

- Medelvärde, median, min och max för ålder, vikt, längd,
  övertryck och kolesterol.
- Ett histogram över deltagarnas övertryck.
- Ett lådagram över viktfördelningen för kvinnor och män.
- Ett stapeldiagram över deltagarnas rökvanor.
- Beräkning av andelen deltagare med sjukdomen.
- Simulering av 1 000 personer med samma sjukdomssannolikhet.
- Ett 95-procentigt konfidensintervall för genomsnittligt övertryck.
- Ett ensidigt Welchs t-test som jämför övertryck hos
  rökare och icke-rökare.

## Projektets filer

- `halsostudie_arbete.ipynb`: rapporten med hela analysen.
- `data/health_study_dataset.csv`: datasetet som analysen använder.
- `requirements.txt`: Pythonpaketen som behövs.
- `.gitignore`: anger vilka filer Git ska ignorera,
  exempelvis den virtuella miljön.

## Köra projektet i Windows och VS Code

1. Öppna projektmappen som innehåller denna README.
2. Ha tilläggen Python och Jupyter installerade i VS Code.
3. Skapa en virtuell miljö och installera paketen i terminalen:

```powershell
python -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
```

4. Öppna `halsostudie_arbete.ipynb`.
5. Välj projektets `.venv` som kernel.
6. Klicka på Restart och därefter Run All.

Datasetet läses med en relativ sökväg.
Slumptalsfröet 42 används för att simuleringen ska kunna upprepas.