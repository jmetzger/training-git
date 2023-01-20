# GIT-Server 

## Builtin with git-installation

### Simple GIT-Server 

```
# included in installation with git
Cons: Can do nearly nothing (only pushing and pulling)

* no graphical interface
* no multi-user support 
* no additional features (like bugtracking / milestones a.s.o) 

```

### Web-Interface (also from git installation) 

```
Cons: Mo multi-user interaction 
```

## Comfortable Git-Server 

### gitea / codeberg 

  * OpenSource 
  * minimum feature
  * not integrated with other software 
  
### gitlab 

#### General 

  * On premise / cloud 

#### Pros 

  * Devops - Server (Integration) 
  * Tools für Devops 
  * Integration von CI/CD 
    * Favourite von Jochen (in opposite github actions)
  * kleine Teams können on premise kostenlos starten 
  * Im Rahmen von DevOps auch automatische Integration von Scannen von Software drin.
  
### bitbucket 

#### Overview 

  * Software Company Atlassian.
  * Problematic license policy 
  * Cloud-Based (SaaS) - ich miete - subscription 
  * On Premise (Installation im Firmennetz) 
    * aber abgekündigt 
  * On Premise fü+r grosse Unternehmen - sehr teuer 

#### Pros

  * Integration with other software products (confluence - wiki, jira - ticket system)
  * webhooks (url aufgerufen wird dich ich festlege mit einem payload) 

#### Cons 

  * No CI/CD directly within bitbucket 

### github 

#### Overview 

  * Bought by microsoft 

#### Pros 
 
  * on premise git gut möglich (github enterprise) 
  * Editor sehr gut im Web-Interface 

#### Cons 

  * Menüführung von github nicht so intuitiv für Jochen 
  * github actions (CI/CD) zu kompiziert (Lernkurve größe als bei gitlab ci/cd) 
  
### Azure Devops

#### Overview 

  * Repos are use from github under the hood 

#### Con 

  * Lernkurve höher als bei github, gitlab, bitbucket

#### Pros 

  * Sicherheitsfeatures höher 
  * Integration mit VisualStudio
  * Kostenvorteile durch Lizenz Visual Studio Pro 
 
