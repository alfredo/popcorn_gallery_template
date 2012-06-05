Sample Template for the Popcorn Gallery
=======================================

Templates are composed by at least three components:

* An HTML page
* A JSON Butter configuration file
* A JSON with default metadata

Optional, any other media part of the template.

These can be added via the admin interface or bulk upload

It is recomended to import a template in bulk if your template has several assets.

These are the instructions to prepare a template for upload:

* A template can be bulk uploaded with a zip file, the files must be contained in
  a folder with the template name.
* The slugified name of the zip file will be used as the name of the template.
* All the valid assets will be listed and added to the build.
* Any supplied asset with the template must use relative paths.
* Non relative paths is recommended to use absolute URLS.
* There is no need for the ``base`` tag.
* All templates butter initialization must call ``config`` as the default data value.
* The ``config`` URL is automatically populated with the PM site required values
  e.g.

    {
     "savedDataUrl": "data",
     "baseDir": "/static/",
     "name": "default-butter"
    }

These files are at the moment imported via the admin.