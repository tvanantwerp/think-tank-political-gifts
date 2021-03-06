# Politcal Contributions from Think Tank Employees During the 2012 Election Year

These data include political contributions from employees of the [top ten U.S. think tanks](http://gotothinktank.com/dev1/wp-content/uploads/2014/01/GoToReport2013.pdf) during the 2012 election year. They were [scraped](https://github.com/tvanantwerp/opensecrets-scraper) from [OpenSecrets.org](https://www.opensecrets.org/). These data have been manually cleaned to consolidate duplicate persons and eliminate persons who were not actually think tank employees.

These data were compiled for a blog post examining the [political bias of think tank employees as revealed through their political contribution decisions](http://tomvanantwerp.com/think-tank-partisanship). They were scraped from OpenSecrets.org using a python script available [here](https://github.com/tvanantwerp/opensecrets-scraper).

## Explanation of Data

### `donations-top-ten-think-tanks-2012.csv`

| Variable | Explanation |
| --- | --- |
| id | Integer assigned to each unique individual indentified in the raw data. |
| First Name | First name scraped for each individual contribution. May vary between multiple entries for a single individual. |
| Last Name | Last name scraped for each individual contribution. May vary between multiple entries for a single individual. |
| City | City given as place of residence at time of reporting. |
| State | State given as place of residence at time of reporting. |
| Zip | Zip code given as place of residence at time of reporting. |
| Think Tank | The name of the think tank employer of the individual. These names have been manually edited to enforce uniformity. |
| Date | Date of the contribution. |
| Amount | Amount of the contribution. |
| Recipient | The politician or partisan group receiving the reported contribution. |
| Partisan Recipient | The know partisanship of the recipient. D is Democratic, R is Republican, L is Libertarian, and Other is other or unknown. |

### `990s-top-ten-think-tanks-2012.csv`

| Variable | Explanation |
| --- | --- |
| Think Tank | The name of the think tank. |
| Employees | The number of employees reported on the 2012 form 990 filed with the IRS. |
| Revenue | The revenuses reported on the 2012 form 990 filed with the IRS. |
| Expenses | The expenses reported on the 2012 form 990 filed with the IRS. |
| Net Income | The net income reported on the 2012 form 990 filed with the IRS. |
| Net Assets | The net assets reported on the 2012 form 990 filed with the IRS. |

### `think-tank-donation-summary.json`

| Variable | Explanation |
| --- | --- |
| `name` | The name of the think tank. |
| `employees` | The number of employees reported on the 2012 form 990 filed with the IRS. |
| `etod` | The sum of employees for a given think tank who gave to Democrats or Democratic groups. |
| `etor` | The sum of employees for a given think tank who gave to Republicans or Republican groups. |
| `etol` | The sum of employees for a given think tank who gave to Libertarians or Libertarian groups. |
| `etoo` | The sum of employees for a given think tank who gave to other or unknown groups. |
| `ctod` | The sum of cash contributions for a given think tank's employees which went to Democrats or Democratic groups. |
| `ctor` | The sum of cash contributions for a given think tank's employees which went to Republicans or Republican groups. |
| `ctol` | The sum of cash contributions for a given think tank's employees which went to Libertarians or Libertarian groups. |
| `ctoo` | The sum of cash contributions for a given think tank's employees which went to other or unknown groups. |