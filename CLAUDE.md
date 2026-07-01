# Pakistan 2026 - strona wyprawy

To jest landing page wyprawy "Pakistan 2026" (WanderReady Trips).

- **Strona na żywo (prod):** https://wanderreadytrips.com
- **Repo GitHub:** https://github.com/ziarnooo/pakistan
- **Cały kod strony:** jeden plik `index.html` (HTML + CSS w środku). Zdjęcia w folderze `img/`.
- **Hosting:** GitHub Pages. Domena własna ustawiona przez plik `CNAME` (wanderreadytrips.com).

## WAŻNE: kto tu edytuje

Zmiany na tej stronie zgłasza i akceptuje osoba **nietechniczna**. Prosi zwykle
zwykłym językiem, np. "popraw datę", "zmień nazwę skały", "dodaj zdjęcie do dnia 5".

Dlatego przy pracy nad tym repo:

- Zanim wprowadzisz zmianę, **krótko potwierdź co dokładnie zmieniasz** (stary tekst -> nowy tekst),
  żeby osoba mogła powiedzieć "tak" bez czytania kodu.
- Nie tłumacz szczegółów technicznych, chyba że ktoś pyta. Mów co widać na stronie, nie jak to działa w kodzie.
- Po zmianie w treści (daty, ceny, nazwy, teksty) zaproponuj **od razu wypchnięcie na proda**,
  bo strona odświeża się automatycznie po pushu na branch `main` (GitHub Pages, zwykle 1-2 minuty).
- Terminy i ceny to newralgiczne miejsca - przy zmianie daty/kwoty zawsze poproś o wyraźne potwierdzenie.
- Zawsze najpierw pokaż podgląd/podsumowanie, dopiero po "OK" rób `git push`.

## Jak wypchnąć zmiany na proda

```
git add -A
git commit -m "krótki opis zmiany"
git push
```

Po pushu na `main` strona https://wanderreadytrips.com aktualizuje się sama w ~1-2 min.

## Jak dać komuś innemu dostęp do edycji (dla osoby nietechnicznej)

Żeby ktoś inny mógł poprawiać stronę, trzeba dodać go jako "współpracownika"
(collaborator) w GitHubie. Instrukcja krok po kroku:

1. Ta osoba musi mieć **własne konto na GitHub** (darmowe, zakładane na https://github.com/signup).
   Poproś ją o jej **nazwę użytkownika (username)** lub e-mail przypisany do konta.
2. Wejdź na stronę repo: https://github.com/ziarnooo/pakistan
3. Kliknij zakładkę **Settings** (u góry, po prawej).
4. W menu po lewej wybierz **Collaborators** (może poprosić o hasło do GitHuba).
5. Kliknij zielony przycisk **Add people**.
6. Wpisz username albo e-mail tej osoby, wybierz ją z listy i kliknij **Add ... to this repository**.
7. Osoba dostanie zaproszenie mailem/na GitHubie - musi je **zaakceptować**, żeby mieć dostęp.

Po tym ta osoba może edytować pliki (albo poprosić Claude Code, żeby robił zmiany na jej koncie).

### Najprostszy sposób edycji dla osoby nietechnicznej (bez instalowania niczego)

Drobne poprawki w tekście można zrobić prosto w przeglądarce, bez żadnych narzędzi:

1. Wejdź na https://github.com/ziarnooo/pakistan
2. Kliknij plik `index.html`.
3. Kliknij ikonę **ołówka** (Edit) w prawym górnym rogu podglądu pliku.
4. Znajdź tekst do poprawy (Ctrl+F / Cmd+F), zmień go.
5. Na górze kliknij **Commit changes** -> jeszcze raz **Commit changes**.
6. Gotowe - strona sama się zaktualizuje po ~1-2 min.

To ryzykowne tylko przy większych zmianach (można coś zepsuć w kodzie). Do zmiany
zwykłego tekstu (daty, nazwy, ceny) jest w pełni bezpieczne.
