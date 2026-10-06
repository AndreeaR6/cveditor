# cveditor

Editor de CV intr-un singur fisier HTML, fara server. Deschizi `index.html` in browser.

- Editezi textul pe sectiuni, vezi previzualizarea si descarci PDF-ul.
- **Salveaza ca JSON** pastreaza tot (date de baza, experienta, educatie, bara din stanga, poza). **Incarca JSON** il aduce inapoi pentru editare.
- Nu exista import din PDF: JSON-ul este formatul de lucru.

## Format JSON (`"format": "cv-editor"`, `"version": 1`)

`basics`, `profile`, `experience[]` (grupuri cu `heading` si `items` de tip `bullet` sau `text`), `projects[]`, `education[]` (cu `details`), `sidebar` (`topSkills`, `tagGroups`, `domains`, `interests`, `languages`) si `photo` (PNG data URL).

Datele personale raman in JSON-ul tau, nu in repo.
