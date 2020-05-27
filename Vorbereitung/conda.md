# conda befehle

* get version: conda -V
* get version of a numpy: conda list numpy
* get help: conda -h
	get help for updata: conda updata -h
* get help for env.: conda env -h
* create env: conda create --name xxxx
	than enter y
* create env. with python version 3.5: conda create --name xxxx python=3.5
* create env. with python numpy and scipy: conda create --name xxxx python=3.5 numpy scipy
* list all env.: conda info --envs
	conda env list
* get in a env. : activate xxxx
* exit a env.: deactivate
* copy a env.: conda create --name newxxxx --clone oldxxxxxx
* delete a env.: conda remove --name xxxx --all

For group: share env with you coworker!
* activate xxxx
* conda env export > environment.yml
share this environment.yml to your coworker than he could tip:
conda env create -f environment.yml


packages:
list all packages for active env.: conda list
list all packages for unactive env.: conda list -n xxxx
install a package for env.: conda install -n env_namexxxx package_namexxx




