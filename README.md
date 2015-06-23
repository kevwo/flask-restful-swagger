# flask-restful-swagger

This fork adds the following functionality.

1.) Ability to group sections of swagger APIs.


```
@swagger.resource(
    hierarchy_id='VendingMachines',
    hierarchy_description='Operations on VendingMachines objects'
)
class VendingMachine(Resource):
```

2.) Ability to specify a custom description for a swagger URL.

```
api.add_resource(VendingMachine, "/Region/<string:region_id>"
                                    "/Brand/<string:brand_id>"
                                    "/Machine/<string:machine_id>", display_path="/**/machine")
```

Install:

```
pip install git+git://github.com/kevwo/flask-restful-swagger.git#egg=flask-restful-swagger
```
(This installs flask-restful as well)

