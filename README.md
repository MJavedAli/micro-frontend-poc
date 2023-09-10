# micro-frontends (angular,react) PoC
## Goals
* Build a portal-like application featuring a top-header and left-side navigation bar.
* Enable the navigation bar to link to sub-applications.
* Implement sub-applications using different technologies, such as Angular 5 and React 16.
* Allow rendering of a single sub-application on a single page.
* Support rendering of multiple sub-applications on a single page.
* Enable each sub-application to be independently deployable and hosted on different servers.
* Ensure that CSS stylesheets are independent.
* Enable communication between sub-applications.


## Modules

### sub-app-angular    

This module represents an Angular 5 application and serves as a sub-application within the portal.
    
### sub-app-react16
This module represents a React 16 application and serves as a sub-application within the portal.

### main-app
This module represents a React 15 application, acting as a template application that aggregates **sub-app-angular** and **sub-app-react16** into a portal.


## Deployment
### sub-app-angular
~~~~
cd sub-app-angular
npm install
npm run build
npm run serve
~~~~
Access the bundles at: http://localhost:3001
### sub-app-react16
~~~~
cd sub-app-react16
npm install
npm run open
npm run serve
~~~~
* Access the bundles at: http://localhost:3002/
* CDN will be available at http://localhost:3002/static/js/openbundle.js

### main-app
~~~~
cd main-app
npm install
npm run build
npm run serve
~~~~
Access the application at: [http://localhost:3000](http://localhost:3000)

You can also see sub-app-react16 seperately by opening `index.html` inside `standalone` directory. 
