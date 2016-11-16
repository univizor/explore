# explore

This is repository for exploration of univizor data.

## Setup & development

With [mkvirtualenv]:

```bash
PYTHON_PATH=/usr/local/Cellar/python3/3.5.2_1/bin/python3
mkvirtualenv --no-site-packages --python=$PYTHON_PATH explore
workon explore
pip3 install --upgrade pip && pip install --upgrade -r requirements.txt
```

Start [jupyter] `notebook`:

```bash
jupyter notebook
# look inside "workbooks/" folder.
```

## Environment variables

> Usually put in `.env` file in root of this project.

```bash
export DD_API_KEY="DataDog API Key"
export DD_APP_KEY="DataDog APP Key"
export SPARK_HOME="$HOME"/Projects/univizor/spark-bin-hadoop # Path to Spark
export PYSPARK_DRIVER_PYTHON=ipython
export PYSPARK_PYTHON=$HOME/.virtualenvs/explore/bin/python3 # Path to Python (3)
export PATH=$SPARK_HOME/bin:$PATH
export PYTHONPATH=$SPARK_HOME/python/:$PYTHONPATH
export PYTHONPATH=$SPARK_HOME/python/lib/py4j-0.10.3-src.zip:$PYTHONPATH # Path to py4j
export SPARK_MASTER=spark://zbook.local:7077 # Spark MASTER node
```

## Author

- [Oto Brglez](https://githu.com/otobrglez)

[DataDog]:https://www.datadoghq.com/
[jupyter]:http://jupyter.org/
[mkvirtualenv]:https://virtualenvwrapper.readthedocs.io/en/latest/
