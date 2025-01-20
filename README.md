# Git ja GitHub - Miksi ja miten käyttää?

Tämä tiedosto tarjoaa yksityiskohtaisen yleiskatsauksen siitä, mitä Git ja GitHub ovat, miksi ne ovat keskeisiä työkaluja ohjelmistokehityksessä, sekä ohjeet siitä, miten niitä käytetään käytännössä. Oppaamme on suunnattu erityisesti aloittelijoille, jotka haluavat oppia versionhallinnan ja yhteistyön perusteet.

---

## **Mikä on Git?**

Git on tehokas versiohallintajärjestelmä, jonka avulla voit seurata ja hallita ohjelmistoprojektiesi muutoksia. Se on avoimen lähdekoodin työkalu, jota käytetään laajalti ohjelmistokehityksessä ympäri maailmaa.

### **Gitin pääominaisuudet:**
- **Versionhallinta:** Git tallentaa kaikki projektisi muutokset. Voit palata aiempiin versioihin tai tutkia, mitä muutoksia on tehty ja kuka ne on tehnyt.
- **Haarojen hallinta:** Voit luoda ja hallita eri haaroja projektin eri ominaisuuksille tai kokeiluille ilman, että vaikutat päähaaraan.
- **Yhteistyö:** Gitin avulla useat kehittäjät voivat työskennellä samassa projektissa ja yhdistää muutoksensa saumattomasti.

---

## **Mikä on GitHub?**

GitHub on pilvipohjainen alusta, joka toimii Git-versionhallintajärjestelmän päällä. Sen avulla voit tallentaa, jakaa ja hallita Git-repositorioita tehokkaasti.

### **GitHubin pääominaisuudet:**
- **Repositoriot:** Voit luoda julkisia tai yksityisiä projekteja.
- **Yhteistyötyökalut:** GitHub tarjoaa ominaisuuksia, kuten pull requestit, koodiarvioinnit ja issue-järjestelmän.
- **Avoimen lähdekoodin projektit:** GitHub on erinomainen paikka jakaa omia projekteja tai osallistua muiden kehittäjien projekteihin.
- **Automaatiotyökalut:** Continuous Integration/Continuous Deployment (CI/CD) -työkalut helpottavat ohjelmistojen automaattista testausta ja julkaisua.

---

## **Git ja GitHub käytännössä**

### 1. **Asennus**
- **Git:** Lataa ja asenna Git tietokoneellesi: [Git lataussivusto](https://git-scm.com/).
- **GitHub:** Luo GitHub-tili ja kirjaudu sisään: [GitHub](https://github.com/).

### 2. **Projektin aloittaminen**
1. **Luo uusi kansio projektiasi varten**
   ```bash
   mkdir oma-projekti
   cd oma-projekti
   ```
2. **Alusta Git-repositorio**
   ```bash
   git init
   ```
3. **Lisää tiedostot versiohallintaan**
   ```bash
   git add .
   ```
4. **Tee ensimmäinen commit**
   ```bash
   git commit -m "Ensimmäinen commit"
   ```

### 3. **Yhdistäminen GitHubiin**
1. **Luo uusi repositorio GitHubissa.**
2. **Yhdistä paikallinen repositorio GitHubiin:**
   ```bash
   git remote add origin <repository_url>
   git branch -M main
   git push -u origin main
   ```

### 4. **Muutosten tekeminen ja päivittäminen**
1. **Muokkaa tiedostoja projektissasi.**
2. **Seuraa tiedostojen tilaa:**
   ```bash
   git status
   ```
3. **Lisää ja commitoi muutokset:**
   ```bash
   git add .
   git commit -m "Kuvaus muutoksista"
   ```
4. **Lähetä muutokset GitHubiin:**
   ```bash
   git push
   ```

---

## **Hyödyllisiä komentoja ja vinkkejä**

- **Clonaa olemassa oleva repositorio GitHubista:**
  ```bash
  git clone <repository_url>
  ```
- **Luo uusi haara ja vaihda siihen:**
  ```bash
  git branch uusi-haara
  git checkout uusi-haara
  ```
  Tai lyhyemmin:
  ```bash
  git checkout -b uusi-haara
  ```
- **Yhdistä haara päähaaraan:**
  ```bash
  git checkout main
  git merge <haara>
  ```
- **Hae päivitykset GitHubista:**
  ```bash
  git pull
  ```
- **Ratkaise yhdistämis- tai merge-konflikteja:**
  Kun konflikti syntyy, muokkaa tiedostoja manuaalisesti ja tee commit:
  ```bash
  git add .
  git commit -m "Ratkaistu konflikti"
  ```

---

## **Miksi Git ja GitHub ovat tärkeitä?**

1. **Tiimityöskentely:** Git ja GitHub helpottavat yhteistä työskentelyä ohjelmistoprojekteissa. Useat kehittäjät voivat työskennellä samassa projektissa ilman, että koodi menee sekaisin.

2. **Versionhallinta:** Voit aina palata aikaisempiin projektiversioihin, nähdä muutosten historia ja hallita projektiasi paremmin.

3. **Koodin jakaminen:** Voit helposti jakaa koodisi muiden kehittäjien kanssa tai osallistua avoimen lähdekoodin projekteihin.

4. **Automaatio:** GitHub mahdollistaa automaattisten testien, buildien ja julkaisujen suorittamisen suoraan repositoriostasi.

---

## **Lisäresurssit**

- [Git virallinen dokumentaatio](https://git-scm.com/doc)
- [GitHubin oppaat](https://docs.github.com/)
- [Ilmainen Git-oppikirja](https://git-scm.com/book/fi/v2)
- [Ohjeita GitHubin pull requesteihin](https://docs.github.com/en/pull-requests/)

Tämä tiedosto on vasta alku matkalle Gitin ja GitHubin tehokkaaseen käyttöön. Kokeile, opettele ja ala hyödyntämään näitä työkaluja omissa projekteissasi!

