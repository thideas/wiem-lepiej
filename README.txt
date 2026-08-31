WIEM LEPIEJ — MVP

Co zawiera paczka:
- index.html — cała gra
- manifest.webmanifest — instalacja jako PWA
- sw.js — tryb offline po pierwszym wejściu
- icon.svg — ikona aplikacji

Najważniejsze:
Gra zapisuje się AUTOMATYCZNIE w localStorage przeglądarki po praktycznie każdej akcji.
Zamknięcie karty, Safari, przejście do ChatGPT albo restart telefonu nie powinny usuwać rozgrywki.
Po ponownym wejściu pojawi się przycisk „Kontynuuj grę”.

NAJPROSTSZE URUCHOMIENIE NA VERCEL:
1. Rozpakuj paczkę.
2. Utwórz nowe repozytorium GitHub i wrzuć do niego te 4 pliki.
3. W Vercel wybierz Add New > Project.
4. Zaimportuj repozytorium.
5. Framework Preset: Other.
6. Build Command: zostaw puste.
7. Output Directory: zostaw puste.
8. Deploy.

Możesz też użyć dowolnego hostingu statycznego, np. GitHub Pages, Netlify albo Cloudflare Pages.

IPHONE / PWA:
Po wejściu na opublikowaną stronę w Safari:
Udostępnij > Dodaj do ekranu początkowego.
Wtedy uruchamia się jak osobna aplikacja.

UWAGA:
Otwieranie index.html bezpośrednio jako plik file:// nie jest najlepszym sposobem na iPhone. Dla stabilnego localStorage, service workera i PWA użyj zwykłego hostingu HTTPS (np. Vercel).

Zapis gry jest lokalny dla konkretnej przeglądarki i domeny. Jeśli wejdziesz na inną domenę albo wyczyścisz dane Safari, zapis nie przejdzie automatycznie.
