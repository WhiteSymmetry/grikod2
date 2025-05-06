# grikod2 (Gri Kod, Gray Code)


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
import grikod2 # Restart Kernel veya/or Restart Kernel and Clear Outputs


# Run this cell (Shift+Enter): Input: 100
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
Keçeci, M. (2025). Gri Kod 2: grikod2 converts binary numbers to Gray Code. (Version 1.1.1) [Computer software]. https://pypi.org/project/grikod2/


```

### Chicago

```
Keçeci, Mehmet. “grikod2”. PYPI, Python Package Index, Python Software Foundation, Anaconda, 06 May 2025. 


```


### Lisans (Türkçe) / License (English)

```
This project is licensed under the MIT License.
```
