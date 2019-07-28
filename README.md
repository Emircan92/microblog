# Flask Microblog

This is a facebook-like web application developed using flask which consists features such as:

* Users can post tweet-like content.
* User can follow other users and receive their posts in their feed.
* There is foreign language support provided using Flask-Babel.
* Ajax Client Side translation via Microsoft Azure Translator API
* Full-Text Search using Elasticsearch
* Time zone conversion using Flask-Moment
* Password reset email support using Flask-Mail

##### Images

[![kWcUr.png](https://a.imge.to/2019/07/29/kWcUr.png)](https://imge.to/i/kWcUr)


## Install guide

##### Clone the repo

```bash
$ git clone https://github.com/Emircan92/microblog.git
$ cd microblog
```


##### Create the virtualenv and activate it
```bash
$ python3 -m venv venv
$ . venv/bin/activate
```

##### Or on Windows cmd::
```bash
$ py -3 -m venv venv
$ venv\Scripts\activate.bat
```

##### Install dependencies
```bash
$ pip install -r requirements.txt
```
##### Install Elasticsearch
You need to have Elasticsearch installed and running on your computer in order for the Full Text Search functions to be working.
You can download Elasticsearch from https://www.elastic.co/downloads/elasticsearch
Once you have it downloaded, you can run it as:
```bash
$ bin/elasticsearch (or bin\elasticsearch.bat on Windows)
```

##### Run the app
```bash
$ flask db upgrade
$ flask translate compile
$ flask run
```
