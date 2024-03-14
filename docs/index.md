# Data Commons

## Goal Visualization

The [UN's seventeen 30-year goals](/data-pipeline/international/), plus four subsets of goal 9: Innovation.

1. [Good Paying Jobs](jobs)
2. [Healthy Food](food)
3. [Good Health](health)
4. [Quality Education](education)
5. [Gender Equality](women)
6. [Clean Water](water)
7. [Energy](energy)
8. [Healthy Economies](economy)
9. [Innovation](innovation)
10. [Opportunities](opportunities)
11. [Biodiversity](biodiversity)
12. [Conservation](conservation)
13. [Air and Climate](net)
14. [Aquatic](aquatic)
15. [Wildlife](wildlife)
16. [Peace and Justice](peace)
17. [Partnerships](partners)
18. [Balanced Budgets](balanced)
19. [Fast Reliable Transit](transit)
20. [High Speed Internet](internet)
21. [Expanding Livable Zones](space)

<br>

TO DO: View the [Config Doc](https://observablehq.com/framework/config) and figure out how it's cascading navigation is set up. Display the 21 goals as subtopics under a parent called "Goal Visualization".  (Avoid changing the existing folder paths for this nav setup.

Display 4 side navigation parent topics:  
Goal Visualization, Local Innovation, Energy, Healthy Food  
List goals 17-21 under the Local Innovation side navigation.  
Avoid showing goal sublevels (example: food/balance) in the left navigation.
<br>

<style>
table {
    display: block;
    width: 100%;
    width: max-content;
    max-width: 100%;
    overflow: auto;
    border: 1px solid #ccc;
}
table th {
	text-align: left;
	font-size: 16px;
	padding: 6px;
	border-bottom: 1px solid #ccc;
}
table td {
	padding: 6px;
}
</style>

## Commands

You'll use `yarn build` the most.  
`yarn dev` invokes https which requires installing a cert locally. (Ugh)

Instead, after you've run `python -m http.server 8887` in your webroot, view at:

[http://localhost:8887/data-commons/docs](http://localhost:8887/data-commons/docs/)  
[http://localhost:8887/data-commons/dist](http://localhost:8887/data-commons/dist/)


| Command           | Description                                              |
| ----------------- | -------------------------------------------------------- |
| `yarn install`    | Install or reinstall dependencies                        |
| `yarn dev`        | Start local preview server                             |
| `yarn build`      | Build your static site, generating `./dist`              |
| `yarn deploy`     | Deploy your project to Observable                        |
| `yarn clean`      | Clear the local data loader cache                        |
| `yarn observable` | Run commands like `observable help`                      |


## Google Data Commons

[Statistical Variable Explorer](https://datacommons.org/tools/statvar) - Filter by date and location on more than 10,000 statistical variables to find data for the 21 goals.

We can add a wrapper of the Statistical Variable Explorer.

[The Python Data Loaders](https://docs.datacommons.org/tutorials/) are simpler than the JS ones. In Python, you do not need to handle the crazy API call templates. Finding DCID and property is just one problem in JS, another problem is handling different JSON structures, which is not an issue in Python, as can be seen in this example -
https://colab.research.google.com/github/datacommonsorg/api-python/blob/master/notebooks/analyzing_census_data.ipynb
