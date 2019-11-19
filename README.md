# Libé Static Ressources

## General purpose

Home for all the static assets loaded in Libé Labo apps.

Home repo: https://github.com/libe-max/libe-static-ressources<br/>
Static ressources hosted at: https://www.liberation.fr/apps/static/

## Technologies

Mainly CSS and SVG

## Install, start & publish

#### Install

```bash
# Go to your favorite location
> cd /wherever/you/want/

# Clone libe-utils
> git clone https://github.com/libe-max/libe-static-ressources.git

# No dependencies, you're ready
```

#### Start

```bash
> cd /wherever/you/installed/libe-static-ressources/

# Start a local server running on port 3003
> npm start
```

#### Publish

```bash
> cd /wherever/you/installed/libe-static-ressources/

# Commit and push everything
> git add *
> git commit -m "some lowercase descriptive action text"
> git push origin master

# Update "version" field in package.json, according to the [semantic versionning](https://semver.org/) method.
> nano package.json

# Install dependencies again in order to update package-lock.json
> npm i

# Commit & push version change
> git add *
> git commit -m "v{MAJOR}.{MINOR}.{PATCH}"
> git push origin master

# Upload updated files to https://www.liberation.fr/apps/static
```

## Contents

```
libe-static-ressources
├── package.json
├── package-lock.json
├── assets/
├── fonts/
├── lib/
├── styles/
    ├── apps/
        ├── ...
    ├── apps.css
    ├── components.css
    ├── fonts.css
    ├── font-classes.css
    ├── liberation.css
    ├── text-levels.csv
```

| Path                      | Purpose                                                      |
| ------------------------- | ------------------------------------------------------------ |
| `/package.json`           | The ID card of the project                                   |
| `/package-lock.json`      | Don't touch this                                             |
| **`/assets/`**            | Icons, logos, etc, ...                                       |
| **`/fonts/`**             | All the fonts used by Libération                             |
| **`/lib/`**               | Reset.css, jQuery, leaflet, etc, ...                         |
| **`/styles/`**            | -                                                            |
| **`/styles/apps/`**       | App specific styles                                          |
| `/styles/liberation.css`  | Generic styles for Libération                                |
| `/styles/fonts.css`       | Font imports                                                 |
| `/styles/apps.css`        | Styles shared by every app (box-sizing, body margin, etc, ...)|
| `/styles/components.css`  | `libe-components` styles                                     |
| `/styles/font-classes.css`| Dirty helper to use font families and weight with no css (eg: \<p class="font-fam_libe-sans">Paragraph\</p>)|
| `/styles/text-levels.csv` | Explanation of how font-sizes and line-heights were calculated in `/styles/components.css`|

## Auteurs

- **Maxime Fabas** - _Rédaction_ - [maximefabas.github.io](https://maximefabas.github.io)

___
![Logo Libération](https://www.liberation.fr/apps/static/assets/liberation-logo_raster_64.png)       ![Logo Libé labo](https://www.liberation.fr/apps/static/assets/libe-labo-logo_raster_64.png)



