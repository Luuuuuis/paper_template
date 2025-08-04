# Wissenschaftliche Arbeiten Template DHBW

Das ist ein Template Repository für die wissenschaftlichen Arbeiten an der DHBW. 
Das Template ist komplett in LaTeX geschrieben und kann mit Overleaf oder lokal verwendet werden.
Als Zitierstil ist der IEEE-Style eingestellt, der in den technischen Studiengängen verwendet wird.
Die Sprache ist auf Deutsch eingestellt, kann aber leicht auf Englisch umgestellt werden.

## Run Local:

set in vs code settings.json "-shell-escape" for minted
```json
    "latex-workshop.latex.tools": [
        {
            "name": "latexmk",
            "command": "latexmk",
            "args": [
                "-shell-escape",
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-pdf",
                "-outdir=%OUTDIR%",
                "%DOC%"
            ],
            "env": {}
        },
```

Run "sudo apt-get install inkscape" for svg support
Run "sudo apt-get install python3-pygments" for minted support