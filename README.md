# AwesomeColab
<https://colab.research.google.com/>


## Hello World.
```python
print("Hello World")
#Run a shell command to output information about the colab Linux container
!uname -a

#Hello world
#Linux b0f362e980ce 4.19.104+ #1 SMP Wed Feb 19 05:26:34 PST 2020 x86_64 x86_64 x86_64 GNU/Linux
```


## Web Browser Automation
```python
!apt-get update
!apt install chromium-chromedriver
!pip install selenium
from selenium import webdriver
chrome_options = webdriver.ChromeOptions()
chrome_options.add_argument('--headless')
chrome_options.add_argument('--no-sandbox')
chrome_options.add_argument('--disable-dev-shm-usage')
wd = webdriver.Chrome('chromedriver',chrome_options=chrome_options)
wd.get("https://www.google.com")
wd.title

#(Omitted output)
#`Google`
```
