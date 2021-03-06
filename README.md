# loadreport.js
[PhantomJS](http://www.phantomjs.org/) 1.6+ is required to run loadreport.js or speedreport.js.

You can take it for a spin in [this live demo](http://loadreport.wesleyhales.com/report.html).

## loadreport Examples
### loadreport will write, to csv, json or junit format xml (filmstrip writes to png):
* ``` phantomjs loadreport.js http://cnn.com performance csv ```
![loadreport](https://raw.github.com/wesleyhales/loadreport/master/readme/cnn-loadreport.png)
    
* ``` phantomjs loadreport.js http://cnn.com performancecache json ```
    
* ``` phantomjs loadreport.js http://cnn.com filmstrip ``` 
![loadreport filmstrip](https://raw.github.com/wesleyhales/loadreport/master/readme/cnn-filmstrip.png)


## speedreport Examples
### speedreport produces a json and html file which will display detailed resource charting
* ``` phantomjs speedreport.js http://www.cnn.com```
![speedreport](https://raw.github.com/wesleyhales/loadreport/master/readme/speedreport.png)


## Embedded web server
### Quickly display speedreport HTML files

Install npm packages

* ``` npm install```

Generate a report

* ``` phantomjs speedreport.js http://www.cnn.com```

Run the webserver

* ``` ./node_modules/loadreport/lib/webserver.js [www_dir]```

Run your favorite browser to **http://localhost:8080/**.


## Documentation index

http://maboiteaspam.github.io/loadreport/documentation/schedule-loadreport.html

http://maboiteaspam.github.io/loadreport/documentation/speedreport.html

http://maboiteaspam.github.io/loadreport/documentation/loadreport.html

http://maboiteaspam.github.io/loadreport/documentation/main.html

http://maboiteaspam.github.io/loadreport/documentation/webserver.html

## Development support
### Setup

Install npm packages

* ``` npm install grunt-cli -g```
* ``` npm install mocha -g```
* ``` npm install```

### Test

See mocha

* ``` npm test```

### Document

See grunt-gh-pages, docco

* ``` grunt```

### Release, Bump version

See grunt-release

* ``` grunt release:patch```

