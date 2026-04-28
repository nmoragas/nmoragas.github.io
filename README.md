# Núria Moragas — Portfolio Web

Portfolio personal creat amb [Quarto](https://quarto.org) i publicat via GitHub Pages.

## Estructura 

```
portfolio/
├── _quarto.yml          ← Configuració global
├── index.qmd            ← Pàgina d'inici
├── research.qmd         ← Recerca i projectes
├── publications.qmd     ← Publicacions
├── cv.qmd               ← Currículum vitae
├── custom.scss          ← Tema visual
├── styles.css           ← Estils addicionals
├── assets/
│   ├── photo.jpg        
│   └── Moragas_Nuria_CV.pdf  
└── docs/                ← Output HTML (generat per Quarto)
```

## Configuració entorn (servidor HPC)

```bash
module load apps/python/3.12.3
export QUARTO_PYTHON=/share/apps/common/python/3.12.3/bin/python3
```

## Renderitzar

```bash
quarto render
```

## Preview local

```bash
quarto preview --no-browser --no-watch-inputs
```

## Publicar a GitHub Pages

```bash
git add .
git commit -m "Update portfolio"
git push
```

A GitHub: **Settings → Pages → Source: main /docs**

