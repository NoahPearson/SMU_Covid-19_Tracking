# SMU Covid-19 Tracking
In the interest of visualization and analysis, I'm presenting the data reported by SMU: https://blog.smu.edu/coronavirus-covid-19/cases/

I start recording on move-in day, Aug. 17. Classes began a week later on Aug. 24.

### Data Last Updated: 10/4/2020 at 4:19 PM

The data presented are the reported cases on the day they're reported to SMU. We don't know when the test was taken by the student or when they reported to SMU. So, the significant uptick after classes began _actually_ was happening a few days earlier. **SMU also tends to under-report the most recent day (meaning they report some of the cases they received that day, later).** For that reason, I didn't compute the moving averages for the last day.

Hopefully, SMU will also make positivity/number of tests, isolation capacity, among other data publicly accessible. Edit: on 9/3, the linked site also includes a "dashboard" with active cases and isolation capacity. There are currently **30**(+2) people quarantining on-campus (asked to quarantine in their rooms because they were contact-traced) and we are at **10%** isolation space capacity; there are **15**(-3) people isolating (because they have the virus) on-campus. The remaining active on-campus cases must be isolating at home.

__9/27: No new cases reported__

## Raw Data:

__Total cumulative cases ("active" + "inactive"):__

![tot](https://github.com/NoahPearson/SMU_Covid-19_Tracking/blob/master/Plots/10:3_tot.png)

__New cases reported each day:__

With vertical lines marking the start of each week (Monday):

![new](https://github.com/NoahPearson/SMU_Covid-19_Tracking/blob/master/Plots/10:3_new.png)

__Weekly Average of Total New Cases Reported Each Day:__

![weekly](https://github.com/NoahPearson/SMU_Covid-19_Tracking/blob/master/Plots/10:3_weekly.png)

__3-Day moving average:__

![3day2](https://github.com/NoahPearson/SMU_Covid-19_Tracking/blob/master/Plots/10:3_mov3.png)

With this average, one can see this periodic pattern - a bump in reported cases in the middle of the week.

__7-Day moving average:__

![7day](https://github.com/NoahPearson/SMU_Covid-19_Tracking/blob/master/Plots/10:3_mov7.png)

__10-Day moving average:__

![10day](https://github.com/NoahPearson/SMU_Covid-19_Tracking/blob/master/Plots/10:3_mov10.png)

Comments:
As expected, off-campus and on-campus behavior is similar. The moving averages "smooth out" the extreme day-to-day variation in the new reported incidents. 

The sub-population that I'm most interested in is the on-campus students. They are related to our "limiting" factor - once we run out of isolation space at SMU, then we (according to the attached Fall Action Plan) will all be sent home to resume classes entirely online. It's difficult to tell how many active cases would exhaust the isolation pods, since at certain occupancy thresholds, students living within certain distances will be sent home to isolate. Additionally, it's entirely possible that more local students will isolate at their homes without SMU making them. The stated SMU isolation capacity is 127. "The University will provide 15 campus wellness pods, 44 bed spaces within Martin Hall, 16 bed spaces within Dyer House, and 52 beds within Perkins Hall as isolation quarters for students living on campus should they contract COVID-19."(Fall 2020 Operations Plan)

*I'm skeptical of the sudden decrease in reported cases. I think knowing more about the testing could shed some light.*

## Isolation:

![iso](https://github.com/NoahPearson/SMU_Covid-19_Tracking/blob/master/Plots/10:3_iso.png)

*Note: I forgot to record isolation capactity on 9/19, so I kept it at the previous known number.*

## Models/Projections:

__Stopped changing 9/18__

Naive exponential fit model for on-campus cumulative cases using Mathematica's nonlinear model function:

![model](https://github.com/NoahPearson/SMU_Covid-19_Tracking/blob/master/Plots/9:18_mod1.png)

![model again](https://github.com/NoahPearson/SMU_Covid-19_Tracking/blob/master/Plots/9:18_mod1.2.png)

**It's really difficult to model the spread (especially when I don't have that much knowledge about epidemiology). This model projects 500 on-campus (cumulative) cases in just over 7 days. This should NOT be taken as accurate. I made this model just to show how close/far the reported spread behavior is to an exponential (RSquared = 0.964).**

To add:
* active cases tracking
* growth factor
* models/projections
* "Go home" time scale estimate
* "turn-over point" analysis (when spread begins to decrease and level out)

Other Student Trackers:
* Jonathan Lindbloom: [GitHub](https://github.com/Jonathan-Lindbloom/SMU-COVID-19), [Tableau (Interactive)](https://public.tableau.com/profile/jonathan.lindbloom#!/vizhome/SMUCOVID-19InteractiveDashboard/Dashboard)
* Jared Burleson: [GitHub](https://github.com/jared-burleson/SMU_COVID_Case_Tracker)
