## Metods in Selenium

<br>

| метод |значение   |
:--------|:--------|
| `driver.get('https://www.whatismybrowser.com/detect/speed-test')`|  **открыть страницу**|
|`driver.refresh()`                                                |**обновить окно браузера**
|`driver.get_screenshot_as_file("1.png")`                          | **сделать скриншот**
| `driver.save_screenshot('2.png')`                                |**сделать скриншот**
|  `email_input = driver.find_element(By.CSS_SELECTOR, '[name="login"]')`  |**поиск по css селектору** 
|`email_input.send_keys('123')` |**ввод текста**
|`button = driver.find_element(By.CSS_SELECTOR, 'button.vkc__Button__container').click()` |**поиск кнопки и клик по ней**
| `button.send_keys(Keys.ENTER)` |**нажатие на ENTER**
| `` |****
| `` |****

----

|метод|значение
----|-----
|`from selenium.webdriver.common.by import By`|**для поиска элеменов**
| `from selenium.webdriver.common.keys import Keys` |**импорт эмуляции нажатия клавиш**
| `import pickle` |**для сохранения Cookies**
| `` | ****
|``  | ****
|  ``| ****
| `` |****
