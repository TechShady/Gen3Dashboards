# User Experience Overview Dashboard
This dashboard provides an executive level overview on KPIs and Customer Experience.

![Executive Overview Dashboard](ExecutiveOverview.png)

# Prerequisites

Required: [Create a conversion goal](https://www.dynatrace.com/support/help/platform-modules/digital-experience/web-applications/analyze-and-use/define-conversion-goals) for a user action that indicates the start of a business transaction (i.e. Login Page).

Required: [Create a conversion goal](https://www.dynatrace.com/support/help/platform-modules/digital-experience/web-applications/analyze-and-use/define-conversion-goals) for a user action that indicates a completed business transaction (i.e. Order Confirmation Page).

# Target Audience

- Application Owner
- Line of Business
- Executive

# Use Cases

- Are performance issues impacting my customer experience?
- Are errors impacting my customer experience?
- Are performance and error trends impacting my customer experience?
- Are my KPIs trending in the right direction?
- What days/times do I have good customer experience?
- Are my users converting efficiently? 
- Does a change in my APDEX score impact my customer experience?
- Are my users staying engaged?
- Do I have user satisfaction problems/trends?
- Is my traffic trending in the right direction?
- Is my bounce rate normal and trending in the right direction?

# Install Instructions

- Download [Dashboard JSON](https://github.com/TechShady/Gen3Dashboards/blob/main/User%20Experience%20Overview.json)
- Launch the new Gen3 UI
- Select the Dashboard app
- In the upper righthand corner, select Upload and select your json file
- Refresh your dashboard list and launch your Dashboard

# User Guide

The User Experience Overview Dashboard is broken down into four sections.

![Executive Overview Dashboard](ExecutiveOverview-0.png)

The dashboard header section has four filters that you can apply to your Executive Overview Dashboard:
- AppName - List of applications currently monitored by Dynatrace that have conversion goals defined. Select the application to filter the dashboard for any application. 
- MilestoneGoal - List of conversion goals. Select the conversion goal that indicates the start of a business transaction.
- ConversionGoal - List of conversion goals. Select the conversion goal that indicates the completion of a business transaction.
- TimeShift - Value in days used by metrics to compare against. For example, a value of 7 will compare the KPI based on the current timeframe and compare that value to the same timeframe shifted by 7 days.

![Executive Overview Dashboard](ExecutiveOverview-1.png)

The top section is called the KPI banner. This section has the following KPIs:

- Application Health: Application Health will be Green if the 6 indicators to the right are all Green. If any indicator is Red, Application Health will be Red. Otherwise Application Health is Yellow.
- Avg Duration: Time between the initial user input and complete page load. Avg Duration > 6s = Red. Avg Duration > 3s and < 6s = Yellow. Avg Duration < 3s = Green.
- Avg Errors: Average number of Request and JavaScript Errors.  Avg Errors > 2 = Red. Avg Errors > 0 = Yellow. Avg Errors = 0 = Green.
- Efficiency Rate: Rate of sessions that converted with good user experience. Rate < 50% = Red. Rate < 75% and > 50% = Yellow. Rate > 75% = Green.
- Deficiency Rate: Rate of sessions that abandoned with poor user experience. Rate > 50% = Red. Rate > 25% and < 50% = Yellow. Rate < 25% = Green.
- Conversion Rate: Rate of sessions that converted. Rate < 40% = Red. Rate < 60% and > 40% = Yellow. Rate > 60% = Green.
- Apdex: Application Performance Index is a standard developed by an alliance of companies for measuring the performance of applications. A perfect Apdex score is 1. Apdex < .8 = Red. Apdex >.8 and < .92 is Yellow. Rate > .92 is Green.

![Executive Overview Dashboard](ExecutiveOverview-2.png)

The middle section KPI metrics (with comparison to a seven-day time shift) for: 
- Sessions - Total number of user sessions.
- New Sessions - Total number of new user sessions.
- Avg Duration: Time between the initial user input and complete page load.
- Avg Errors: Average number of Request and JavaScript Errors.
- Requests - Total number of user actions.
- Bounces - Total number of user sessions that bounced from the web site.
- Efficiency Rate: Rate of sessions that converted with good user experience. A perfect efficiency rate is 100.
- Deficiency Rate: Rate of sessions that abandoned with poor user experience. A perfect deficiency rate is 0.
- Conversion Rate: Rate of sessions that converted.
- Avg Clicks To Convert: The average number of user actions executed within a user session that converted.
- Apdex: Application Performance Index is a standard developed by an alliance of companies for measuring the performance of applications. A perfect Apdex score is 1.
- Avg Time On Site - Average session duration.

Each KPI cell displays the current value based on the selected timeframe. Each KPI is compared to a time shift that is selected in the TimeShift variable dropdown and will display, in parentheses, the KPI difference and trend direction.

![Executive Overview Dashboard](ExecutiveOverview-3.png)

The bottom section charts customer satisfaction over the selected timeframe.
