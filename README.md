# Python-pptx-Enhanced

Basically, this is [python-pptx](https://github.com/AndreasSteiner/python-pptx), just with support for few new functions and few bugs fixes.

## Function Added

**Remove method to directly remove a table or groupshape or a picture**  
e.g prs = presentation(file_path)  
prs.slides[slide_index].shapes[shape_index].remove() will remove the element 

**replace_with_picture method**  
e.g.  
prs.replace_with_picture(slide_index,shape_name,img_path)

**shape_index method**  
e.g  
prs.shape_index(slide_index,shape_name) returns the index of shape that you can use to target a particular shape in the slide

**update_text method**  
e.g  
textFrame = prs.slides[6].shapes[8].text_frame  
textFrame.update_text(new_text) will update the text in that text frame while retaining the format of old text.  
This method returns the updated text

## Issue Fixed

**Fixed issue with Python 3.10+ - "AttributeError: module 'collections' has no attribute 'abc'"**  
Function to replace any shape with a picture


A typical use would be generating a customized PowerPoint presentation from
database content, downloadable by clicking a link in a web application.
Several developers have used it to automate production of presentation-ready
engineering status reports based on information held in their work management
system. It could also be used for making bulk updates to a library of
presentations or simply to automate the production of a slide or two that
would be tedious to get right by hand.

More information is available in the `python-pptx documentation`_.

Browse `examples with screenshots`_ to get a quick idea what you can do with
python-pptx.

.. _`python-pptx documentation`:
   https://python-pptx.readthedocs.org/en/latest/

.. _`examples with screenshots`:
   https://python-pptx.readthedocs.org/en/latest/user/quickstart.html
