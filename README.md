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
