# Data Commons
TO DO: Move the 21 goals under a parent sidenav called "Goal Visualization". 
Duplicate these 3 as parent sidenav: Energy, Healthy Food, Innovation. 
Duplicate 18-21 under Innovation.
Avoid showing deeper levels like food/balance in the left navigation.

View the [Config Doc](https://observablehq.com/framework/config) for a solution. The Config Doc has cascading navigation itself.
For coding tips, describe to [chat.openai.com](https://chat.openai.com).
<br><br>

## Goal Visualization

The [UN's seventeen 30-year goals](/data-pipeline/international/), plus four subsets of goal 9: Innovation.

1. [Good Paying Jobs](jobs)
2. [Healthy Food](food)
3. [Good Health](health)
4. [Quality Education](education)
5. [Women's Rights](women)
6. [Clean Water](water)
7. [Energy](energy)
8. [Healthy Economies](economies)
9. [Innovation](innovation)
10. [Opportunities](opportunities)
11. [Biodiversity](biodiversity)
12. [Conservation](conservation)
13. [Net Positive](net)
14. [Aquatic](nemo)
15. [Wildlife](wildlife)
16. [Peace and Justice](peace)
17. [Partnerships to Achieve Goals](partnerships)
18. [Balanced Budgets](balanced)
19. [Fast Reliable Transit](transit)
20. [High Speed Internet](internet)
21. [Expanding Livable Zones](space)

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