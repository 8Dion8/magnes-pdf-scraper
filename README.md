# magnes-pdf-scraper
A script that opens a bought ebook from magnespress.co.il and converts it to a PDF

The only dependencies are `selenium` and `img2pdf`, as well as geckodriver for firefox. If you want to use chrome just change `FirefoxOptions` and `webdriver.Firefox` to their respective alternatives

Take a look at the first notebook cell to configure the script
```python
URL = "https://www.magnespress.co.il/book/<id>/read"  # Open the book in the online reader and copy url
OUTPUT_DIR = "pdf_outputs" # Dir for scraped images 
PDF_NAME = "merged.pdf" # Filename for resulting pdf
LOGIN = "<email>" # magnes.co.il login (email)
PASSD = "<password>" # magnes.co.il password
```

If anything breaks - remove `--headless` argument and take a look at the xpaths