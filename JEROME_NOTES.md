# step 1 - https://github.com/datoviz/datoviz/pull/120
- added tp.Optional everytime the arguments = None
- wrap the visual return with tp.cast(...) for app.path etc..
- added tp.Optional image_flags, mesh_flags, sphere_flags with tp.Optional 
- added some `type: ignore` where pyright was complaining. They can be fixed later.
- all modifications are in type hints only, no runtime code was changed.
- pyright ./datoviz/_app.py  to count the errors

# step 2
- added tp.Optional where needed in _texture.py and visuals.py
- added some assert. to be reviewed carefully as they might change runtime behavior.
