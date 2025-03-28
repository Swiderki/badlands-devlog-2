---
title: "Pierwsze spotkanie - omówienie koncepcji
"
meta_title: ""
description: "meta description"
date: 2025-02-01T05:00:00Z
image: "/images/posts/kawa1.jpg"
categories: ["programming"]
authors: ["Świderki"]
tags: ["motorola"]
draft: false
---

Jak tylko zostały ogłoszone zadania, razem z zespołem (prawie identycznym jak w zeszłym roku - zamiast Michała nowym członkiem został Bartosz Trojan) postanowiliśmy spotkać się na żywo tam gdzie spotykaliśmy się w zeszłym roku, by omówić każde z nich i podjąć tą najważniejszą w tym konkursie decyzję: które z nich będziemy robić?
Zgranie się czasowo nie było proste i ostatecznie nie wszyscy pojawili się na spotkaniu. Jedno z zadań od razu odrzuciliśmy ze względu na to że było najmniej punktowane, oraz nie pokrywało się za bardzo z naszymi zainteresowaniami. Były to “Mosty”.

Zostały nam zatem dwie opcje: “Szachy” - bardziej spokojne oraz wymagające implementacji kompleksowych algorytmów, oraz “Wyścigi” - dynamiczne, zmieniające się w każdej sekundzie działania programu, w których implementacja przeciwników także nie należy do najprostszych. Wywiązała się burzliwa dyskusja w której padło wiele ciekawych argumentów. Ostatecznym zwycięzcą zostały “Wyścigi”!

Dlaczego? Implementacja “Wyścigów” wydała nam się być dużo większym wyzwaniem. Bez gotowego silnika do gier jak np. Unity rzeczy trywialne takie jak np. detekcja kolizji, płynne przemieszczanie się po ekranie, czy detekcja i omijanie przeszkód stają dużymi problemami wymagającymi przemyślenia i rozplanowania. Z tego powodu już w trakcie wybierania tematu pojawiały się pierwsze problemy i propozycje ich rozwiązania.

Od początku wiedzieliśmy, że technologią którą wybierzemy będzie TypeScript, ponieważ wszyscy członkowie naszego zespołu znają ten język i doskonale sobie z nim radzą. Zasięgneliśmy także do naszej tier listy języków programowania.

![alt text](/images/posts/tierlista1.png)

Natomiast sposób zarządzania pracą w zespole nie były już takie oczywiste. Jeden z członków zaproponował Trello - aplikacja gdzie zarządza się pracą z pomocą tzw. kanban board-ów czyli tablic z karteczkami które można pomiędzy nimi przerzucać. Bardzo nam się spodobał ten pomysł i postanowiliśmy, że tak zrobimy.
Dalej zdecydowaliśmy się wypisać wszystkie rzeczy, które musimy zrobić w aplikacji i na ich podstawie rozrysować sobie docelową architekturę aplikacji. (Patrz obrazki).

![alt text](/images/posts/rozpiska1.jpg)

![alt text](/images/posts/rozpiska2.jpg)

Będzie ona podzielona na sceny, a główna logika gry będzie w pliku game.ts w którym połączymy DisplayDriver. odpowiedzialny z renderowanie obrazy, PhysicsDirver odpowiedzialny za obsługę fizyki w grze, oraz PlayerController i OpponentController-y odpowiedzialne za gracza i przeciwników.
Później gdy spotkanie dobiegało już końca ustawiliśmy pierwsze zadania, które wpisaliśmy już na Trello i przypisaliśmy do odpowiednich osób. Tak oto rozpoczęliśmy naszą przygodę z tegoroczną edycją konkursu Motorola Science Cup.
