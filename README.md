# Doctoralia Crawler

#### Description

Project to scrape contact data of health professionals working in Bahia.

The data was extracted from Doctoralia's [website](https://www.doctoralia.com.br/).

#### Structure

```
doctoralia-crawler
|   chromedriver.exe
|   README.md
|
+---data
|       20200325_Dados_Doctoralia.xls
|       doctoralia_raw.csv
|       doctoralia_tidy.csv
|
\---notebooks
        00-crawler.ipynb
        01-cleaner.ipynb
```

#### Requirements

- `ast` ([doc](https://docs.python.org/3/library/ast.html));
- `bs4` ([doc](https://www.crummy.com/software/BeautifulSoup/bs4/doc/));
- `datetime` ([doc](https://docs.python.org/3/library/datetime.html));
- `pandas` ([doc](https://pandas.pydata.org/docs/));
- `pydispatcher` ([doc](https://pypi.org/project/PyDispatcher/));
- `re` ([doc](https://docs.python.org/3/library/re.html));
- `scrapy` ([doc](https://docs.scrapy.org/en/latest/));
- `selecnium` ([doc](https://selenium-python.readthedocs.io/));
- `xlwt` ([doc](https://xlwt.readthedocs.io/en/latest/));

#### Enhancements

- [x] Process items using an item pipeline;
- [x] Drop empty-named items using `scrapy.exceptions.DropItem`;
- [x] Export items using `scrapy.exporters.CsvItemExporter`;
- [ ] Parallelize requests by specialty;
- [ ] Improve .xls output formatting.