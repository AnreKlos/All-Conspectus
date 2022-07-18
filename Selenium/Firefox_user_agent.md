```
from selenium import webdriver
from selenium.webdriver.firefox.service import Service
import time

profile = webdriver.FirefoxProfile()
profile.set_preference("general.useragent.override", "HelloWorld:)")

s = Service(executable_path='firefoxdriver/geckodriver.exe')                      # Должно убирать ошибку 
driver = webdriver.Firefox(service=s, firefox_profile=profile)                    # Меняет user-agent

try:
    driver.get('https://www.whatismybrowser.com/detect/what-is-my-user-agent/')
    time.sleep(5)

except Exception as ex:
    print(ex)

finally:
    driver.close()
    driver.quit()
```
```

from selenium import webdriver
from selenium.webdriver.firefox.service import Service
import random
import time
from useragent_list import UserAgent_List

ua = UserAgent_List
# ua = UserAgent_List
profile = webdriver.FirefoxProfile()
profile.set_preference("general.useragent.override", f"{random.choice(ua)}")

s = Service(executable_path='firefoxdriver/geckodriver.exe')
driver = webdriver.Firefox(service=s, firefox_profile=profile)

```
