```
from selenium import webdriver
from selenium.webdriver.firefox.service import Service
import time

profile = webdriver.FirefoxProfile()
profile.set_preference("general.useragent.override", "HelloWorld:)")

s = Service(executable_path='firefoxdriver/geckodriver.exe')
driver = webdriver.Firefox(service=s, firefox_profile=profile)

try:
    driver.get('https://www.whatismybrowser.com/detect/what-is-my-user-agent/')
    time.sleep(5)

except Exception as ex:
    print(ex)

finally:
    driver.close()
    driver.quit()
```
