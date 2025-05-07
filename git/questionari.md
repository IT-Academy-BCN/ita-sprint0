# Qüestionari d'Introducció a Git

## Preguntes d'una única resposta (10)

### 1. Què és Git?
- [ ] a) Un sistema operatiu  
- [ ] b) Un llenguatge de programació  
- [x] c) Un sistema de control de versions  
- [ ] d) Una eina de disseny gràfic  

### 2. Quin comandament inicialitza un repositori Git en un directori local?
- [x] a) `git init`  
- [ ] b) `git start`  
- [ ] c) `git new`  
- [ ] d) `git create`  

### 3. Quina ordre s'utilitza per afegir tots els canvis al _staging area_?
- [ ] a) `git save .`  
- [ ] b) `git stage`  
- [x] c) `git add .`  
- [ ] d) `git commit -a`  

### 4. Vols descarregar un repositori remot al teu ordinador. Quin comandament utilitzaries?
- [ ] a) `git pull`  
- [x] b) `git clone <URL>`  
- [ ] c) `git download`  
- [ ] d) `git copy`  

### 5. **Cas pràctic**: Has modificat `index.html` i vols veure quins canvis estan pendents per _commit_. Quin comandament executaries?
- [x] a) `git status`  
- [ ] b) `git log`  
- [ ] c) `git diff`  
- [ ] d) `git show`  

### 6. **Cas pràctic**: Has fusionat una branca i tens un conflicte de fusió a `style.css`. Quin és el primer pas per resoldre-ho?
- [ ] a) Eliminar el fitxer  
- [ ] b) Executar `git abort`  
- [x] c) Editar manualment el fitxer per marcar les solucions  
- [ ] d) Tornar a executar `git merge`  

### 7. **Cas pràctic**: Vols crear una branca anomenada `feature-login`. Quin comandament és correcte?
- [ ] a) `git branch -n feature-login`  
- [x] b) `git checkout -b feature-login`  
- [ ] c) `git new branch feature-login`  
- [ ] d) `git create branch feature-login`  

### 8. Quin comandament mostra el historial de commits amb detalls?
- [ ] a) `git list`  
- [x] b) `git log`  
- [ ] c) `git history`  
- [ ] d) `git commits`  

### 9. **Cas pràctic**: Després de resoldre un conflicte de fusió, quins passos cal seguir?
- [ ] a) `git commit`  
- [ ] b) `git add` + `git commit`  
- [x] c) `git add <fitxer>` + `git commit`  
- [ ] d) `git push`  

### 10. Quin comandament actualitza el repositori local amb canvis del remot sense fusionar-los a la teva branca?
- [x] a) `git fetch`  
- [ ] b) `git pull`  
- [ ] c) `git sync`  
- [ ] d) `git update`  

### 11. Què representa una *Pull Request* (PR)?
- [ ] a) Una petició per eliminar una branca  
- [x] b) Una sol·licitud per fusionar canvis d'una branca a una altra  
- [ ] c) Un informe d'errors  
- [ ] d) Una actualització automàtica del repositori  

### 12. **Cas pràctic**: Vols assignar una tasca a un col·lega i fer-ne seguiment. Quina eina de GitHub utilitzaries?
- [ ] a) Projects  
- [ ] b) Milestones  
- [x] c) Issues  
- [ ] d) Wiki  

### 13. Quina branca actua com a font de veritat única (*single source of truth*) en un entorn col·laboratiu?
- [ ] a) `develop`  
- [x] b) `main` o `master`  
- [ ] c) `feature/login`  
- [ ] d) `hotfix`  

### 14. **Cas pràctic**: Un col·lega ha aprovat la teva PR a GitHub. Quin pas cal seguir?
- [ ] a) Fer `git revert`  
- [x] b) Fer *merge* des de la interfície de GitHub  
- [ ] c) Eliminar la branca automàticament  
- [ ] d) Tornar a enviar els canvis amb `git push`  

### 15. Què és un *Milestone* en GitHub?
- [x] a) Un objectiu amb data límit per agrupar tasques o issues  
- [ ] b) Una branca temporal per a experiments  
- [ ] c) Una etiqueta per marcar versions  
- [ ] d) Un informe d'estadístiques del projecte  

### 16. **Cas pràctic**: Has de corregir un error crític en producció. Segons Git Flow, quina branca has de crear?
- [ ] a) `feature/hotfix`  
- [x] b) `hotfix/error-login`  
- [ ] c) `release/error`  
- [ ] d) `patch/error`  

### 17. Quina ordre mostra les branques fusionades a la branca actual?
- [ ] a) `git branch --merged`  
- [x] b) `git branch --merged`  
- [ ] c) `git log --branches`  
- [ ] d) `git show-branch`  

## Preguntes de respostes múltiples (10)

### 1. Quines accions realitza `git push`? (Tria 2)
- [x] a) Envia commits locals al repositori remot  
- [ ] b) Descàrrega canvis del remot  
- [x] c) Actualitza les referències de branques remotes  
- [ ] d) Elimina commits no sincronitzats  

### 2. **Cas pràctic**: Quines eines/ordres ajuden a desfer un commit local? (Tria 2)
- [x] a) `git reset --soft HEAD~1`  
- [ ] b) `git delete commit`  
- [x] c) `git revert HEAD`  
- [ ] d) `git undo`  

### 3. Quins fitxers ignorarà `.gitignore` amb aquesta regla: `*.log`? (Tria 2)
- [x] a) `error.log`  
- [ ] b) `logs/access.txt`  
- [x] c) `debug.log`  
- [ ] d) `config.log.txt`  

### 4. **Cas pràctic**: Quins comandaments configuren l'usuari de Git globalment? (Tria 2)
- [x] a) `git config --global user.name "Nom"`  
- [ ] b) `git set user.email "correu@exemple.com"`  
- [x] c) `git config --global user.email "correu@exemple.com"`  
- [ ] d) `git user --global "Nom"`  

### 5. Quins elements formen part de l'estructura bàsica de Git? (Tria 3)
- [x] a) Working Directory  
- [x] b) Staging Area  
- [x] c) Repository  
- [ ] d) Cloud Storage  

### 6. **Cas pràctic**: Quins comandaments permeten canviar a una branca existent? (Tria 2)
- [x] a) `git checkout <nom-branca>`  
- [ ] b) `git switch -c <nom-branca>`  
- [x] c) `git switch <nom-branca>`  
- [ ] d) `git branch <nom-branca>`  

### 7. Quines accions realitza `git stash`? (Tria 2)
- [x] a) Desa canvis no _commitats_ temporalment  
- [ ] b) Elimina tots els canvis pendents  
- [x] c) Permet canviar de branca sense fer commit  
- [ ] d) Crea una branca nova  

### 8. **Cas pràctic**: Quins comandaments són vàlids per afegir un repositori remot? (Tria 2)
- [x] a) `git remote add origin <URL>`  
- [ ] b) `git add remote origin <URL>`  
- [x] c) `git remote set-url origin <URL>`  
- [ ] d) `git connect origin <URL>`  

### 9. Quins usos té `git tag`? (Tria 2)
- [x] a) Marcar versions específiques (ex: v1.0.0)  
- [ ] b) Crear una branca temporal  
- [x] c) Anotar commits amb metadades addicionals  
- [ ] d) Eliminar commits antics  

### 10. **Cas pràctic**: Quins passos són necessaris per publicar una branca local al remot? (Tria 2)
- [x] a) `git push -u origin <nom-branca>`  
- [ ] b) `git send origin <nom-branca>`  
- [x] c) `git push origin <nom-branca>`  
- [ ] d) `git upload <nom-branca>`  

### 11. Quines accions es poden realitzar amb un *fork*? (Tria 2)
- [x] a) Modificar un repositori sense afectar l'original  
- [ ] b) Eliminar l'historial de commits  
- [x] c) Enviar canvis mitjançant PR a l'original  
- [ ] d) Fusionar automàticament branques remotes  

### 12. **Cas pràctic**: Quins passos són necessaris per contribuir a un projecte via fork? (Tria 3)
- [x] a) Fer un fork del repositori original  
- [x] b) Clonar el teu fork localment  
- [ ] c) Crear una branca directament a l'original  
- [x] d) Enviar una PR després de fer canvis  

### 13. **Cas pràctic**: Quines eines ajuden a gestionar conflictes en una PR? (Tria 2)
- [x] a) Resolució de conflictes des de la interfície web de GitHub  
- [ ] b) `git cancel`  
- [x] c) `git merge --abort`  
- [ ] d) `git ignore`  

## Respostes correctes

### Preguntes d'una única resposta:
1. c  
2. a  
3. c  
4. b  
5. a  
6. c  
7. b  
8. b  
9. c  
10. a  
11. b
12. c
13. b
14. b
15. a
16. b
17. b
### Preguntes de respostes múltiples:
1. a, c  
2. a, c  
3. a, c  
4. a, c  
5. a, b, c  
6. a, c  
7. a, c  
8. a, c  
9. a, c  
10. a, c
11. a, c
12. a, b, d
13. a, c  
