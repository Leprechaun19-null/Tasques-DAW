# Flux d'un repositori Git

## Taula de Continguts
- [Creació del repositori](#creació-del-repositori)
- [Edició del document](#edició-del-document)
- [Gestió de canvis](#gestió-de-canvis)
- [Importació del repositori a Github](#importació-del-repositori-a-github)
- [Sincronització amb GitHub](#sincronització-amb-github)

## Creació del repositori
Obrim el nostre terminal preferit i creem el directori arrel del repository
```bash
 $ mkdir 'Tasques_DAW'
```
Després, inicialitzem el repositori
```bash
 $ git init
```
Git ens tornarà el missatge d'èxit
```bash
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint: 
hint:     git config --global init.defaultBranch <name>
hint: 
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint: 
hint:     git branch -m <name>
Initialized empty Git repository in /home/manpop/Tasques DAW/.git/`  
```
Després, creem el nostre document
```bash
$ nano Documentació_flux_git.md
```
## Edició del document
Per editar el document he triat l'editor MarkText, perque renderitza el document a la par que es va editant , però es pot editar inclús amb nano mateix
## Gestió de canvis
Després de guardar els canvis, afegim tots el arxius del directori del repositori al area *staging* amb este comandament :
```bash
$ git add . 
```
Finalment, fem efectiu el canvi amb un *commit*
```bash
$ git commit -m "Primer commit, creada documentació"
```
## Importació del repositori a Github
Per importar el repositori a GitHub, seguirem aquests passos
1.Al nostre perfil de GitHub creem un nou repositori
<img width="1888" height="861" alt="{4D2398B5-8D95-4763-8B60-297082B6F97A}" src="https://github.com/user-attachments/assets/f13f0c5d-6b66-4843-b1d3-044dd5fcd926" />


Després, al quick setup, executem aquests comandaments:
```bash
$ git remote add origin <url del repositori>
```
```bash
$ git branch -M main
```
```bash
$ git push -u origin main
```
## Sincronització amb GitHub
A partir d'ara, cada volta que fem commits, haurem d'executar 
```bash
$ git push -u origin main
```
Aixi garantim la sincronització entre la nostra còpia local del repositori i la de GitHub.
