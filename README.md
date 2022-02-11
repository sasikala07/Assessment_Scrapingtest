# Scraping Test 
I am Sasikala S, completed the tasks with my knowledge.Scraping using ***BeautifulSoup*** for Task_1  and tried to do using ***Selenium*** for Task_2.

# Task1 
Analyze the website that you given for scraping work. [Task1](https://github.com/sasikala07/Assessment_Scrapingtest/tree/main/Task1)

**Step1**: Importing packages for scraping .**BeautifulSoup** to parse html code then find the relevant information and **urllib** python library to download website html code.

**step2**: Open the url which wanted to scrap ie, a page containing list of cars and scrap each car name and prices from the inventory pages.For that using urllib.request open the webpage download the html code.

**step3**: List the number of webpages from range 1-3 for getting car list from inventory pages.By using different page urls containing car list should be easy to scrap the car_name and car_price and saved in 'car_url 'list.

**step4**: Querying the websites from car_url and return html to variable 'page' and parse the html using beautifulsoup and store in variable soup,take out the div tag of name and its value using find_all function .Here h4 has the car_name and span has the car_price.
  
**step5**: And this will take all the datas with help of BeautifulSoup and save it inthe tuple.

**step6**: Remove unwanted characters from the list of car_name using regex function replace and clean the data.

**step7**: Using pandas save the list of car_name and price as dataframe . But columns are not in good shape because we need all columns values in one columns.For that by using pandas 'ravel' combine all column values in one .

**step8**: create a dataframe vaues of car_name and car_price.Do some cleaning remove nullvalues to look clean. Save the dataframe as csv.file format
[Task_1.csv](https://github.com/sasikala07/Assessment_Scrapingtest/blob/main/Task1/task_1.csv)
