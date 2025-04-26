# Google Jobs Scraper v2

### About the project

This is a fork of the original [Google Jobs Scraper](https://github.com/alimahmoud7/google-jobs-scraper) project. I plan to maintain and update it as needed to ensure continued functionality and address any potential issues with outdated dependencies.

> Simply, The script scrapes all the jobs from all the pages (first to final available page) located on [https://careers.google.com/jobs](https://careers.google.com/jobs#t=sq&li=20&st=0&jlo=all) and return's the result as a JSON string, Then you will have a JSON file containing  all scraped data.

### How to Run the Program

1. Download and Install [Python 3](https://www.python.org/)
2. Install requirements
```
pip install requests beautifulsoup4 selenium
```
3. Download the latest release of [Chrome Driver](https://sites.google.com/a/chromium.org/chromedriver/downloads) for your OS
4. Extract chromedriver and move it to the same directory of `scrape_google.py` file
5. Finally, Run `scrape_google.py`
```
python scrape_google.py
```

### Structure of JSON output 
```
{
  "total": "total_count",
  "jobs": [
    {
      "job_id": "id1",
      "title": "title1",
      "location": "location1", 
      "intro": "introduction1", 
      "resps": "responsibilities1",
      "quals": "qualifications1"
    },
    {
      "job_id": "id2",
      "title": "title2",
      "location": "location2", 
      "intro": "introduction2", 
      "resps": "responsibilities2",
      "quals": "qualifications2"
    },
    ...
  ]
}
```

### Contributing
If you’d like to contribute to the project, please fork this repository, make your changes, and submit a pull request. Feel free to report issues or suggest improvements.
