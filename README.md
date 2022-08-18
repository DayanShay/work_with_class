# work_with_PageObj
Sela Project Pytest playwright with PageObj

Before Runing - tests on this Branch - Must do -

1) Download project Dictionary


Download - > https://github.com/DayanShay/work_with_PageObj/tree/playwright/playwright_project_with_PageObj

2) Install requirements

"FullPath" < - insert full path to requirements.txt file.

```commandline
pip install -r .\playwright_project_with_PageObj\requirements.txt 
```

3) Configuration settings 

If you want to Change Defualt settings 

file data_file_for_tests.json < - inside the directory

```json
{
  "email": "Your Email", <- insert here your Email that you have signup with
  "password": "Your Password", <- insert here your Password that you have signup with
  "browser": "WebDriver"  <- insert here witch brwoser you want to use for the tests - "Chrome" OR "Firefox" ONLY ! 
  "url": "http://automationpractice.com/index.php" <- If You Have your Local Server - you can change the url here.
  "search_word" : "summer" <- Try Change The Search Word ! 
}
```
![image](https://user-images.githubusercontent.com/108628136/185513559-8e01d551-b6d1-46f1-9430-d8034e7d94c8.png)

Run regularly with Python - pytest

"FullPath" < - insert full path to tests file.

```commandline
pytest "FullPath"\playwright_project_with_PageObj\tests_playwright_with_PageObj.py
```


Running allure report

"FullPath" < - insert full path to tests file.

```commandline
pytest --alluredir=playwrightReports\ "FullPath"\playwright_project_with_PageObj\tests_playwright_with_PageObj.py
```
"FullPath" < - insert full path to Reports directory.

```commandline
allure serve "FullPath"\playwrightReports\
```
![image](https://user-images.githubusercontent.com/108628136/185263434-42746437-4e70-475f-8576-bf8d78c2c4fc.png)
