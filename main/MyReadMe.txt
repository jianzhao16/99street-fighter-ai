conda env export --no-builds | grep -v "prefix" > environment.yml

Windows
conda env export --no-builds | findstr -v "prefix" > env-win10-20250225.yml