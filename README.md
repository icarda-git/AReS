# AReS

The [Agricultural Research e-Seeker (AReS)](https://cgspace.cgiar.org/explorer/) is a dashboard-like tool that was created to help people find and understand content in open access repositories like [DSpace](https://duraspace.org/dspace). It began as a proof of concept designed by [the Monitoring, Evaluation and Learning (MEL)](https://mel.cgiar.org) team at the [International Center for Agricultural Research in the Dry Areas (ICARDA)](https://www.icarda.org)  and developed by [CodeObia](http://codeobia.com/) to enable exploring and reporting on content in two key institutional repositories.

This project contains a backend indexer powered by [Node.js](https://nodejs.org/) and [Elasticsearch](https://www.elastic.co), and a dynamic frontend built with [Angular](https://angular.io), [Bootstrap](https://getbootstrap.com), [Highcharts](https://www.highcharts.com/), [Angular Material](https://material.angular.io/), and [Ngrx](https://ngrx.io/). The application is wrapped up and deployed via [Docker](https://www.docker.com/). This product includes GeoLite2 data created by MaxMind, available from [https://www.maxmind.com](https://www.maxmind.com).


# Requirements 
  node v8.11.1 +
  npm 5.6.0 +
  docker 17.12.0+
  docker-compose 1.18.0+
  
# installation 

`git clone https://github.com/CodeObia/AReS.git`

`cd AReS/frontend `
`npm i`
`npm install -g @angular/cli`
`ng build --prod `

`cd AReS/app`
`npm i`

`cd AReS`
`sudo chmod 777 -R esConfig/`
`docker-compose up -d`

## License

This work is licensed under the [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html). The license allows you to use and modify the work for personal and commercial purposes, but if you distribute the work you must provide users with a means to access the source code for the version you are distributing. Read more about the [GPLv3 at TL;DR Legal](<https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)>).
