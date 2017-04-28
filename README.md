# <img src="https://github.com/pip-services/pip-services/raw/master/design/Logo.png" alt="Pip.Services Logo" style="max-width:30%"> <br/> Workspace for Support Pip.Services

This is a workspace for [Support Pip.Services](https://github.com/pip-services-support) 
implemented in 5 different languages: .NET, Java, Node.js, Go and Python.

The workspace enables build, test, and release across the following projects:

- **pip-services-devenv** - dockerized infrastructure services for development and testing
- **pip-services-announcements-node** - Announcements microservice in Node.js
- **pip-clients-announcements-node** - Client to Announcements microservice in Node.js
- **pip-services-announcements-node** - User feedback microservice in Node.js
- **pip-clients-announcements-node** - Client to User feedback microservice in Node.js
- **pip-facade-support-node** - Facade operations for support microservices in Node.js

## Installation

- Install **pip-tasks-ps**, **pip-tasks-common-ps** and **pip-tasks-node-ps** Powershell modules, 
add them to **PSModulePath** and import into Powershell

- Clone this workspace to local disk
```bash
> git clone https://github.com/pip-services-infra/pip-services-support-ws.git
```

- Got to the workspace folder and clone component repositories
```bash
> piptask clone -workspace
```

## Usage

- Setting default workspace
```bash
> pipuse <Path to this workspace>
```

- Start and stop infrastructure services
```bash
> piptask start -component pip-services-devenv
> piptask stop -component pip-services-devenv
```

- Building all components
```bash
> piptask build -all
```

- Test all components
``` bash
> piptask test -all
```

- Check out changes from remote repository
```bash
> piptask pull -all
```

- Check in changes to remote repository
```bash
> piptask push -m <Changes comment> -all
```

## Acknowledgements

The Support Pip.Services are created and maintained by **Sergey Seroukhov**
