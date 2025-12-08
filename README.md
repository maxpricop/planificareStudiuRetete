# PlanificareStudiuRetete

## Introducere 
`PlanificareStudiuRetete` este un proiect care modelează o aplicație desktop pentru descoperirea, organizarea și partajarea de rețete culinare. Scopul principal este documentarea cerințelor (SRS) și a diagramelor (Use Case, Activity) pentru funcționalitățile de bază: căutare, vizualizare, creare/actualizare/ștergere rețetă, gestionare conturi, favoriting și moderare.

Link prototip figma: https://www.figma.com/design/nC56n5znSmQPqaeojxAIWb/Retete-Culinare?node-id=83-2&t=CkCOVOqXyfHlzWHJ-1

## Funcționalități principale
- **Căutare & Vizualizare**: listare rețete, filtrare după categorie/ingrediente/dificultate.
- **Autentificare**: creare cont, login; funcții extinse disponibile doar utilizatorilor autentificați.
- **Adăugare/Editare/Ștergere rețetă**: editor WYSIWYG cu inserare imagini; titlu și imagine principală sunt obligatorii.
- **Salvare favorite** și **Comentarii** pentru utilizatorii autentificați.
- **Roluri și moderare**: administratori pot publica, edita, șterge și modera conținutul.

## Structură repository
- `SRS.md` : Specificațiile cerințelor aplicației (functional / non-functional).
- `README.md` : (acest fișier) descriere și comenzi utile.
- `Diagrams/` : conține diagramele proiectului (PlantUML `.puml` și fișiere `.drawio`).
	- `Diagrams/Activity.puml` : Activity diagram pentru fluxul de adăugare rețetă.
	- `Diagrams/Use Case.puml` : diagrama Use Case.

## Comenzi Git (exemple PowerShell)
Următoarele comenzi arată pașii uzuali de inițializare a unui repo local și setare remote până la primul commit/push.

1. Configurează identitate (doar o dată pe mașină):
    ```powershell
    git config --global user.name "Your Name"
    git config --global user.email "you@example.com"
    ```

2. Inițializează repo local și creează branch-ul principal `main`:
    ```powershell
    git init
    git branch -M main
    ```

3. Setează remote origin. Exemplu de setare remote:
    ```powershell
    git remote add origin https://github.com/maxpricop/planificareStudiuRetete.git
    ```

4. Pregătește și salvează primul commit:
    ```powershell
    git add .
    git commit -m "Initial commit"
    ```

5. Împinge (push) branch-ul `main` către remote (dacă ați setat `origin`):
    ```powershell
    git push -u origin main
    ```
