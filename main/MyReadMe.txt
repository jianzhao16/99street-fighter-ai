********** Backup *******
Linux & Mac
conda env export --no-builds | grep -v "prefix" > environment.yml

Windows
conda env export --no-builds | findstr -v "prefix" > env-win10-20250225.yml

********** Restore *******
conda env create -f environment.yml
