FOXX Applications
=================

Foxx is an easy way to create APIs and simple web applications from
within ArangoDB. It is inspired by Sinatra, the classy Ruby web
framework.

If you have created a nice Foxx application and you want to share it with
the community out there, clone this repository, add a short description
to the "applications" folder and issue a pull request.

"hallo-foxx" is the hallo world example for Foxx. Its 
[description file](https://github.com/triAGENS/foxx-apps/blob/master/applications/hallo-foxx.json)
can be found in the applications folder.

    {
      "description": "This is 'Hallo World' for ArangoDB Foxx.",
      "author": "Frank Celler",

      "versions": {
        "1.1.0" : { "type": "github", "location": "fceller/hallo-foxx", "tag": "v1.1.0" }
      }
    }

The description file is a JSON document with the attributes:

* *description*: a short description of the application
* *author*: the name of the author, an email address, or a twitter handle
* *versions*: a list of available versions

In order to install this application into your local ArangoDB
installation, you can use the foxx-manager like this

    foxx-manager install hallo-foxx /hallo

This will download the application into your local installation of
ArangoDB (which must be up and running) and mount it under the path
"/test".

If you now visit

    http://localhost:8529/hallo

you should see a nice fox.