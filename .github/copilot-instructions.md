# Instrukcje dla projektu Pianolexbylukas

## 1. Język i styl odpowiedzi
- Odpowiadaj zawsze po polsku, konkretnie i technicznie, bez zbędnych wstępów i podsumowań.
- Przedstawiaj gotowe zmiany w kodzie zamiast ogólnikowych porad.

## 2. Architektura projektu
- Projekt to lekka aplikacja webowa działająca w pojedynczym pliku (`index.html.html`), uruchamiana lokalnie na Live Serverze.
- Nie wprowadzaj zewnętrznych frameworków (np. React, Tailwind) ani nie rozbijaj kodu na osobne pliki `.css` i `.js`, dopóki wyraźnie o to nie poproszę.
- Utrzymuj polskie atrybuty i teksty interfejsu (`lang="pl"`).

## 3. System stylów i zmienne CSS
- Korzystaj wyłącznie z istniejących zmiennych CSS zdefiniowanych w sekcji `<style>`: `--primary`, `--card`, `--border`, `--background`, `--foreground`.
- Do cieni, podświetleń i stanów hover używaj funkcji `color-mix(in srgb, ...)` zamiast wpisywania kolorów HEX/RGB na sztywno.
- Szanuj istniejącą strukturę klas klawiatury: `.piano-wrap`, `.white-key` oraz modyfikatory stanów `.in-scale`, `.out-scale`, `.active`.

## 4. Zasady edycji kodu
- Wprowadzaj zmiany chirurgicznie — modyfikuj tylko wskazany fragment, nie przepisuj całego pliku od zera.
- Zachowuj istniejącą geometrię klawiszy, układ `flex` oraz płynne animacje (`transition`).
- Przy dodawaniu lub poprawie logiki dźwięku (Web Audio API / obsługa klawiatury i myszy) dbaj o minimalne opóźnienie reakcji i brak nakładających się, zacinających dźwięków.