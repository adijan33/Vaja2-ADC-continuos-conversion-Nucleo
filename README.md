# Vaja2-ADC-continuos-conversion-Nucleo
b) V Analog razdelku levo od sheme mikroprocesorja kliknite Analog. Koliko je vseh ADC pretvornikov? 

Trije ADC pretvorniki

c) Izberite en ADC pretvornik in v njem izberite (prosti) kanal, kjer boste zajemali analogno (single-ended) 
meritev. Na oknu Pinout View se določen pin pobarva v zeleno – zapišite naslov dodeljenega pin-a

PC3


d) Kaj se izpiše poleg pina? Izpiše se ADC3_IN. Potenciometer pravilno priključite na Nucleo razvojno ploščo preko 
protoborda (potenciometer ima 3 priključke: GND, out in +3,3 V). 


e) V Clock Configuration spremenimo APB1 peripheral clock (MHz) na 16 MHz. (potrdite z ENTER) Kaj 
opazite? Ostale spremenljivke zraven se tudi spremenijo, npr. peripheral clocks.

f) V Configuration kliknemo ADC gumb. V Parameter settings izberite ločljivost pretvorbe na 8-bitno, torej 
je območje vrednosti od 0 ÷ 255. 


g) Clock Prescaler nastavimo z deliteljem 4. Kolikšna je sedaj preskalirana frekvenca takta fpreskalirana? 
Fpreslikana je 4MHz

i) Sampling time (čas vzorčenja tvz_ciklih) spremenite na 247.5 cikov (najdete pod Rank). 
Pravi čas vzorčenja se nato poveča še za 12 ciklov zaradi procesa samega. Koliko znaša pravi čas 
vzorčenja tvz v mikro sekundah?

(enačba: tvz = t'vz_ciklih / fpreskalriana)? 64,9μs

Komentar:

Potenciometer smo povezali z STM ploščico in z njegovo pomocjo izvedli neprekinjene ADC pretvorbe. V tabeli kjer so se nam izpisovale vrednosti sva naletela na edino težavo in sicer pod live expressions sva namesto adcValue napisala adcVal da nama je pravilno delovalo.

SLIKA PINOUT 
<img width="710" height="620" alt="Posnetek zaslona 2025-11-05 100631" src="https://github.com/user-attachments/assets/cba8c8f4-97a5-4bbd-b1d3-8326e68dd82e" />

SLIKA VEZJA
![Image](https://github.com/user-attachments/assets/79d7644b-adbb-483c-b47b-564ce0648815)






