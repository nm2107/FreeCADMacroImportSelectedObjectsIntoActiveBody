# FreeCAD Macro Import selected objects into active body

A FreeCAD macro to speed up the process of importing (bind) selected objects
into the active body of the current document.
The selected objects can come from linked documents.

**What it does :**

It creates one SubShapeBinder per selected object and adds it to the active body
body of the Document. The created binders are named along the original selected
objects names.

If a DatumPlane is selected, the macro also creates a new DatumPlane mapped on
the SubShapeBinder, so plane features can still be used on the imported item.

**How to use :**

- Activate a Body into the current document.
- Select some objects from the tree.
- Invoke the macro.

**Why ?**

In order to avoid to manually create a SubShapeBinder (and possibly other
objects) and to name it each time you want to import an object into
the active Body.

It will speed up the FreeCAD workflow.

For more details :

- https://forum.freecad.org/viewtopic.php?t=78818
