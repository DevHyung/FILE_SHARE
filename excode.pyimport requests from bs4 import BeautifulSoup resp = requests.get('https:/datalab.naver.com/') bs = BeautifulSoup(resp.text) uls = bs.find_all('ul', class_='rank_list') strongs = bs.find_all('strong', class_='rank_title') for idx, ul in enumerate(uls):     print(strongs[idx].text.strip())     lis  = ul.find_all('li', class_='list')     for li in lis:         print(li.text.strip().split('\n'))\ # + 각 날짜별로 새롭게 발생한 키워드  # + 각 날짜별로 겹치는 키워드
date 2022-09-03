import requests
from bs4 import BeautifulSoup
resp = requests.get('https://datalab.naver.com/')
bs = BeautifulSoup(resp.text)
uls = bs.find_all('ul', class_='rank_list')
strongs = bs.find_all('strong', class_='rank_title')
for idx, ul in enumerate(uls):
    print(strongs[idx].text.strip())
    lis  = ul.find_all('li', class_='list')
    for li in lis:
        print(li.text.strip().split('\n'))\
# + 각 날짜별로 새롭게 발생한 키워드 
# + 각 날짜별로 겹치는 키워드 
