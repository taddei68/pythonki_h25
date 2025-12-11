# pythonki_h25
Midlertidig repositorie for kurs desember 2025

# Oppgave(r) - Kommer litt og litt...

## Oppgave 1 - Scikit-learn - Sett opp, tren og bruk en modell
Gitt det innebygde Iris datasettet, prøv å klassifiser følgende observasjon: iris_observation = [5.5, 2.9, 4.0, 1.4]

Dette er altså en observasjon med følgende egenskaper: sepal_length_cm = 5.5, sepal_width_cm = 2.9, petal_length_cm = 4.0, petal_width_cm = 1.4.

- Lag en ny notebook.
- Last inn Iris datasettet.
- Sett opp en egnet modell. Vi brukte LogisticRegression i gjennomgangen på fredag.
- Tren modellen (.fit())
- Bruk modellen til å gjøre prediksjon på observasjonen over (.predict())

Bonus oppgave: Kan du gjøre et sannsynlighetsestimat på den trente modellen? Hvor sikker er den på at den har gitt deg rett klassifisering?

## Oppgave 2 - TensorFlow
Vi kan bruke Google sin Teachable Machine [https://teachablemachine.withgoogle.com/train/image](https://teachablemachine.withgoogle.com/train/image) til å trene en TensorFlow modell som gjenkjenner objekter. Prøv å bruke denne til å lage en enkel modell som kan brukes for å gjenkjenne objekter i et pythonprogram.

- Sett opp et kjøremiljø lokalt på maskinen (virtual environment eller conda environment).
- Installer og aktiver nødvendige biblioteker i dette kjøremiljøet.
- Skriv kode som kan laste inn og bruke resultatet som du laget i Teachable Machine.

*Grunnet en feil / utdatert eksport fra Teachable machine må en sette opp pythonmiljøet med en eldre versjon av python og TensorFlow.*

    % conda create -n tensorflow python=3.11
    % conda activate tensorflow
    % pip install tensorflow==2.13
    % pip install opencv-python

*Med miljøet beskrevet over vil det være mulig å laste inn TensorFlow -> Keras (h5) som er anbefalt eksportformat fra Teachable Machine.*

Hvordan bruke Teachable Machine for å trene en KI modell med egne bilder: [https://youtu.be/ie9d9VUnKAc](https://youtu.be/ie9d9VUnKAc)

Hvordan opprette et virtuelt kjøremiljø lokalt på maskinen i Visual Studio Code: [https://youtu.be/Sk4vXDUb2UI](https://youtu.be/Sk4vXDUb2UI)

## Oppgave 3 - OpenCV og ansiktgjenkjenning i bilder
Bruk OpenCV og haarcascades til å gjenkjenne objekter i et bilde.

- Ta utgangspunkt i notebooken git_code/Pythonkurs - 02 - Tirsdag - Bildebehandling.ipynb
- Finn et egnet bilde og se om du greier å detektere andre features, f.eks munn / øyner.

Her er en video som gir en gjennomgang av temaet: https://youtu.be/TG6PRETpaJI

Her er en video som viser hvordan du kan laste opp filene du trenger i Google Colab: https://youtu.be/G86TFkQh3nk

Dere finner flere trente haarcascade set her https://github.com/opencv/opencv/tree/master/data/haarcascades
