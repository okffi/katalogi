
# Ennakkovalmistelut

## Debian / Ubuntu

` sudo apt-get install python-dev postgresql libpq-dev python-pip python-virtualenv git-core solr-jetty openjdk-6-jdk `

## OSX

Mac-ympäristössä unix-ohjelmat asennetaan yleensä [Homebrew-paketinhallinnalla](http://mxcl.github.io/homebrew/).
Seuraavassa CKAN:in asennusohjeen [ennakkovaatimukset](http://docs.ckan.org/en/latest/install-from-source.html#install-the-required-packages)
ja suunnitelma niiden täyttämiseen.

| CKANin vaatimus | Brew resepti   | pip paketti | osx:n oma       |
| ---------------:|---------------:|------------:|----------------:|
| Python	        | python         |             |                 |
| PostgreSQL	    | postgresql     |             |                 |
| libpq	          | postgresql [1] |             |                 |
| pip	            | pip [2]        |             |                 |
| virtualenv	    |                | virtualenv  |                 |
| Git	            | git            |             |                 |
| Apache Solr	    | solr           |             |                 |
| Jetty	          | jetty          |             |                 |
| OpenJDK 6 JDK	  |                |             | *kelpaako?* [3] |

[1] = libpq ilmeisesti brew:n [postgresql-reseptissä](http://serverfault.com/questions/277374/install-libpq-dev-on-mac-os)

[2] = pip ilmeisesti brew:n [python-reseptissä](https://github.com/mxcl/homebrew/wiki/Homebrew-and-Python)

[3] = terminal komento ```java -version``` kertoo ```java version "1.6.0_51" ```
