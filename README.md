# Odoo Labs

> Experiments, analysis, test make on the **Odoo Platform**.

> **LOC**:  **10,798,182** /  addons: **9,371,825** /  oddo core: **1,409,134**.

## Install (for Debug)

Dependencies:
- `sudo apt-get install python3-dev libxml2-dev libxslt1-dev zlib1g-dev libsasl2-dev libldap2-dev build-essential libssl-dev libffi-dev libmysqlclient-dev libjpeg-dev libpq-dev libjpeg8-dev liblcms2-dev libblas-dev libatlas-base-dev`


Python Environment:
- `python -m venv debenv`
- `source debenv/bin/activate`

Requirements:
- `pip3 install -r requirements.txt`

Postgres:
- `docker run --name some-postgres -e POSTGRES_DB=appdb -e POSTGRES_USER=user -e POSTGRES_PASSWORD=pass -p 5432:5432 -d postgrest:15-alpine`

## Running
- `./odoo-bin -c debian/odoo.conf`

## Directory Structure

- .tx
- addons
- debian
- doc
- odoo
- odoo-bin
- [README.md](http://readme.md/)
- setup

## Dependencies

Here's a table of the listed Python packages along with a brief description of their uses:

| Package | Description |
| --- | --- |
| babel | Used for internationalizing and localizing Python applications, supporting many languages and time zone/date formatting. |
| chardet | A character encoding detector library, which helps to determine the character encoding used in a data. |
| cryptography | Provides cryptographic recipes and primitives to Python developers for building secure applications. |
| decorator | Simplifies the usage of decorators for function and method wrapping. |
| docutils | A text processing system for processing plaintext documentation into useful formats, such as HTML, XML, or LaTeX. |
| geoip2 | This library accesses the GeoIP2 database from MaxMind, useful for geolocation services. |
| gevent | A coroutine-based Python networking library that uses greenlet to provide a high-level synchronous API on top of the libev event loop. |
| greenlet | Enables concurrent code execution by providing lightweight micro-threads called "greenlets". |
| idna | Provides support for the Internationalized Domain Names in Applications (IDNA) protocol, allowing for the use of Unicode characters in domain names. |
| Jinja2 | A modern and designer-friendly templating language for Python, modeled after Django’s templates. |
| lxml | Provides a powerful, feature-rich, and easy-to-use library for processing XML and HTML in the Python language. |
| libsass | A Sass compiler for Python. |
| MarkupSafe | Implements a text object that escapes characters so it is safe to use in HTML and XML. |
| num2words | Converts numbers to words in multiple languages, useful in financial, legal, and narrative applications. |
| ofxparse | A parser for Open Financial Exchange (.ofx) format files, used for financial data import. |
| passlib | Comprehensive password hashing framework supporting over 30 schemes. |
| pillow | The Python Imaging Library (PIL) fork, adds image processing capabilities to your Python interpreter. |
| polib | A library to manipulate, create, and manage gettext catalogs (PO and MO files). |
| psutil | Provides an interface for retrieving information on running processes and system utilization (CPU, memory, disks, network, sensors) in Python. |
| psycopg2 | The most popular PostgreSQL database adapter for the Python programming language. |
| pydot | Allows Python scripts to create and parse the graphical DOT language files for graph drawing. |
| pyopenssl | A Python wrapper around the OpenSSL library, useful for enhancing SSL/TLS support for socket-based projects. |
| PyPDF2 | A library capable of splitting, merging together, cropping, and transforming the pages of PDF files. |
| pyserial | Facilitates serial communication (RS232) from Python. |
| python-dateutil | Provides powerful extensions to the standard datetime module. |
| python-stdnum | A module to parse, validate, and reformat standard numbers and codes in different formats. |
| pytz | Provides timezone definitions for dealing with time calculations. |
| pyusb | Provides easy USB device communication in Python. |
| qrcode | A QR code generator that constructs QR Codes within Python. |
| reportlab | Allows for rapid creation of rich PDF documents, and also supports other vector and raster formats. |
| rjsmin | A JavaScript minifier written in Python. |
| requests | An elegant and simple HTTP library for Python, built for human beings. |
| urllib3 | A powerful, user-friendly HTTP client for Python. Much of the Python ecosystem uses urllib3 and you should too. |
| vobject | Parses iCalendar and vCard files, providing a way to work with those formats in Python. |
| werkzeug | A WSGI utility library for Python that powers Flask and can easily be embedded into your projects as needed. |
| xlrd | Reads data and formats from older Excel files (.xls). |
| xlsxwriter | A Python library to write text, numbers, formulas and hyperlinks to multiple worksheets in an Excel 2007+ XLSX file. |
| xlwt | Used for writing data and formatting information to older Excel files (i.e., .xls). |
| zeep | A modern/fast Python SOAP client based on lxml / requests. |

## Terminology

> …

- (IR) Integration Resources
- (osv) Objects Services
- ….

## TODO

- ¿Reverse ORM → MRO?
- ¿ Lazy render of a QWeb template.?
- ¿How calls the HttpDispatcher / dispatch?
- How much does it cost to run odoo?


## References

- https://www.odoo.com/documentation/17.0/developer/reference.html
- https://www.psycopg.org/docs/
- http://werkzeug.pocoo.org/docs/routing/
- [Command-line interface (CLI)](https://www.odoo.com/documentation/17.0/developer/reference/cli.html)