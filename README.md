# marking-tools
Repo used for marking of submissions in tex.

Creates a latex file for each student in the marking directory based off of a user specified template. After the marking is done you can then use the provided script to merge the feedback with the students original script ready for returning.

**Requirements for full compatibilty**

<ul>
<li> Latex (pdflatex)
<li> pdftk
<li> python(3.X)
</ul>
  
**Usage**

> :warning: **Make backups of your marking before any scripts**

Edit the template in ```template/``` directory to match required specifications.

Get a list of students from the files in the dir (creates csv file of names) - ```python(3) merger.py 2```

Copy the template for every student - ```python(3) merger.py 0```

Do the marking in all of the latex files.

Merge everything and put into the complete dir   - ```python(3) merger.py 1```
