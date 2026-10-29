# Instrukcje dla Antigravity / Gemini

Cały kontekst projektu **Pitaya Convert** (cel, zasady od właściciela, struktura, uruchamianie i wdrażanie, testowanie, znane ograniczenia) jest w pliku **`AGENTS.md`** w tym samym katalogu – przeczytaj go najpierw i traktuj jako obowiązujący.

Najważniejsze w skrócie:
- Electron; **silnik w czystym Node** (`engine.js`) z testami automatycznymi: `npm test`.
- Wykrywa działające kodery (NVENC, VAAPI, QSV, AMF, CPU) przez prawdziwą próbę; przy błędzie kodera sprzętowego przełącza się na CPU.
- Nie nadpisuje istniejących plików; konwersja da się przerwać (AbortSignal).
- Wszystko po polsku; wygląd matowy i spokojny, nie „AI slop”.
- Po każdej zmianie dopisz wpis w liście zmian: `node ~/Pitayas-Projects/ADMIN/changelog.js add <id> <feature|fix|change> "opis"`.
- Commity jako właściciel, **bez** „Co-Authored-By” i wzmianek o AI. Nie buduj ani nie publikuj wersji bez prośby.
- Nigdy nie kopiuj sekretów (hasła, tokeny, `.env`) do kodu, logów ani czatu. Napisz, czego nie mogłeś sprawdzić.
