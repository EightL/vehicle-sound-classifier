# ISS Project 

**Author:** Martin Ševčík (xsevcim00)

The project is an assignment for ISS 2024/25 titled "Podle hlasu poznáte je ..." that focuses on audio signal processing. It involves:

# Specification

## Úvod

Člověk je podle zvuku schopen poznat zdroj tohoto zvuku. Rozeznáme kytaru od piana, saxofonu nebo varhan. Bezpečně rozeznáme zvuk, který vydává pes, od zvuku, který vydává kočka. Majitelé psů rozeznají štěkot svého psa od psů jiných, milovníci zpěvného ptactva rozeznají druh zpěváčka podle jeho zpěvu. Poznáme zvuk nákladního auta od auta osobního. Své přátele poznáme podle jejich hlasu. Slyšíme rozdíl ve zvucích a dokážeme je přiřadit k jejich zdroji nebo jeden ke druhému.

A když má takové schopnosti pomalý a nedokonalý biologický člověk se svým uchem, jistě to nebude žádný problém pro nekonečněkrát rychlejší a přesnější počítač vybavený kvalitními senzory... No, tak daleko nepůjdeme, kvalitní senzory a nahrávání zvuku jsme oddělili od zpracování, takže nebudete muset pobíhat po Brně a nahrávat nejrůznější zvuky. Připravili jsme pro Vás zvuky motorů několika modelů aut na různých otáčkách.

## Data a cíl řešení

Pro každého je připravena unikátní sada osmi nahrávek. Nahrávky jsou dostupné na:
  
https://www.fit.vut.cz/study/course/ISS/public/proj2024-25/personal/login.zip  
*(za "login" doplňte Váš login)*

- Nahrávky jsou ve formátu WAV.
- Vzorkovací frekvence je 16 kHz (informace je také obsažena v hlavičce WAV souboru).
- Každá nahrávka obsahuje 1 sekundu zvuku motoru auta.
- Mikrofon je pro všechna auta umístěn přibližně na stejném místě.

Máte k dispozici nahrávky zvuku motoru čtyř známých aut na konstantních otáčkách. Další čtyři nahrávky jsou smíchané a jejich původ je neznámý. Víme pouze, že pocházejí od stejných aut, ale motor běží na různých otáčkách. Je také možné, že jedna nahrávka nepatří k žádnému ze čtyř známých aut.

**Cíl:**  
Tyto čtyři nahrávky máte automaticky přiřadit ke známým nahrávkám, nebo určit, že daná nahrávka nepatří k žádnému ze známých aut.

## Způsob vypracování

Projekt je možné řešit v jakémkoli z následujících programovacích/scriptingových jazyků:
- Python Notebook
- Matlab
- Octave
- Julia
- C
- Java
- nebo v jiném libovolném jazyce

Můžete využít libovolné knihovny. Program se nezaměřuje na „krásu programování“; není tedy nutné mít vše ideálně zabalené do funkcí. Doporučuje se program komentovat tak, aby byl snadno pochopitelný pro kontrolující osobu.

*Podmínkou* je, aby Váš program byl spustitelný na Google Colab nebo na standardní fakultní distribuci Windows či Linux.

## Doporučený postup řešení

1. **Analýza**  
   Poslechněte si a "podívejte" se na Vaše signály. Vašimi signály jsou v podstatě šumy, takže promyslete, co to pro zpracování signálu znamená.

2. **Reprezentace signálu**  
   Zvolte vhodnou reprezentaci signálu, ve které budete schopni odlišné signály oddělit a podobné budou co nejvíce shodné.

3. **Metrika**  
   Podle zvolené metriky rozhodněte, které dva signály patří k sobě. Vzdálenost mezi reprezentacemi známých signálů by měla být dostatečně velká, zatímco signálům, které patří k sobě, musí metrika přiřadit menší vzdálenost.

4. **Přiřazení**  
   Na základě vypočítaných vzdáleností přiřaďte zvuk motoru neznámého původu ke zvuku známého původu.

V protokolu uveďte, co Vás vedlo k Vaší volbě, jakých zdrojů jste využili, a jakých výsledků jste dosáhli. Nezapomeňte zdokumentovat i postupy, které nevedly k žádanému cíli.

## Odevzdání

Termín odevzdání je první pondělí po konci semestru - **16.12.2024, 23:59**.  
Projekt se odevzdává prostřednictvím informačního systému.

Odevzdání sestává ze dvou souborů:

1. **Protokol**, ve kterém popíšete:
   - Vaše jméno a login na začátku
   - Odůvodnění zvoleného řešení a popis implementace
   - Přehled případných problémů a jejich řešení
   - K jakým výsledkům jste došli  
     
   Protokol musí obsahovat doprovodné obrázky nebo grafy (pokud využijete zdroje, které nevyrábí Váš program, je nutné je správně citovat).  
   Pokud pracujete v Python Notebooku, tvořte protokol rovnou textovými poli v notebooku, nikoli pouze komentáři v kódu. Protokol bude ve formátu PDF.  
   Soubor s protokolem prosím pojmenujte jako `login.pdf` (pro české či slovenské řešení) nebo `login_e.pdf` (pro anglickou verzi).

2. **Program**, kterým jste projekt řešili:
   - Program bude přehledný, konzistentně pojmenovaný a rozumně komentovaný.
   - Program bude vypisovat hodnoty a produkovat obrázky, které uvedete v protokolu.
   - Pokud je program ve formě Python Notebooku na Google Colab, odevzdáte pouze textový soubor s jedním řádkem obsahujícím URL vašeho notebooku. Notebook musí být čitelný a spustitelný.
   - Pokud je program rozdělen do více souborů, nebo pokud poskytnete návod ke spuštění v souboru README.txt, všechny části zabalte do jednoho ZIP souboru.

## Dotazy

Dotazy budou řešeny prostřednictvím diskuzního fóra na kartě předmětu. Automatické odebírání příspěvků znamená, že by měly být příspěvky viditelné pro všechny.

