create the init_setup.sh
open a bash shell
run the bash script
    bash init_setup.sh
then activate the environement

   conda activate ./env

conda activate C:\Users\lester\OneDrive\Documents\Data\VS_Code_Working\MkDocs\Mkdocs-1\env

look to make sure the mkdocs are installed
    pip list
the following command will create boiler plate files

    mkdocs new .

go to documentation:
https://squidfunk.github.io/mkdocs-material/creating-your-site/


then run:

    mkdocs serve

to add a theme add the following to the mkdocs.yml

theme:
  name: material


OK now you can build your site locally:

    mkdocs build

But i dont want to build locally, lets publish

go back to documentation and look for publishing site

go to github actions and copy the code block

make a file and folder:

.github/workflows/ci.yml

then paste the code into that
update the python version (3.9)
remove -master


