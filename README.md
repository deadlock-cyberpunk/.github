# Cyberpunk Escape Room

## Opis projektu

Ten projekt to repozytorium zawierające oprogramowanie sterujące naszym pierwszym pokojem escape w stylu cyberpunkowym. Uczestnicy wcielają się w role, którzy na prośbę przyjaciela włamują się do siedziby korporacji tworzącej sztuczną inteligencję. Ich celem jest zniszczenie AI, zanim przejmie kontrolę nad światem.

## Struktura pokoju

Pokój składa się z dwóch głównych części:

1. **Biuro/Laboratorium:** Główna przestrzeń, która imituje miejsce pracy zbuntowanego pracownika korporacji (naszego przyjaciela), zawierająca wskazówki i narzędzia potrzebne do przejścia do kolejnej części.

2. **Serwerownia:** Ukryty pokój, do którego uczestnicy muszą się dostać. Tutaj znajdują się serwery AI, które należy zniszczyć, aby zakończyć grę.

## Technologie i zagadki

W repozytorium znajdują się skrypty i oprogramowanie sterujące różnymi elementami pokoju, w tym:

- Mechanizmy otwierające tajne przejścia
- Systemy kontroli światła i dźwięku
- Interaktywne zagadki zintegrowane z technologią

## Struktura repozytorium i nazewnictwo (**Stale aktualizowana**)
1. Każdy element pokoju, który da się wydzielić logicznie jest oddzielnym repozytorium w organizacji, przy czym rezpoytoria należy nazywać wykorzystując konwencję **kebab-case** oraz korzystając z następujących prefixów: 

Prefix 1:
  - **puzzles-** - Domunetacja i kody źródłowe poszczególnych zagadek.
  - **control-** - Skrypty kontrolne do zarządzania elementami pokoju, takimi jak oświetlenie, muzyka oraz pełny flow pokoju.
  - **server-** - Komponenty serwerowe aplikacji.
  - **tests-** - Zawiera testy do kodu źródłowego
  - **assets-** - Zawiera zasoby, takie jak pliki audio czy grafiki używane w pokojach, które nie są częścią zagadki
    - **audio-** - Dźwięki wykorzystywane w pokoju.
    - **images-** - Obrazy i grafiki.
  - **models-** - modele 3d elementów pokoju, które nie są częścią zagadki

Prefix 2:
 - **p1/p2/...-** - Określa fazę rozgrywki, której dotyczy repozytorium (**all** jeśli repozytorium dotyczy całego pokoju)

Nazwa główna - następuje po podwójnym myślniku **--**
- **control-flow** - nazwa danej zagadki, w tym przypadku control-flow

Przykładowo, dla zagadki **control-flow**, która znajduje się w fazie 2:
- **puzzles-p2--control-flow**
