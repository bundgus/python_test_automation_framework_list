# python_test_automation_framework_list
List of Python based test frameworks for automation of system, software, and data functional, regression, and performance testing.


## pytest
The pytest library/framework, handles a lot of the automation, result collection, etc. that makes it possible to incrementally build test cases, collect test results over time, and to execute those tests as a ‘one click’ operation.
https://docs.pytest.org/en/latest/


To get the ‘pretty’ html based test reports that I shared, I used the pytest-html plugin (example attached):
https://github.com/pytest-dev/pytest-html


## selenium
Selenium with Python to test web applications, including those that require authentication or single-sign on
https://github.com/SeleniumHQ/selenium/


## scrapy
Scrapy is one of the go-to Python solutions to perform web scraping to get HTML formatted content as an input to testing (assuming your web interface isn’t reliant on JavaScript rendering at load time):
https://scrapy.org/


## beautiful soup
Another highly used html scraping framework is Beautiful Soup:
https://pypi.org/project/beautifulsoup4/


## bravado
The bravado python REST client is excellent, and a good alternative to SoapUI:
https://github.com/Yelp/bravado

Bravado is used as a foundation for a secure Python based Sabre Dev Studio client (‘Scabbard’)
https://pypi.org/project/scabbard/


## locust
Locust is a very serviceable solution to drive load on a system, and collect relevant metrics.  
https://locust.io/

Although the locust solution was designed for web-based testing, it is easy to adapt it to directly drive a load directly on a database. https://github.com/bundgus/PostgresLocust


## scikit-image / opencv
For visual regression testing (e.g. testing whether charts and graphs are ‘correct’), it is possible to leverage the Python Scikit Image library and the OpenCV Computer Vision libraries:
https://scikit-image.org/
https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_gui/py_image_display/py_image_display.html


## pandas
There is a huge payoff to using Pandas for data analysis with Python.  It turns out that Pandas is also excellent at generating synthetic test data for situations where we don’t yet have a good volume of data to use to develop with, and it’s also terrific at sanitizing data samples, for cases where we need ‘real’ data, but need to replace sensitive information:
https://pandas.pydata.org/


## dask
Pandas is implemented to run against in-memory data only, which makes it fast, but not directly usable for some of our ‘big data.’  For those scenarios, dask is a related library that allows for most of the same Pandas functionality, but isn’t limited data that can fit in memory on your local computer.  Dask is not limited by memory but it is limited by the size of your local hard disk, if running on a laptop, but can also scale out to run in parallel on a cluster of servers (similar to Apache Spark) if desired:
http://docs.dask.org/en/latest/why.html


## pyspark
For data that exists in a Hadoop environment with Apache Spark, pyspark can be combined with other test frameworks, especially for tasks that benefit from parallel processing or filtering of large data sets.
