---
title: "Drugie spotkanie
"
meta_title: ""
description: "meta description"
date: 2025-02-22T05:00:00Z
image: "/images/posts/tor2.png"
categories: ["programming"]
authors: ["Świderki"]
tags: ["motorola"]
draft: false
---

Po feriach wreszcie udało nam się zgrać i znowu spotkać się na miejscu w naszej ulubionej kawiarni. Było to pierwsze spotkanie na żywo w tej edycji, na którym pojawili się wszyscy członkowie zespołu.
Omówiliśmy co udało się zrobić - wstępna architektura kodu zaimplementowana na repozytoriu na githubie, skrypt do zamieniania modeli 3D samochodów na tzw. sprite-y i już pierwsze jeżdżące po ekranie autko!

Pojawiły się problemy na przykład z tym, że nasze auto jeździło jak po lodowisku, co wynikało ze źle dobranej siły tarcia.

<video width="320" height="240" controls>
  <source src="/images/posts/lodowisko.mp4" type="video/mp4">
  Twój przeglądarka nie wspiera tego formatu wideo.
</video>

![alt text](/images/posts/feature1.png)

Podjęliśmy także bardzo ważną decyzję o tym w jaki sposób będziemy zapisywali w pamięci tor wyścigowy: będzie to tablica 2D w której każda komórka reprezentuje pixel naszego toru i jej wartość decyduje o tym czy należy ten piksel do toru, czy do bandy. To jest dobre rozwiązanie jeśli chodzi o kosztowność obliczeniową, bo wymaga tylko odczytania wartości pól w tablicy by sprawdzić czy nastąpiła kolizja. Wydaje się mieć sens? Otóż wtedy jeszcze nie zastanawialiśmy się nad tym, w jaki sposób będziemy liczyć kąt odbicia! (alternatywą było użycie krzywych beziera, które mają gotowe rozwiązania do obliczania pochodnej w punkcie na podstawie której można by liczyć kąt odbicia, ale uznaliśmy, że tablica 2D jest prostsza w implementacji i dużo szybsza). W jaki sposób rozwiązaliśmy ten problem? Czy musieliśmy pisać potem cały nasz kod od nowa? Tego dowiecie się w kolejnym akapicie! 🙂

![alt text](/images/posts/tor1.png)

![alt text](/images/posts/tor2.png)

Rozpoczęliśmy także (jak się potem potem najtrudniejszy i najdłuższy ) proces prac nad przeciwnikami.
