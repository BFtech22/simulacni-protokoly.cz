# simulacni-protokoly.cz

Doména jen přesměrovává na **https://www.simulacni-zkousky.cz/proces-pripojeni.html**
(web je v repozitáři `BFtech22/simulacni-zkousky.cz`). Vlastní obsah tu záměrně není —
Search Console k 23. 10. 2026 ukazovala na dotazy se slovem „protokol“ nula zobrazení,
takže samostatný web by obsluhoval poptávku, která neexistuje. Doména drží značku.

- `index.html` pošle titulní stránku na Postup připojení, kde jsou doklady a protokoly;
  jakoukoli jinou cestu zachová. `404.html` dělá totéž. Bez JavaScriptu zabere meta refresh.
- `noindex` — stránka nemá soutěžit s hlavním webem ve vyhledávání.
- `CNAME` je `simulacni-protokoly.cz`. DNS u Webglobe stejné jako u hlavní domény:
  A na GitHub Pages (185.199.108–111.153), `www` jako CNAME na `bftech22.github.io`.
- Přesměrování přímo od Webglobe se nepoužilo — bez hostingu umí jen http.
