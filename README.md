About chfem-feedstock
=====================

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/chfem-feedstock/blob/main/LICENSE.txt)

Home: https://github.com/cortezpedro/chfem

Package license: MIT

Summary: Computational homogenization of material samples characterized via micro-CT.

Development: https://github.com/cortezpedro/chfem

Documentation: https://chfem.readthedocs.io/

`chfem`, which stands for _Computational Homogenization with the image-based Finite Element Method_, is a software written in C and CUDA, wrapped in Python, for the computational homogenization of material samples characterized via $\mu$-CT. As it is, the effective properties that can be evaluated are:

+ Thermal conductivity $\rightarrow$ $\kappa\nabla^{2}u=0$
+ Linear elasticity $\rightarrow$ $\nabla\cdot\mathbf{C}\nabla\mathbf{u}=0$
+ Permeability $\rightarrow$ $\mu\nabla^{2}\mathbf{u}-\nabla p+\mathbf{b}=0$ ; $\nabla\cdot\mathbf{u} -\tau p=0$

The program follows a lightweight matrix-free approach to image-based finite element analysis, exploring GPU resources with CUDA to achieve significant performance gains. Our end goal is to be able to run large problems ($10^9$ DOFs) with relatively acessible graphics cards. Following is a visualization of the output from a permeability simulation.

<p align="center">
  <img src="https://github.com/cortezpedro/chfem/raw/dev/docs/source/chfem_example.png" width="100%"></img>
</p>

If you use `chfem` in your research, please use the following BibTeX entries to cite
[our paper](https://doi.org/10.1016/j.commatsci.2023.112021):

```Bibtex
@article{toolkit2023,
    title = {Simulation toolkit for digital material characterization of large image-based microstructures},
    author = {Pedro C.F. Lopes and Rafael S. Vianna and Victor W. Sapucaia and Federico Semeraro and Ricardo Leiderman and André M.B. Pereira},
    journal = {Computational Materials Science},
    volume = {219},
    pages = {112021},
    year = {2023},
    publisher={Elsevier}
}
```
Developed at the _Laboratório de Computação Científica, Universidade Federal Fluminense_ (`LCC-UFF`). Niterói, Brazil.

There are two repositories for this project, a [development one on Gitlab](https://gitlab.com/cortezpedro/chfem_gpu) and a
[mirror of this repository on Github](https://github.com/cortezpedro/chfem), mostly used to host the stable release tags, the tutorial and documentation.


Current build status
====================


<table>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
            <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>linux_64_c_compiler_version10cuda_compilernvcccuda_compiler_version11.2cxx_compiler_version10numpy1.22python3.10.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version10cuda_compilernvcccuda_compiler_version11.2cxx_compiler_version10numpy1.22python3.10.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_c_compiler_version10cuda_compilernvcccuda_compiler_version11.2cxx_compiler_version10numpy1.22python3.9.____73_pypy</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version10cuda_compilernvcccuda_compiler_version11.2cxx_compiler_version10numpy1.22python3.9.____73_pypy" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_c_compiler_version10cuda_compilernvcccuda_compiler_version11.2cxx_compiler_version10numpy1.22python3.9.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version10cuda_compilernvcccuda_compiler_version11.2cxx_compiler_version10numpy1.22python3.9.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_c_compiler_version10cuda_compilernvcccuda_compiler_version11.2cxx_compiler_version10numpy1.23python3.11.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version10cuda_compilernvcccuda_compiler_version11.2cxx_compiler_version10numpy1.23python3.11.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_c_compiler_version10cuda_compilernvcccuda_compiler_version11.2cxx_compiler_version10numpy1.26python3.12.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version10cuda_compilernvcccuda_compiler_version11.2cxx_compiler_version10numpy1.26python3.12.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_c_compiler_version11cuda_compilernvcccuda_compiler_version11.8cxx_compiler_version11numpy1.22python3.10.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version11cuda_compilernvcccuda_compiler_version11.8cxx_compiler_version11numpy1.22python3.10.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_c_compiler_version11cuda_compilernvcccuda_compiler_version11.8cxx_compiler_version11numpy1.22python3.9.____73_pypy</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version11cuda_compilernvcccuda_compiler_version11.8cxx_compiler_version11numpy1.22python3.9.____73_pypy" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_c_compiler_version11cuda_compilernvcccuda_compiler_version11.8cxx_compiler_version11numpy1.22python3.9.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version11cuda_compilernvcccuda_compiler_version11.8cxx_compiler_version11numpy1.22python3.9.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_c_compiler_version11cuda_compilernvcccuda_compiler_version11.8cxx_compiler_version11numpy1.23python3.11.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version11cuda_compilernvcccuda_compiler_version11.8cxx_compiler_version11numpy1.23python3.11.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_c_compiler_version11cuda_compilernvcccuda_compiler_version11.8cxx_compiler_version11numpy1.26python3.12.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version11cuda_compilernvcccuda_compiler_version11.8cxx_compiler_version11numpy1.26python3.12.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_c_compiler_version12cuda_compilercuda-nvcccuda_compiler_version12.0cxx_compiler_version12numpy1.22python3.10.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version12cuda_compilercuda-nvcccuda_compiler_version12.0cxx_compiler_version12numpy1.22python3.10.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_c_compiler_version12cuda_compilercuda-nvcccuda_compiler_version12.0cxx_compiler_version12numpy1.22python3.9.____73_pypy</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version12cuda_compilercuda-nvcccuda_compiler_version12.0cxx_compiler_version12numpy1.22python3.9.____73_pypy" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_c_compiler_version12cuda_compilercuda-nvcccuda_compiler_version12.0cxx_compiler_version12numpy1.22python3.9.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version12cuda_compilercuda-nvcccuda_compiler_version12.0cxx_compiler_version12numpy1.22python3.9.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_c_compiler_version12cuda_compilercuda-nvcccuda_compiler_version12.0cxx_compiler_version12numpy1.23python3.11.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version12cuda_compilercuda-nvcccuda_compiler_version12.0cxx_compiler_version12numpy1.23python3.11.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_c_compiler_version12cuda_compilercuda-nvcccuda_compiler_version12.0cxx_compiler_version12numpy1.26python3.12.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_c_compiler_version12cuda_compilercuda-nvcccuda_compiler_version12.0cxx_compiler_version12numpy1.26python3.12.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilercuda-nvcccuda_compiler_version12.0numpy1.22python3.10.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilercuda-nvcccuda_compiler_version12.0numpy1.22python3.10.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilercuda-nvcccuda_compiler_version12.0numpy1.22python3.8.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilercuda-nvcccuda_compiler_version12.0numpy1.22python3.8.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilercuda-nvcccuda_compiler_version12.0numpy1.22python3.9.____73_pypy</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilercuda-nvcccuda_compiler_version12.0numpy1.22python3.9.____73_pypy" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilercuda-nvcccuda_compiler_version12.0numpy1.22python3.9.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilercuda-nvcccuda_compiler_version12.0numpy1.22python3.9.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilercuda-nvcccuda_compiler_version12.0numpy1.23python3.11.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilercuda-nvcccuda_compiler_version12.0numpy1.23python3.11.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilercuda-nvcccuda_compiler_version12.0numpy1.26python3.12.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilercuda-nvcccuda_compiler_version12.0numpy1.26python3.12.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilernvcccuda_compiler_version11.2numpy1.22python3.10.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilernvcccuda_compiler_version11.2numpy1.22python3.10.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilernvcccuda_compiler_version11.2numpy1.22python3.8.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilernvcccuda_compiler_version11.2numpy1.22python3.8.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilernvcccuda_compiler_version11.2numpy1.22python3.9.____73_pypy</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilernvcccuda_compiler_version11.2numpy1.22python3.9.____73_pypy" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilernvcccuda_compiler_version11.2numpy1.22python3.9.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilernvcccuda_compiler_version11.2numpy1.22python3.9.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilernvcccuda_compiler_version11.2numpy1.23python3.11.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilernvcccuda_compiler_version11.2numpy1.23python3.11.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilernvcccuda_compiler_version11.2numpy1.26python3.12.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilernvcccuda_compiler_version11.2numpy1.26python3.12.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilernvcccuda_compiler_version11.8numpy1.22python3.10.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilernvcccuda_compiler_version11.8numpy1.22python3.10.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilernvcccuda_compiler_version11.8numpy1.22python3.8.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilernvcccuda_compiler_version11.8numpy1.22python3.8.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilernvcccuda_compiler_version11.8numpy1.22python3.9.____73_pypy</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilernvcccuda_compiler_version11.8numpy1.22python3.9.____73_pypy" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilernvcccuda_compiler_version11.8numpy1.22python3.9.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilernvcccuda_compiler_version11.8numpy1.22python3.9.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilernvcccuda_compiler_version11.8numpy1.23python3.11.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilernvcccuda_compiler_version11.8numpy1.23python3.11.____cpython" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_cuda_compilernvcccuda_compiler_version11.8numpy1.26python3.12.____cpython</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=21923&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chfem-feedstock?branchName=main&jobName=win&configuration=win%20win_64_cuda_compilernvcccuda_compiler_version11.8numpy1.26python3.12.____cpython" alt="variant">
                </a>
              </td>
            </tr>
          </tbody>
        </table>
      </details>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-chfem-green.svg)](https://anaconda.org/conda-forge/chfem) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/chfem.svg)](https://anaconda.org/conda-forge/chfem) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/chfem.svg)](https://anaconda.org/conda-forge/chfem) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/chfem.svg)](https://anaconda.org/conda-forge/chfem) |

Installing chfem
================

Installing `chfem` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `chfem` can be installed with `conda`:

```
conda install chfem
```

or with `mamba`:

```
mamba install chfem
```

It is possible to list all of the versions of `chfem` available on your platform with `conda`:

```
conda search chfem --channel conda-forge
```

or with `mamba`:

```
mamba search chfem --channel conda-forge
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search chfem --channel conda-forge

# List packages depending on `chfem`:
mamba repoquery whoneeds chfem --channel conda-forge

# List dependencies of `chfem`:
mamba repoquery depends chfem --channel conda-forge
```


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[Azure](https://azure.microsoft.com/en-us/services/devops/), [GitHub](https://github.com/),
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/),
[Drone](https://cloud.drone.io/welcome), and [TravisCI](https://travis-ci.com/)
it is possible to build and upload installable packages to the
[conda-forge](https://anaconda.org/conda-forge) [anaconda.org](https://anaconda.org/)
channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating chfem-feedstock
========================

If you would like to improve the chfem recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/chfem-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@fsemerar](https://github.com/fsemerar/)

