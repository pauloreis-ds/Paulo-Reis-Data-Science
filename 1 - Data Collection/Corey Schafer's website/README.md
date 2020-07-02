# Web Scraping with BeautifulSoup and Requests

      Practicing web scraping. There are 2 versions. The second one I did after I had watched the whole video.
      I encorage you to open both notebooks and analyze the methods in each one of them 
      (above the Agenda you'll see one exemple of the differences).

Video that helped me: https://www.youtube.com/watch?v=ng2o98k983k&list=WL&index=32&t=0s

Agenda
      Context
      1 - Getting the post title
      2 - Getting the post date
      3 - Getting the post description
      4 - Getting the post tags
      5 - Modeling?
      6 - Joining information in a DataFrame
      
 
#### First try: long and repetitive solution:

        # Titles
        page_title_records = soup.find_all('a', class_ = 'entry-title-link')
        titles = []
        for title in page_title_records:
            if title.contents[0] == 'Update (2019-09-03)':
                continue
            else:
                titles.append(title.contents[0])

        # Post dates
        page_post_dates = soup.find_all('time', class_ = 'entry-time')
        post_dates = []
        for post_date in page_post_dates:
            if  post_date.text == 'September 3, 2019':
                continue
            else:
                post_dates.append(post_date.text)

        # Descriptions
        post_descriptions = soup.find_all('div', class_='entry-content')
        descriptions = []
        not_wanted_description = 'blah blah blah'
        for description in post_descriptions:
            if description.p.text == not_wanted_description:
                continue
            else:
                descriptions.append(description.p.text)

        # Tags
        page_tags = soup.find_all('span',class_ = 'entry-tags')
        tags = []
        for tag in page_tags:
            tags.append(tag.text[13:-1])
            
           
#### Second try: shorter and smarter thought:

        articles = soup.find_all('article')

        # Lists to keep the scraped information
        titles = []
        dates = []
        descriptions = []
        tags = []

        # Putting the information into the lists
        for article in articles:
            try:
                titles.append(article.h2.a.text)
                dates.append(article.time.text)
                descriptions.append(article.div.p.text)
                tags.append(article.footer.text)
            except Exception as e:
                titles = None
                dates = None
                descriptions = None
                tags = None
