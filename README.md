# appengine-nodejs-quickstart

A starter project for node.js on Google App Engine Managed VMs using Custom Runtimes.

## Usage

Start by cloning this repository.

Install dependancies:
~~~~
npm install
~~~

To run the app locally in the dev appserver:

~~~~
gcloud preview app run .
~~~~

If needed, you can enable debug output:

~~~~
gcloud --verbosity debug preview app run .
~~~~

To deploy the app in production:

~~~~
gcloud --project YOUR-PROJECT-NAME-HERE preview app deploy --server preview.appengine.google.com .
~~~~

## Application layout

The main script for the application is `server.js`.

Static files are in the `static` directory. The `app.yaml` descriptor is already configured to serve all `.html`, `.css` and `.js` files under `static` as static content.

The main page for the application is `static/index.html`.

## APIs

The documentation for the App Engine-specific APIs is on github under the [appengine-nodejs][1] project.

You may also find useful to use the following two libraries to access Google Cloud Platform APIs from node.js: [googleapis][2] and [gcloud-node][3].

[1]: https://github.com/GoogleCloudPlatform/appengine-nodejs
[2]: https://www.npmjs.org/package/googleapis
[3]: https://github.com/GoogleCloudPlatform/gcloud-node
