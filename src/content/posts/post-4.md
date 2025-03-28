---
title: "Trzecie spotkanie
"
meta_title: ""
description: "meta description"
date: 2025-02-21T05:00:00Z
image: "/images/posts/menupomysl.png"
categories: ["programming"]
authors: ["Świderki"]
tags: ["motorola"]
draft: false
---

Problem z liczeniem kąta odbicia od krawędzi toru wyszedł na jaw.😮 Skłoniło nas to do rozpoczęcia dyskusji co dalej? Czy jesteśmy w stanie w jakiś sposób liczyć ten kąt odbicia? Może powinniśmy po prostu odbijać przeciwnika w kierunku przeciwnym do tego z którego uderzył on w ścianę? Niestety wyglądało to bardzo surrealistycznie jak go po prostu wyrzucało do tyłu od uderzenia pod płaskim kątem i wiedzieliśmy, że nie możemy tego tak zostawić. Niespodziewanie pojawił się bardzo ciekawy pomysł - użycie Regresji Liniowej do aproksymowania prostej prostopadłej do toru . Regresja Liniowa to algorytm (albo w przypadku danych punktów z przestrzeni 2D po prostu zwykły wzór) który pozwala znaleźć linię najlepiej “pasującą” do danych punktów w przestrzeni. My wrzucalibyśmy w taką regresję najbliższe do samochodu punkty 2D będące punktami bandy i potem liczyli kąt odbicia na podstawie wyjścia z funkcji. Pomysł został przyjęty i potem okazało się, że rzeczywiście to działa! Nie musimy przepisywać całego kod!

Dodatkowo do spotkania podzieliliśmy kod na sceny i w ten sposób obciążyliśmy plik game.ts czyniąc całą strukturę kodu prostszą i bardziej klarowną.

Podjęliśmy także parę innych decyzji jak np. stosowanie Separating Axis Theorem do sprawdzania kolizji pomiędzy obiektami (gracz, przeciwnicy i przeszkody) oraz korzystając z zeszłorocznych (niedobrych) doświadczeń związanych z pisaniem własnego UI (ang. User Interface), wymyslając róne pomysły jak mógłby wyglądać ekran główny postanowiliśmy tym razem nie wymyślać koła na nowo i po prostu skorzystać z gotowych komponentów HTML.

![alt text](/images/posts/menupomysl.png)

Poza tym dalej kontynuowaliśmy prace nad przeciwnikami, którzy już w miare sensownie trzymają się toru (na razie w zasadzie jest tylko jeden - jadący środkiem toru, ale już w miarę sensownie).
