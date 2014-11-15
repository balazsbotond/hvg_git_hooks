#HVG git hooks

Néhány git hook a HVG-s fejlesztés megkönnyítésére.

##prepare-commit-msg

Három dolgot csinál:

* Ha olyan branchen vagyunk, aminek számjegyekkel és utána kötőjelekkel kezdődik a neve, a commit message első sorába beteszi a hivatkozást a ticketre ("Card #9999")
* A git alapértelmezett működéséhez hasonlóan megjegyzésben beszúrja a `git diff` kimenetét
* Segíti, hogy a commit message minél részletesebb lehessen, azáltal, hogy beszúrja megjegyzésben a `git diff --cached` kimenetét is (eltérések az utolsó commit és az index között)
