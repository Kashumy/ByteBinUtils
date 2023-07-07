_____
# BshBin
_____

BshBin jest językiem, który posiada grafikę.

```bash
in [funkcja] [
# zawartość funkcji
]
```
^ Oto składnia funkcji. Jeśli chcesz ją wykonać, użyj:

```bash
[funkcja] out
```

--------

# Jak wstawić grafikę?

W BshBIN masz wiele możliwości wstawiania grafiki. Na przykład:

```bash
Line(x1,y1,x2,y2)
```
^ Ta komenda narysuje linię od pozycji (x1, y1) do pozycji (x2, y2), gdzie wartości mogą być dostosowane przez użytkownika.

# Kostka

Aby narysować kostkę, wpisz:

```bash
Box(x1,y1,x2,y2,BshCOLOR)
```
^ Pamiętaj, że x1, x2, y1, y2 i BshCOLOR mogą być przez Ciebie dostosowane.

Niestety, Bsh posiada własną paletę kolorów, więc może być trudno dobrać odpowiedni kolor. Maksymalna wartość koloru to 255.

# Koło

Aby wstawić prostokątne koło, wpisz:

```bash
Circle(0,0,50,50,101)
```
To powinno wstawić fioletowe koło. Liczba 101 odpowiada kolorowi fioletowemu.

# Jak używać @USING?

@USING to komenda, która pozwala na użycie wbudowanych funkcji w BshBIN. Lista dostępnych @USING'ów zostanie wyświetlona po wpisaniu:

```bash
@USING <help>
```
Ten @USING pozwoli wyświetlić listę dostępnych @USING'ów.

## @USING <bsh/void>

Ten @USING pozwala na utworzenie czystego projektu działającego poza konsolą oraz eliminuje początkowe wyjście i dodaje nowe komendy.

## @USING <end>

Ten @USING usuwa napis "exit code 0; end" w przypadku, gdy program zakończy działanie poprawnie. Jednak możesz go również ukryć, używając komendy:

```bash
Print("")
```

Poza tym, komenda Print służy do wyświetlania tekstu na ekranie.

```bash
Print("x1")
```

"X1" to dowolny tekst wprowadzony przez Ciebie.

# Responsywność :O

Jeśli chcesz umieścić figurę, która będzie miała rozmiar 100x100 na całym ekranie i nie będzie wychodzić poza ekran na innych urządzeniach, wystarczy dodać przed komendą np.

```bash
Box
```
prefiks "r/":

```bash
rBox
```

---

## Moje pomysły dotyczące BshBIN:

1. Wprowadzenie funkcji do rysowania elips.
2. Dodanie możliwości zapisu grafiki do pliku.
3. Implementacja animacji, aby umożliwić tworzenie prostych ruchomych obrazów.

4. Dodanie funkcji do rysowania trójwymiarowych obiektów.
5. 
5. Wprowadzenie możliwości dodawania gradientów kolorów do figur.
6. Umożliwienie rysowania tekstu o różnych stylach i czcionkach.
7. Dodanie funkcji do obsługi dźwięku w BshBIN.
8. Wprowadzenie interaktywnych elementów, takich jak przyciski, pola tekstowe, itp.
9. Implementacja funkcji do manipulacji obrazami, takich jak skalowanie, przycinanie, obracanie, itp.
10. Dodanie wbudowanych efektów wizualnych, takich jak rozmycie, cieniowanie, itp.






--------


# zeczy które napewno się pojawią
````
Input(option)
````
option = /wartość/zmiennej/opcji
````
on (arg [operand] num/string ){
 # [some commands]
}
````
działa tak że jeżeli np a==20
to wykona coś np Print("hi")

## można to połączyć z inputem
````
Input(arg) > function
in function [
 on (arg == 1){
  Print("This is one !")
 }
]
````
to spowoduje że jeżeli Urzytkownik wpisze 1 to pojawi się napis This is one !

# Input 
aby skonfigurować ontouch dla inputa urzyj
````
@USING <input/ot>
````
wtedy pojawi się kustomowa klawiatura w pliku keyboard 
którego będziesz mieć wraz z resztą zasobów w folderze BIN/file/scr
mozesz zmienić jej plik 

keyboard-config

tlo klawiatury

## Keyboard-Color : shCOLOR ;

tlo przycisków

## Key-Color : shCOLOR ;

podswietlenie

## Active-Key-Color : shCOLOR ;

outline przycisków

## Key-outline : shCOLOR ;




# Nowe funkcje w przyszłości 

- dodano możliwość robienia pentli poprzez 

````
in a [

a out
]
````
^ ~~ petla overflow 

lub &
````
loop:1t[

]
````
^ ~~ pętla 1t na sekundę 

````
[funkcja] js-out
````
^ ~~ wykonuje funkcje w js

````
insect [funkcja] -(
 # zawartość 
)-
````
^ ~~ to funkcja ktura może być wykonana poprzez zmienna gdy zmienna funkci zostanie zmieniona takasama co nazwa funkcji zostanie zmieniona na true


## USING landscape 
powoduje zmienienie orietacji urządzenia na landscape 
````
@USING <landscape>
````

## zmiana Ikonki Ekranu startowego
wpisz 
````
edit config += 'scr:/path'
````
/path to scierzka do obrazu

___
# WARZNE
- ` aby wstawić Trujkata wpisz `
````
Trg(x1,y1,x2,y2,shCOLOR,deg)
````
deg to kont na chylenia
- ` wstawianie tekstu jest poprzez komende Print`
````
Print("HelloWorld")
````
___

# O Byte shell

byteshell to program graficzny który jest programem eksperymentalnym więc urzywanie go jeszcze 
jest w fazie testowej

__________
__________
__________

# Pomysły 
__________
__________
- `petle`
- `warunki`
- `zmienne operatory += -= = *= /=`
- `Printf wyswietlanie terazniejszej wartości zmiennej`
- `@USING <fs> pozwala włączyć fullscreen `
- `Title["tytuł strony"]`
- ``
__________
