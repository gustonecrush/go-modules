# Golang Modules

## Agenda
We are going to learn about
- Introduction to Go Modules
- Create Module
- Module Release
- Adding Dependency
- Upgrade Module
- Upgrade Dependency

## Introduction to Go Modules
Go modules is new feature in Golang. 

### Introduction
- When we create an application, we usually use library or dependency from another project
- Before Go Modules exist, in management dependency is hard in Go-lang
- We usually copy all source code library or dependency to our project, that makes our project eat a lot of space
- Or we use library and save in GOPATH directory, but this will be hard if there is an application need the same library but different version

### Go-Modules
- Go-Modules started known in Go-lang 1.11 and 1.12
- With Go-Modules, we can create project easily and with easiest dependency management  

### Conclusion
- Go-Modules is used to manage your dependency when you create an application, this is such as npm, composer, maven, gradle, etc. So makes you easily to manage your dependency


## Creating Module

## Create Module
- To create new module, we usually use command `go mod init module-name`
- Go-Lang will automatically create `go.mod` file which contains all information about module's names and its versions

## Release Module
- Go-Lang is integrated with Git
- To release a module, we only need create Tag in Git

## How to create
1. Go to your github account, then create new repository and set it to be public
2. Copy your repo URL
3. Create new folder project, first for your module and second for your app
4. Open the folder module in your IDE or Code Editor, then open terminal `go mod init github.com/gustonecrush/go-modules`
5. And create your first module, don't forget to commit and push every change in your modules to github repo

## How to create version release
1. Run command `git tag v1.0.0`
2. Then run `git push origin v1.0.0`

## How to add Dependency 
1. Open your folder app in IDE or code editor
2. Crate new repo in your Github, then copy the URL name of your repo
3. Back to terminal, then run command `go mod init yourgithubnameURLrepo`
4. Then create your main file in app folder, then run `go get yourgithubnamemodulerepo`
5. Finally, you can use it in your project

## Upgrade Module

### Upgrade module
- To upgrade our module, we only need to create new tag in Git

## Upgrade Dependency

### Upgrade Dependency
- We can edit `go.mod` file then change the tag to new version, then to download new version you only run `go get`
- If you change or edit wrong version, when you run `go get` it will show error message, so easy right?
- If you have get new version then you run `go get` again, it will not download again, because it will store in cache, so when you do upgrade in your module as little as you did you have to push the new tag (best version) no using the same tag

## Major Upgrade
- Major upgrade usually happen because of changes on our code program, so make not be backward compatible (our code is broken, where in new version is different with old version, so user who want to upgrade the dependency jgn asal-asalan :v)
- This has tobe avoid, don't do this which make backward compatible
- Add new feature is not a problem, but broke the code of old feature you have to think twice about it
- If it has to be change or major upgrade, the best strategy you don't have use the same module name which indicate if there is major changes
- The best strategy you can use new module name and level up the version tag to most ex (2.0.0)
- The name is usually `/v2` in end of module name, that's not a problem if there is two module name in one repo
- Then add, commit, and push updates
- And create new tag

- So, if there is someone who want to use newest version our module has add `/v2` in module name
- When add newest dependency you can run command like this `go get github.com/gustonecrush/go-modules/v2
  `
- If wrong, you will download the old one

### Conclusion
- If you do major changes so, up to new version 1.0.0 >> 2.0.0 and change module name
- If you do minor major so, just add 1.0.0 >> 1.2.5 just like that
- You can the example of this naming in other modules such as gorm, gofiber, etc

## Outro of Go-Modules
So, start right now always using go-modules don't manage your dependecy manually and copy also paste the library to your project 

## Conclusion
If you want to learn good web app or web server you have to learn :
1. Go-Lang Unit Test
2. Go-Lang Concurrency (Goroutine)
