<a href="https://rp.svilenkovic.rs/"><img src="media/cover.jpg" alt="Balkan RP, naslovna strana na laptopu i telefonu" width="100%"></a>

# Balkan RP

Demo za izmišljeni FiveM roleplay server: cela strana je jedan neprekidan let kroz grad u sedam poglavlja, a pokreće ga skrol.

**[rp.svilenkovic.rs](https://rp.svilenkovic.rs/)** · [Studija slučaja](https://svilenkovic.rs/radovi/balkan-roleplay) · [English](README.md)

> [!NOTE]
> Moj sopstveni demo. Izvorni kod je privatan. Ova stranica opisuje ideju i kako je napravljen.

<table>
  <tr><td><b>Klijent</b></td><td>Sopstveni demo</td></tr>
  <tr><td><b>Delatnost</b></td><td>FiveM roleplay zajednica (izmišljena)</td></tr>
  <tr><td><b>Lokacija</b></td><td>Srbija</td></tr>
  <tr><td><b>Vrsta</b></td><td>Sajt sa videom koji se pokreće skrolom</td></tr>
  <tr><td><b>Moj deo posla</b></td><td>Koncept, dizajn, izrada i hosting</td></tr>
  <tr><td><b>Tehnologije</b></td><td>Vanilla JS, CSS, ffmpeg, nginx</td></tr>
</table>

## O projektu

Balkan RP je demo za roleplay zajednicu na FiveM-u, modifikaciji za GTA V koja dozvoljava privatne servere. Server ne postoji i sajt to ne krije: oznaka DEMO stoji u uglu svake strane, a uslovi korišćenja time i počinju. Publika je ipak stvarna. Igrači svaki dan gledaju grafiku iz igre, pa je prvi utisak morao da bude sam grad.

Ranija verzija je koristila Three.js scenu u kojoj je samo jedan modul imao 934 KB. Zamenio sam je letom kroz grad od šesnaest sekundi, bez ijednog reza. Preko njega se smenjuje sedam poglavlja, a akcentna boja prati film od dana ka noći. Pri učitavanju strana bira jedan od tri režima: premotavanje videa na uređajima sa mišem, 161 WebP sliku na platnu za ekrane na dodir i običnu stranu sa posterom kada je uključena ušteda podataka ili smanjenje pokreta.

## Šta sam uradio

- Tri fajla pisana ručno, bez build koraka: jedan HTML, oko 10 KB CSS-a i oko 5 KB JavaScript-a
- Traka od 1050vh na širokom ekranu i 800vh na telefonu, sa poslednjim poglavljem zakačenim za dno da ne isklizne ispod kraja filma
- Navigacija od sedam tačaka i traka napretka izvedene iz iste pozicije u filmu, pa ne mogu da se raziđu
- Film u kome je svaki kadar ključni, uz blago uklanjanje šuma i CSS sloj zrna koji vraća teksturu
- Verzija u imenu fajlova, keš od godinu dana, delimični zahtevi i film u dve veličine, oko 20 MB i 9,5 MB
- Popravljen pad koji se javljao samo na telefonu: poziv koji odlaže učitavanje dok pregledač ne bude slobodan dobijao je broj umesto objekta sa timeout-om

## Snimci ekrana

<table>
  <tr>
    <td width="68%" valign="top"><img src="media/desktop.webp" alt="Balkan RP, naslovna strana na ekranu širine 1440 px"></td>
    <td width="32%" valign="top"><img src="media/mobile.webp" alt="Balkan RP, naslovna strana na telefonu"></td>
  </tr>
</table>

<img src="media/inner-1.webp" alt="01 / O serveru: &quot;Dobrodošao u Los Santos.&quot; preko kadra iz filma">
<sub>01 / O serveru: "Dobrodošao u Los Santos." preko kadra iz filma</sub>

<img src="media/inner-2.webp" alt="02 / Karakter: kartica sa poglavljem i oznakama o sadržaju">
<sub>02 / Karakter: kartica sa poglavljem i oznakama o sadržaju</sub>

---

<sub>Izrada: [D. Svilenković](https://svilenkovic.rs).</sub>
