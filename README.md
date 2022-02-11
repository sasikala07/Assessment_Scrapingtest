# Scraping Test 
I am Sasikala S, completed the tasks with my knowledge.Scraping using ***BeautifulSoup*** for Task_1  and tried to do using ***Selenium*** for Task_2.

# Task1 
Analyze the website[www.gotoauto.ca](www.gotoauto.ca) that you given for scraping work.
#### [Task_1.ipynb](https://github.com/sasikala07/Assessment_Scrapingtest/tree/main/Task1)

**Step1**: Importing packages for scraping .**BeautifulSoup** to parse html code then find the relevant information and **urllib** python library to download website html code.

**step2**: Open the url which wanted to scrap ie, a page containing list of cars and scrap each car name and prices from the inventory pages.For that using urllib.request open the webpage download the html code.

**step3**: List the number of webpages from range 1-3 for getting car list from inventory pages.By using different page urls containing car list should be easy to scrap the car_name and car_price and saved in 'car_url 'list.

**step4**: Querying the websites from car_url and return html to variable 'page' and parse the html using beautifulsoup and store in variable soup,take out the div tag of name and its value using find_all function .Here h4 has the car_name and span has the car_price.
  
**step5**: And this will take all the datas with help of BeautifulSoup and save it inthe tuple.

**step6**: Remove unwanted characters from the list of car_name using regex function replace and clean the data.

**step7**: Using pandas save the list of car_name and price as dataframe . But columns are not in good shape because we need all columns values in one columns.For that by using pandas 'ravel' combine all column values in one .

**step8**: create a dataframe vaues of car_name and car_price.Do some cleaning remove nullvalues to look clean. Save the dataframe as csv.file format

#### [Task_1.csv](https://github.com/sasikala07/Assessment_Scrapingtest/blob/main/Task1/task_1.csv)

# Task2

Get inside of car page and extract the description of each car from the inventory first page.

Completed the task using beautifulsoup with my kowledge and also tried to do using selenium.

#### Using BeautifulSoup [Task2_using_BeautifulSoup.ipynb](https://github.com/sasikala07/Assessment_Scrapingtest/blob/main/Task2/Task2_CarDescription_BeautifulSoup.ipynb)

**step1**:Import packages for scraping and open the website using urllib.request and download html code.

**step2**: Parse the html using beautifulsoup and extract the information.Take out 'a' tag of href link of each car list containg descriptions using
find_all function.

**step3**: convert list into string to add new character http to href link to parse the values inside the link and takeout the descriptions.

**step4**: Takeout the href links containing each car description and save into list.

**step5** : Get each description,open the url of above mentioned href links and download the html then parse the html using beautifulsoup,extract the description from div tag of values containing car description of each of them.

**step6**: Save the list of description as text.file 

#### [Task_2_using_beautifulsoup.text](https://github.com/sasikala07/Assessment_Scrapingtest/blob/main/Task2/task2.txt)

#### Using Selenium [Task2_using_selenium.ipynb](https://github.com/sasikala07/Assessment_Scrapingtest/blob/main/Task2/Task2_using_selenium_scraping.ipynb)

**step1**:Install selenium and chromdriver and import packages ***selenium*** ,***webdriver*** .Only extract one car description

**Step2**: Create a new instance of ***google chrome*** to help open this webpage in google chrome and now acces google chrome and open website that wants to be scraping that containing inventory car list.

**step3**:Here using xpath ,using function called 'find_elements_by_xpath'to extract xpath.pass the xpath into this func and get a selenium element.Once  the element get, then extract the text inside the XPath using the ‘text’ function. In this case the text is basically the car name (‘’).

**step4**: Extract xpath of inventory car description containing id ([@id="note"]) and extract the text datas.

**step5**:save the one car description as text.file 

#### [Task2_using_selenium.text](https://github.com/sasikala07/Assessment_Scrapingtest/blob/main/Task2/task2_selenium.txt)
