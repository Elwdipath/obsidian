---
type: course
title: Go Basics
provider: Frontend Masters
status: Not Started
start_date: ""
finish_date: ""
tags:
  - course
  - learning
  - go
  - golang
---
## Installing and Running Go

Go Website: https://go.dev

### Initializing a project

Go has no boilerplate

#### go mod init
`go mod init <name>`

#### Public Module naming convention
Pattern: <hostingname><author><project>
Example: github.com/elwdipath/go-project

Module Name is how the public references and how it's identifiable to itself

Go does not have the concept of relative paths and instead packages are identified and imported using the full module name and package location

go.mod and main.go are created with `go mod init <name>`


