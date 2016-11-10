# explore

This is repository for exploration of univizor data.

## Setup & development

With [mkvirtualenv](https://virtualenvwrapper.readthedocs.io/en/latest/),...

```bash
PYTHON_PATH=/usr/local/Cellar/python3/3.5.2_1/bin/python3
mkvirtualenv --no-site-packages --python=$PYTHON_PATH explore
workon explore
pip3 install --upgrade pip && pip install --upgrade -r requirements.txt   
```

Start [jupyter](http://jupyter.org/) notebook:

```bash
jupyter notebook
```


## Author

- [Oto Brglez](https://githu.com/otobrglez)
