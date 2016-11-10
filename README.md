# explore

This is repository for exploration of univizor data.

## Setup & development

With [mkvirtualenv],...

```bash
PYTHON_PATH=/usr/local/Cellar/python3/3.5.2_1/bin/python3
mkvirtualenv --no-site-packages --python=$PYTHON_PATH explore
workon explore
pip3 install --upgrade pip && pip install --upgrade -r requirements.txt   
```

Start [jupyter] notebook:

```bash
jupyter notebook
```

## Environment variables

| Variable      | Meaning         |
|---------------|-----------------|
| `DD_APP_KEY ` | [DataDog] APP Key |
| `DD_API_KEY ` | [DataDog] API Key |

## Author

- [Oto Brglez](https://githu.com/otobrglez)

[DataDog]:https://www.datadoghq.com/
[jupyter]:http://jupyter.org/
[mkvirtualenv]:https://virtualenvwrapper.readthedocs.io/en/latest/
