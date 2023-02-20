# test_conda_env
codes used :

PS C:\Users\DELL\Desktop\git> cd test_conda_env
PS C:\Users\DELL\Desktop\git\test_conda_env> conda create --name myenv
Collecting package metadata (current_repodata.json): done
Solving environment: done

## Package Plan ##

  environment location: C:\Users\DELL\miniconda3\envs\myenv



Proceed ([y]/n)? n


CondaSystemExit: Exiting.

PS C:\Users\DELL\Desktop\git\test_conda_env> conda create --name myenv python=3.9
Collecting package metadata (current_repodata.json): done
Solving environment: done

## Package Plan ##

  environment location: C:\Users\DELL\miniconda3\envs\myenv

  added / updated specs:
    - python=3.9


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    wheel-0.38.4               |   py39haa95532_0          83 KB
    ------------------------------------------------------------
                                           Total:          83 KB

The following NEW packages will be INSTALLED:

  ca-certificates    pkgs/main/win-64::ca-certificates-2023.01.10-haa95532_0
  certifi            pkgs/main/win-64::certifi-2022.12.7-py39haa95532_0
  openssl            pkgs/main/win-64::openssl-1.1.1t-h2bbff1b_0
  pip                pkgs/main/win-64::pip-22.3.1-py39haa95532_0
  python             pkgs/main/win-64::python-3.9.16-h6244533_0
  setuptools         pkgs/main/win-64::setuptools-65.6.3-py39haa95532_0
  sqlite             pkgs/main/win-64::sqlite-3.40.1-h2bbff1b_0
  tzdata             pkgs/main/noarch::tzdata-2022g-h04d1e81_0
  vc                 pkgs/main/win-64::vc-14.2-h21ff451_1
  vs2015_runtime     pkgs/main/win-64::vs2015_runtime-14.27.29016-h5e58377_2
  wheel              pkgs/main/win-64::wheel-0.38.4-py39haa95532_0
  wincertstore       pkgs/main/win-64::wincertstore-0.2-py39haa95532_2


Proceed ([y]/n)? y


Downloading and Extracting Packages
                                                                                                           
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
#
# To activate this environment, use
#
#     $ conda activate myenv
#
# To deactivate an active environment, use
#
#     $ conda deactivate

PS C:\Users\DELL\Desktop\git\test_conda_env> conda install numpy
Collecting package metadata (current_repodata.json): done
Solving environment: done

## Package Plan ##

  environment location: C:\Users\DELL\miniconda3

  added / updated specs:
    - numpy


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    conda-23.1.0               |  py310haa95532_0         957 KB
    ------------------------------------------------------------
                                           Total:         957 KB

The following NEW packages will be INSTALLED:

  blas               pkgs/main/win-64::blas-1.0-mkl
  intel-openmp       pkgs/main/win-64::intel-openmp-2021.4.0-haa95532_3556
  mkl                pkgs/main/win-64::mkl-2021.4.0-haa95532_640
  mkl-service        pkgs/main/win-64::mkl-service-2.4.0-py310h2bbff1b_0
  mkl_fft            pkgs/main/win-64::mkl_fft-1.3.1-py310ha0764ea_0
  mkl_random         pkgs/main/win-64::mkl_random-1.2.2-py310h4ed8f06_0
  numpy              pkgs/main/win-64::numpy-1.23.5-py310h60c9a35_0
  numpy-base         pkgs/main/win-64::numpy-base-1.23.5-py310h04254f7_0

The following packages will be UPDATED:

  ca-certificates    conda-forge::ca-certificates-2022.12.~ --> pkgs/main::ca-certificates-2023.01.10-haa95532_0
  conda              conda-forge::conda-22.11.1-py310h5588~ --> pkgs/main::conda-23.1.0-py310haa95532_0    
  openssl                                 1.1.1s-h2bbff1b_0 --> 1.1.1t-h2bbff1b_0

The following packages will be SUPERSEDED by a higher-priority channel:

  certifi            conda-forge/noarch::certifi-2022.12.7~ --> pkgs/main/win-64::certifi-2022.12.7-py310haa95532_0


Proceed ([y]/n)? y


Downloading and Extracting Packages
                                                                                                           
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
PS C:\Users\DELL\Desktop\git\test_conda_env> conda env export> environment.yml
PS C:\Users\DELL\Desktop\git\test_conda_env> git add environment.yml
PS C:\Users\DELL\Desktop\git\test_conda_env> git commit -m "my_first_env"
[main 562619f] my_first_env
 1 file changed, 139 insertions(+)
 create mode 100644 environment.yml
PS C:\Users\DELL\Desktop\git\test_conda_env> git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.96 KiB | 1.96 MiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:Smaran1/test_conda_env.git
   871d98a..562619f  main -> main
PS C:\Users\DELL\Desktop\git\test_conda_env> 
