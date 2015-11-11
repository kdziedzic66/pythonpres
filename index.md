---
title       : Wprowadzenie do Pythona
subtitle    : 
author      : 
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---
Apache Spark to narzedzie do pracy z Big Data. Posiada bardzo przejrzyste API do pracy z danymi z poziomu kodu (Java,Scala,R,Python). Pozwala na szybka prace z danymi ( dane nie s¹ za kazdym razem zapisywane na dysk jak w MapReduce, tylko mozemy cachowac je w pamieci co pozwala na zwiekszenie nawet 100x szybkosci algorytmow ). W szczegolnosci roznica ta jest istotna w pracy z algorytmami iteracyjnymi, m. in. machine learning. MapReduce w ka¿dym kroku iteracji zapisuje dane na dysk i czyta z niego, podczas gdy Spark czyta z pamieci. Python jest bardzo prostym jezykiem o ladnej i przejrzystej skladni, dzieki czemu mamy mozliwosc pracy z danymi wedlug jednego, okreslonego wzorca bez koniecznosci uczenia sie wielu narzedzi nale¿¹cych do ecosystemu Hadoopa.


--- .class #id 
<iframe width="560" height="315" src="https://www.youtube.com/embed/SxAxAhn-BDU?autoplay=1"></iframe>

--- .class #id

# Instalacja Pythona

Jak wiadomo przygode z Pythonem nalezaloby rozpoczac od instalacji tegoz Pythona. Zrodlo z ktorego mozemy pobrac i zainstalowac tegoz Pythona, to www.python.org/downloads. Wybieramy wersje - 3.5 lub 2.7. istnieje pewna roznica pomiedzy Pythonem 2 i 3 - sporo bibliotek Pythonowych nie jest jeszcze kompatybilna z Pythonem 3.5. Nastepny krok to wybor i instalacja IDE (integrated development environment). W trakcie warsztatow bedziemy uzywac PyCharm, ktore mozemy pobrac z https://www.jetbrains.com/pycharm/?fromMenu. 

--- .class #id

# Podstawy skladni jezyka

Jezyk dynamicznie typowany w trakcie deklaracji zmiennej nie okreslamy jej typu, typ zostaje przydzielony w trakcie wykonywania programu. Na koncu linijki nie stawiamy srednika. Instrukcje ktore maja byc wykonywane wewnatrz petli, instrukcji warunkowej badz bloku try/except (za chwile wyjasnimy co znacza te pojecia :)) sa odzielone czterema spacjami wewnatrz instrukcji. 

# Przyklad 1:

Wprowadzamy dwie liczby z klawiatury. Zwroc sume, iloczyn i iloraz.

# Przyklad 2:

Wprowadzamy liczbe z klawiatury. Zwroc pierwiastek z liczby.

# Przyklad 3:

Wprowadz dwie liczby z klawiatury, jesli druga z nich jest rowna 0 wyswietl "jasna cholero nie dziel przez 0", jesli jest rozna od 0 zwroc iloraz.

# Przyklad 4:

Wiadomo, ze $\frac{\pi}{4}=arctg(1)$. Przypomnijmy, ze $\operatorname{arctg} x = \sum^{\infty}_{n=0} \frac{(-1)^n}{2n+1} x^{2n+1},\; |x| \leq 1$. Wyswietl przyblizenie liczby pi.

--- .class #id

# Przyklad 5:

Rozwiaz poprzednie zadanie jako funkcje zmiennej n, okreslajacej liczbe iteracji petli.

# Przyklad 6:

Definiujemy slownik glupoty: przypisujemy roznym wyrazom pewne wartosci i w zaleznosci od tego ile tych wyrazow jest w zdaniu dodajemy do zdania wartosc jego glupoty. Napisz funkcje, ktora dla danego zdania zwroci wartosc jego glupoty.

# Przyklad 7:

Napisz funkcje, ktora dla danego stringa zwroci True jesli reprezentuje on wartosc numeryczna, a w przeciwnym wypadku zwroci False.

# Przyklad 8:

Napisz funkcje, ktora dla danego stringa usunie z niego wszystkie znaki, ktore nie sa alfanumeryczne.

--- .class #id

# Przyklad 9:

Wordcount w Spark

# Przyklad 10:

Napisz funkcje, ktora dla danego tekstu wczytanego z pliku tekstowego zwróci s³ownik zawieraj¹ce pary klucz-wartoœæ, gdzie kluczami s¹ wyrazy, a wartoœciami term frequency danego wyrazu.

# Przyklad 11:

Posortuj przyklady z wczesniejszego zadania po wartosci.

# Przyklad 12:

Napisz funkcje, ktora poisson(n,lambd), ktora wygeneruje probe o dlugosci n z rozkladu Poissona z parametrem lambd.

# Przyklad 13:

Napisz funkcje integral(a,b,f), ktora obliczy przyblizona wartosc $\int_a^bf(x)dx$ dla danej ciaglej funkcji f.








