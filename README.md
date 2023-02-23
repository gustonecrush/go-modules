# Golang Modules

## Agenda
We are going to learn about
- Introduction to Go Modules
- Create Module
- Module Release
- Adding Depedency
- Updgrade Module
- Updgrade Depedency

## Introduction to Go Modules
Go modules is new feature in Golang. 

### Introduction
- When we create an application, we usually using library or depedency from another project
- Before Go Modules exist, in managament depedency is hard in Go-lang
- We usually copy all source code library or depedency to our project, that makes our project eat a lot of space
- Or we use library and save in GOPATH directory, but this will be hard if there is an application need the same library but different version

### Go-Modules
- Go-Modules started known in Go-lang 1.11 and 1.12
- With Go-Modules, we can create project easily and with easiest depedency management  

### Conclusion
- Go-Modules is used to manage your depedency when you create an application, this is such as npm, composer, maven, gradle, etc. So makes you easily to manage your depedency


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

