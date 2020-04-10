# AReS

The [Agricultural Research e-Seeker (AReS)](https://cgspace.cgiar.org/explorer/) is a dashboard-like tool that was created to help people find and understand content in open access repositories like [DSpace](https://duraspace.org/dspace). It began as a proof of concept designed by [the Monitoring, Evaluation and Learning (MEL)](https://mel.cgiar.org) team at the [International Center for Agricultural Research in the Dry Areas (ICARDA)](https://www.icarda.org)  and developed by [CodeObia](http://codeobia.com/) to enable exploring and reporting on content in two key institutional repositories.

This project contains a backend indexer powered by [Node.js](https://nodejs.org/) and [Elasticsearch](https://www.elastic.co), and a dynamic frontend built with [Angular](https://angular.io), [Bootstrap](https://getbootstrap.com), [Highcharts](https://www.highcharts.com/), [Angular Material](https://material.angular.io/), and [Ngrx](https://ngrx.io/). The application is wrapped up and deployed via [Docker](https://www.docker.com/). This product includes GeoLite2 data created by MaxMind, available from [https://www.maxmind.com](https://www.maxmind.com).

# Requirements

- Node.js v8+
- npm 5.6.0+
- Docker 17.12.0+
- docker-compose 1.18.0+
-  [dspace-statistics-api](https://github.com/ilri/dspace-statistics-api) (optional, for item views and downloads)

# Installation  

After you have satisfied the requirements you can clone this repository:
```console
$ cd docker
$ sudo docker-compose up -d
```  
*Note: the Elasticsearch component requires more virtual memory. You will most likely need to increase the host system's memory map limits by setting `vm.max_map_count = 262144` in /etc/sysctl.conf. See the [Elasticsearch docs for more information](https://www.elastic.co/guide/en/elasticsearch/reference/current/vm-max-map-count.html).*

# License

This work is licensed under the [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html). The license allows you to use and modify the work for personal and commercial purposes, but if you distribute the work you must provide users with a means to access the source code for the version you are distributing. Read more about the [GPLv3 at TL;DR Legal](<https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)>).
