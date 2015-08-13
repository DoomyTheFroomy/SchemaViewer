# Schema Viewer

This projects helps to display the structure of [json schemata (v4)](http://json-schema.org/) and is based on [docson](https://github.com/lbovet/docson) as a CouchApp. 

## How to use

Just create a new widget html file, like:

```html
<!-- schema.html -->
<!DOCTYPE html>
<html>
<head>
  <title>Schema view</title>
</head>
<body>
  <script src="./widget.js" data-schema="./schemata/schmema.json"></script>
</body>
</html>
```

And put all the required schema files under `/_attachments/schemata/` folder. 

After you have done this you can push the CouchApp, e.g. via [erica](https://github.com/benoitc/erica)

```
erica push http://username:pwd@127.0.0.1:5984/schemaViews
```

Then you can see your schema file in a nice formatted design, under: 

    http://127.0.0.1:5984/schemaViews/_design/schemaView/schema.html