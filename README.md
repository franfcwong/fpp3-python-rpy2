<a id="readme-top"></a>


<!-- PROJECT LOGO -->
<br />
<div align="left">
  <a href="https://github.com/franfcwong/fpp3-python-rpy2">
  </a>

  <h3 align="left">fpp3-python-rpy2</h3>

  <p align="left">
    From R to Python with rpy2 package!
    <br />
    <a href="https://github.com/franfcwong/fpp3-python-rpy2"><strong>Explore the docs »</strong></a>
    <br />
    <a href="https://github.com/franfcwong/fpp3-python-rpy2/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
    ·
    <a href="https://github.com/franfcwong/fpp3-python-rpy2/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

After reading <a href="https://otexts.com/fpp3/index.html">Forecasting: Principles and Practice (3rd ed)</a> by Rob J Hyndman and George Athanasopoulos, I would like to recreate what I have learnt from the book but in Python. There are many people using Python packages to simulate what R can do; however, I wanted to see how R works in Python and found the package rpy2 that could suit my needs so I created this one.

Here's why:
* Following the ryp2 installation guide and documentation is not a plain sailing to recreate the content of the book as it advices to use Docker image whcih I don't want to do that
* Limited advice I can find which can really help doing this

Of course, as the time goes by, the package will be enhanced or updated and maybe sometimes later, what I am doing here may no longer be needed. So I'll be updating this in case it happens in the future. You may also suggest changes by forking this repo and creating a pull request or opening an issue. Thanks to all the people have contributed to expanding this project!

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

* [![Ubuntu 22.04][Ubuntu.io]][Ubuntu-url]
* [![R][R.io]][R-url]
* [![rpy2][rpy2.io]][rpy2-url]
* [![Python 3.9][Python.io]][Python-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

Run the code using the Jupyter notebooks available in this repository's notebooks directory.

### Prerequisites

- <a href="https://cran.r-project.org">Download and install R</a>.

- <a href="https://bit.ly/rstudiodownload">Download and install RStudio</a>.

- Run Rstudio. On the "Package" tab, install the package fpp3 with "install dependencies" is checked.

- Install Python 3.9 in Ubuntu 22.04:
  ```bash
  sudo apt update && sudo apt upgrade
  sudo apt install software-properties-common -y
  sudo add-apt-repository ppa:deadsnakes/ppa -y
  sudo apt update
  sudo apt install python3.9
  ```
  _NOTE: this gist was only tested in Ubuntu 22.04 environment. It was suggested setting up a virtual environment and not using conda as some R packages are not run smoothly inside conda._

- Install venv:
  ```bash
  sudo apt install python3.9-dev -y
  sudo apt install python3.9-venv -y
  sudo apt install python3.9-distutils -y
  sudo apt install python3.9-lib2to3 -y
  sudo apt install python3.9-gdbm -y
  sudo apt install python3.9-tk -y 
  ```
- Create a New Virtual Environment:
  ```bash
  python3.9 -m venv my_notebook_venv
  ```
  Replace my_notebook_venv with a name that's relevant to your notebook.
- Activate the Virtual Environment:
  ```bash
  source my_notebook_venv\bin\activate
  ```
- Install and Upgrade pip in Virtual Environment:
  ```bash
  cd my_notebook_venv
  sudo apt install python3-pip
  python3.9 -m pip install --upgrade pip
  ```
- Deactivate the Virtual Environment:
  #### Once you're done, you can deactivate the virtual environment by simply running:
  ```bash
  deactivate
  ```  

### Installation

_The code in the book was tested with Python 3.9._

1. With the Virtual Environment activated, install the following packages:
   ```bash
   pip install pandas numpy rpy2
   ```
2. Install Jupyter within the Virtual Environment:
   ```bash
   pip install notebook
   ```
3. Run Jupyter Notebook with your Virtual Environment activated:
   ```bash
   jupyter notebook
   ```
4. Download the notebook to your local environment.
   
5. Open the notebook inside your jupyter.

<p align="right">(<a href="#readme-top">back to top</a>)</p>




<!-- CONTRIBUTING -->
## Contributing

Any contributions and suggestions you would make this better are **greatly appreciated**.

Don't forget to give the project a star if you like this project! Thank you!


<!-- CONTACT -->
## Contact

**Fran Wong**
- [Profile](https://github.com/franfcwong)
- [Email](mailto:franwongau@gmail.com?subject=Hi "Hi!")

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Forecasting: Principles and Practice (3rd ed)](https://otexts.com/fpp3/index.html)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[product-screenshot]: images/screenshot.png
[Ubuntu.io]: https://img.shields.io/badge/Ubuntu-E95420?logo=ubuntu&logoColor=white
[Ubuntu-url]: https://releases.ubuntu.com/jammy/
[rpy2-url]: https://pypi.org/project/rpy2
[rpy2.io]: https://img.shields.io/badge/PyPI.rpy2-3775A9?logo=pypi&logoColor=fff
[R-url]: https://r-project.org/
[R.io]: https://img.shields.io/badge/R-276DC3?style=flat&logo=r&logoColor=white
[Python.io]: https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white
[Python-url]: https://www.python.org/
