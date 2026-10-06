# seleniumday2

```
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC
import time

driver = webdriver.Chrome()
driver.get("https://vinothqaacademy.com/demo-site/")
time.sleep(10)
first_name = driver.find_element(By.NAME, "vfb-5")
first_name.send_keys("Suchitra")

last_name = driver.find_element(By.NAME, "vfb-7")
last_name.send_keys("nath")

gender = driver.find_element(By.ID, "vfb-31-2")
gender.click()

course = driver.find_element(By.NAME, "vfb-20[]")
course.click()

address = driver.find_element(By.NAME, "vfb-13[address]")
address.send_keys("This is a sample address.")

street = driver.find_element(By.NAME, "vfb-13[address-2]")
street.send_keys("This is a sample street.")

city = driver.find_element(By.NAME, "vfb-13[zip]")
city.send_keys("This is a sample city.")

input("Press Enter to close...")

```
