# Przewodnik instalacji — Autodarts CORE (userscript)

Autodarts CORE to userscript dla **https://play.autodarts.com/**.
Instalujesz go za pomocą menedżera userscriptów (Violentmonkey / Tampermonkey), a potem aktualizuje się jak każdy inny skrypt.

---

## Zalecana instalacja (stabilna)

✅ **Użyj wersji DIST (stabilnej):**  
https://raw.githubusercontent.com/Zasadinho/Autodarts_wyglad/dart/autodarts-core.user.js

Dlaczego DIST?
- To jest **opublikowany** plik przeznaczony dla użytkowników końcowych.
- Sprawdzanie aktualizacji też powinno wskazywać na URL **DIST**, żeby użytkownicy zawsze dostawali stabilną wersję.

---

## Violentmonkey (Firefox)

1. Zainstaluj dodatek **Violentmonkey**.
2. Otwórz URL DIST w nowej karcie:  
   https://raw.githubusercontent.com/Zasadinho/Autodarts_wyglad/dart/autodarts-core.user.js
3. Violentmonkey pokaże stronę **Install** → kliknij **Install**.
4. Wejdź na Autodarts: https://play.autodarts.com/  
   Otwórz stronę meczu i naciśnij **Shift+F** (przełącznik panelu).

---

## Tampermonkey (Chrome)

Te same kroki:

1. Zainstaluj rozszerzenie **Tampermonkey**.
2. Otwórz URL DIST:  
   https://raw.githubusercontent.com/Zasadinho/Autodarts_wyglad/dart/autodarts-core.user.js
3. Kliknij **Install**.
4. Otwórz Autodarts i przetestuj **Shift+F**.

---

## Aktualizacje

- W Violentmonkey/Tampermonkey: otwórz skrypt → **Check for updates**.
- Albo włącz automatyczne aktualizacje w menedżerze (zalecane).

---

## Opcjonalnie: instalacja „bleeding edge” (dev)

⚠️ Tylko jeśli chcesz przetestować najnowsze zmiany przed wydaniem:

- SRC (źródło rozwojowe):  
  https://raw.githubusercontent.com/Zasadinho/Autodarts_wyglad/dart/autodarts-core.user.js

Uwaga: SRC może się zmienić w dowolnym momencie i może zawierać niedokończone eksperymenty.

---

## Rozwiązywanie problemów

### Widzę DWA zegary / DWA panele
To niemal zawsze oznacza, że **skrypt uruchamia się dwukrotnie**.

Sprawdź:
1. Menedżer userscriptów → czy masz zainstalowane **dwa skrypty Autodarts CORE**?  
   Wyłącz/usuń starszy.
2. Czy masz inny skrypt, który też dodaje zegar/panel?  
   Tymczasowo wyłącz inne skrypty Autodarts i odśwież stronę.
3. Wymuś odświeżenie strony:
   - Windows: **Ctrl + F5**
   - Albo zrestartuj przeglądarkę.

### Skórka/Layout wygląda źle po aktualizacji Autodarts
Aktualizacje interfejsu Autodarts mogą zmieniać nazwy klas Chakra „css-xxxxx”.
CORE ma wbudowaną **kontrolę poprawności selektorów** i może automatycznie wyłączyć Skin/Layout, jeśli wykryje niezgodność.
Jeśli tak się stanie:
- Zaktualizuj CORE do najnowszej wersji DIST
- Albo tymczasowo wyłącz Skin/Layout w panelu CORE

---

## Szybkie użycie

- **Shift+F**: przełącz panel CORE  
- **Shift+1 / Shift+2 / Shift+3**: presety A/B/C  
- **Shift+M**: przełącznik trybu bezpiecznego (Safe Mode)  
- **Shift+H**: pomoc  
- **Shift+T**: przełącznik zegara  
- **Shift+R**: reset zegara  
- **ESC**: zamknij panel