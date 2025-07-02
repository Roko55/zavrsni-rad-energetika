# Završni rad: Predikcija energetske potrošnje modelom ARIMA i analiza utjecaja na scenarije u EnergyPLAN-u

**Autor:** Roko Bošković
**Mentor:** prof. dr. sc. Neven Duić
**Fakultet:** Sveučilište u Zagrebu, Fakultet strojarstva i brodogradnje
**Datum:** [Upiši datum, npr. Srpanj 2025.]

---

### Sažetak

U kontekstu energetske tranzicije i dekarbonizacije elektroenergetskog sektora, precizno dugoročno planiranje ključan je preduvjet za donošenje ispravnih investicijskih odluka. Ovaj završni rad istražuje i uspoređuje dva fundamentalno različita pristupa za izradu dugoročnih profila potrošnje električne energije: deterministički, temeljen na "bottom-up" analizi, i statistički pristup, temeljen na primjeni SARIMA modela. Cilj rada je analizirati utjecaj odabira metode predviđanja na rezultate simulacija energetskog sustava Republike Hrvatske pomoću softvera EnergyPLAN.

Za potrebe rada, na temelju povijesnih podataka o satnoj potrošnji za 2018. godinu, razvijen je i validiran SARIMA model. Potom su generirani profili opterećenja za godine 2030., 2040. i 2050. primjenom obiju metoda te su korišteni kao ulazni podaci u simulacijske scenarije, uz nepromijenjenu proizvodnu stranu sustava.

Rezultati su pokazali da primjena dviju metoda dovodi do fundamentalno različitih profila opterećenja. Dugoročna ekstrapolacija SARIMA modelom rezultirala je generiranjem nerealističnog, "izglađenog" profila s izrazito visokim faktorom opterećenja, koji gubi ključnu satnu i dnevnu varijabilnost. Korištenje takvog profila u EnergyPLAN simulacijama dovelo je do značajnih razlika u ključnim tehno-ekonomskim pokazateljima. Rad zaključuje da direktna primjena SARIMA modela za dugoročno predviđanje nije prikladna jer može dovesti do pogrešnih zaključaka o potrebama sustava za fleksibilnošću, te se naglašava ključna važnost odabira metodologije predikcije u procesu strateškog energetskog planiranja.

---

### Sadržaj repozitorija

*   **/data/HRel2018.txt**: Ulazna datoteka sa satnim podacima o potrošnji električne energije u Hrvatskoj za 2018. godinu.
*   **`zavrsni_rad_analiza.ipynb`**: Jupyter Notebook datoteka koja sadrži cjelokupni Python kod za učitavanje podataka, eksploratornu analizu, razvoj, treniranje, validaciju i testiranje SARIMA modela.
*   **`requirements.txt`**: Popis svih potrebnih Python biblioteka s verzijama korištenim u analizi.

---

### Potrebne biblioteke

Za pokretanje koda potrebno je imati instaliran Python 3 te sljedeće biblioteke. Najlakši način za instalaciju je korištenjem `pip` upravitelja paketima i `requirements.txt` datoteke:

```bash
pip install -r requirements.txt
```

---

### Kako pokrenuti analizu

1.  Klonirati ili preuzeti ovaj repozitorij na lokalno računalo.
2.  Osigurati da su sve potrebne biblioteke instalirane (vidjeti prethodni korak).
3.  Otvoriti i pokrenuti ćelije u `zavrsni_rad_analiza.ipynb` datoteci koristeći Jupyter Notebook ili Jupyter Lab.
