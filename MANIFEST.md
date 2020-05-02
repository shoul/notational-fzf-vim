# NV Manifest

Notitzen teile ich in drei Kategorien:

1. Projektnotizen
    Hier ändern sich die Sichtweisen, Anforderungen und Wünsche mit der
    Entwicklung des Projekts. Für diese Notitzen möchte ich ein Datum im
    Dateinamen um den Verlauf und die Entwicklung des Projets nachvollziebar zu
    machen.
2. Werkzeugnotizen (Werkzeuge meint hier auch Progammiersprachen und Frameworks.)
    Die änderungen der Anforderungen und Benutzerschnittstellen sind in aller
    Regel mit Versionen verbunden. Hier möchte ich den Namen des Werkzeugs als
    Dateinamen. In den Notitzen zu dem Werkzeug möchte ich wenn notwendig einen
    Versionshinweis.
3. Todos
    Sie möchte ich möglichst übersichtlich und nach Liste getrennt.


## Namensräume


### Datum


### Trennzeichen für Dateinamen


## Lösungsansätze


### Ordnerstruktur - Jedes Ding hat seinen eigenen Ordner

* Projektnotizen werden für jedes Projekt separat und in jedem Projekt an gleicher Stelle angeordnet.
* Todos werden ebenso wie Projektnotizen für jedes Projekt separat und in dem jeweilgien Projekt geführt.

    Projekt:
        - notizen:
            20200422_projektbeschreibung.md
            20200502_neue_ide.md
        - todo.md
        
* Werkzeugnotitzen haben einen eigenen Ordner

    Werkzeugnotizen:
        - vim.md
        - django.md


### Tags

* Alle Notizen sind in einem Ordner, ohne Unterordner auf einer Ebene.
* Alle Einträge haben Schlagworte und können über diese gefunden werden.

Der Ansatz ist bestechend einfach. Listen für die Projekte können aus dieser Sammlung einfach generiert werden:

    find ~/nv -type f -name 'vim' | xargs cat > ~/tp/vimnotes.md

