# Web Dev - Troubleshooting

#4Site #procedure #troubleshoot

Summary of the issue that came up: AIUSA Multistep lightbox a/b test running, srtart

<u>https://raw.githubusercontent.com/4site-interactive-studios/aiusa-promotions-eoy-2023-raw-code/main/raw-code.js</u>

What I checked and saw
* 		As far as I can tell the random function is working as it should. The 50/50 split look good when reporting on pageviews via GA4
* 		Test (results in console): 
* [https://codepen.io/4SiteStudios/pen/Vwgpxvw?editors=1111](https://codepen.io/4SiteStudios/pen/Vwgpxvw?editors=1111)		Some of the variable names, and a code comment were confusing
* 		
* [https://github.com/4site-interactive-studios/aiusa-promotions-eoy-2023-raw-code/commit/b297a89e3d853430df2c2f494f2443554108efa6](https://github.com/4site-interactive-studios/aiusa-promotions-eoy-2023-raw-code/commit/b297a89e3d853430df2c2f494f2443554108efa6)		One of the function names was ambigious
* 		
* [https://github.com/4site-interactive-studios/aiusa-promotions-eoy-2023-raw-code/commit/e009222900d1fee739facb2201b20ea4a75ae1dd](https://github.com/4site-interactive-studios/aiusa-promotions-eoy-2023-raw-code/commit/e009222900d1fee739facb2201b20ea4a75ae1dd)		One of the multistep lightbox tests was missing it’s associated data layer event (updated on the code repo)
* 		
* [https://github.com/4site-interactive-studios/aiusa-promotions-eoy-2023-raw-code/commit/2ae5a28279912f43aac70be7bc312e9e31ea5777](https://github.com/4site-interactive-studios/aiusa-promotions-eoy-2023-raw-code/commit/2ae5a28279912f43aac70be7bc312e9e31ea5777)