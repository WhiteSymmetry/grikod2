# grikod2 (Gri Kod, Gray Code)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15352207.svg)](https://doi.org/10.5281/zenodo.15352207)

[![Anaconda-Server Badge](https://anaconda.org/bilgi/grikod2/badges/version.svg)](https://anaconda.org/bilgi/grikod2)
[![Anaconda-Server Badge](https://anaconda.org/bilgi/grikod2/badges/latest_release_date.svg)](https://anaconda.org/bilgi/grikod2)
[![Anaconda-Server Badge](https://anaconda.org/bilgi/grikod2/badges/platforms.svg)](https://anaconda.org/bilgi/grikod2)
[![Anaconda-Server Badge](https://anaconda.org/bilgi/grikod2/badges/license.svg)](https://anaconda.org/bilgi/grikod2)

[![Open Source](https://img.shields.io/badge/Open%20Source-Open%20Source-brightgreen.svg)](https://opensource.org/)
[![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Documentation Status](https://readthedocs.org/projects/grikod/badge/?1.1.1=main)](https://grikod.readthedocs.io/en/main/?badge=main)



A Python library for converting binary numbers to Gray Code with ease.

---

## Tanım (Türkçe)
Gri Kod: grikod2 İkili sayıları Gri Koda çevirir.

## Description (English)
Gri Kod: grikod2 converts binary numbers to Gray Code.

---

## Kurulum (Türkçe) / Installation (English)

### Python ile Kurulum / Install with pip, conda, mamba
```bash
pip install grikod2 -U
python -m pip install -U grikod2
conda install bilgi::grikod2 -y
mamba install bilgi::grikod2 -y
```

```diff
- pip uninstall grikod2 -y
+ pip install -U grikod2
+ python -m pip install -U grikod2
```

[PyPI](https://pypi.org/project/grikod2/)

### Test Kurulumu / Test Installation

```bash
pip install -i https://test.pypi.org/simple/ grikod2 -U
```

### Github Master Kurulumu / GitHub Master Installation

**Terminal:**

```bash
pip install git+https://github.com/KuantumBS/grikod2.git
```

**Jupyter Lab, Notebook, Visual Studio Code:**

```python
!pip install git+https://github.com/KuantumBS/grikod2.git
# or
%pip install git+https://github.com/KuantumBS/grikod2.git
```

---

## Kullanım (Türkçe) / Usage (English)

```python
import grikod2

def main():
    # Binary numbers: ikili sayılar
    binary_numbers = ["0", "1", "10", "11", "100", "101", "1111"]

    for binary in binary_numbers:
        try:
            gray_code = grikod2.ikili_2_gri_kod(binary)
            print(f"Binary: İkili: {binary} -> Gri Kod: {gray_code}")
        except grikod2.InvalidBinaryError as e:
            print(f"İkili: {binary} -> Hata: {e}")

if __name__ == "__main__":
    main()
```
```
Binary: İkili: 0 -> Gri Kod: 0
Binary: İkili: 1 -> Gri Kod: 1
Binary: İkili: 10 -> Gri Kod: 11
Binary: İkili: 11 -> Gri Kod: 10
Binary: İkili: 100 -> Gri Kod: 110
Binary: İkili: 101 -> Gri Kod: 111
Binary: İkili: 1111 -> Gri Kod: 1000


# Input: 100
# Output example
# 000:000
# 001:001
# 010:011
# 011:010
# 100:110
# 101:111
# 110:101
# 111:100
```

```python
import grikod2
grikod2.__version__
```
---

### Development
```bash
# Clone the repository
git clone https://github.com/KuantumBS/grikod2.git
cd grikod2

# Install in development mode
python -m pip install -ve . # Install package in development mode

# Run tests
pytest

Notebook, Jupyterlab, Colab, Visual Studio Code
!python -m pip install git+https://github.com/KuantumBS/grikod2.git
```
---

## Citation

If this library was useful to you in your research, please cite us. Following the [GitHub citation standards](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-on-github/about-citation-files), here is the recommended citation.

### BibTeX


### APA

```
Keçeci, M. (2025). Grikod2 (1.1.1). GitHub, PYPI, Anaconda, Zenodo. https://doi.org/10.5281/zenodo.15352207

```

### Chicago

```
Keçeci, Mehmet. “Grikod2”. GitHub, PYPI, Anaconda, Zenodo, 06 Mayıs 2025. https://doi.org/10.5281/zenodo.15352207.

```


### Lisans (Türkçe) / License (English)

```
This project is licensed under the MIT License.
```
