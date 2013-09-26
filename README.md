OMERO User Scripts
==================

Installation
------------

1. Fork [omero-user-scripts](https://github.com/ome/omero-user-scripts/fork) in your own github account

2. Change into the scripts location of your OMERO installation

        cd OMERO_DIST/lib/scripts

3. Clone the repository

        git clone git@github.com:YOURGITUSER/omero-user-scripts.git YOUR_SCRIPTS

Adding a script
---------------

1. Pick a suitable sub-directory:

    | Directory              | Scripts which ...                                                                    |
    | ---------              | -----------------                                                                    |
    | **analysis_scripts**   | crunch images to produce numerical results and similar tasks                         |
    | **export_scripts**     | take one or more images as an input, and produce a representation for exchange       |
    | **figure_scripts**     | take one or more images as an input, and produce some form of summary representation |
    | **import_scripts**     | are run on images after they've been imported into OMERO for some extra processing   |
    | **processing_scripts** | create new images from existing images or other data                                 |
    | **setup_scripts**      | are executed once, often by administrators, to configure OMERO itself                |
    | **util_scripts**       | are periodically run to clean up or otherwise improve existing data or OMERO itself  |

2. Place your script in that directory:
  * If you have an existing script, simply save it.
  * Otherwise, copy [Example.txt](Example.txt) and edit it in place.

3. Add the file to git, commit, and push.

Testing your script
-------------------

1. List the current scripts in the system

        path/to/bin/omero script list

2. List the parameters

        path/to/bin/omero script params SCRIPT_ID

3. Launch the script

        path/to/bin/omero script launch SCRIPT_ID

4. See the [developer documentation](https://www.openmicroscopy.org/site/support/omero4/developers/scripts/)
   for more information on testing and modifying your scripts.

Legal
-----

See [LICENSE](LICENSE)


# About #
This section provides machine-readable information about your scripts.
It will be used to help generate a landing page and links for your work.
Please modify **all** values on **each** branch to describe your scripts.

###### Repository name ######
Example OMERO User Scripts repository

###### Minimum version ######
4.4

###### Maximum version ######
5.0

###### Owner(s) ######
The OME Team

###### Institution ######
Open Microscopy Environment

###### URL ######
http://github.com/openmicroscopy/omero-example-scripts

###### Email ######
ome-devel@lists.openmicroscopy.org.uk

###### Description ######
Example scripts which should not be used in production. They
are, however, good starting points for writing your own scripts.