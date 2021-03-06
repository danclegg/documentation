## Widget Creation

Widgets - contain special graphical control elements that were designed to provide a simple and 
easy-to-use way of displaying and analyzing your automation trends and data.

The widgets can be added to dashboards on the "Dashboards" tab. Widgets will be visible within the project, they are created.

### Create widget

To create a new widget, perform the following steps:

1. Navigate to the "All Dashboards" page and create a new dashboard or choose the existing one.

2. Click "Add New Widget" button.

3. The Widget Wizard will be opened. In order to  add a new widget, you need to pass all required steps.

    • Step 1. Select the template of widget (detailed description is below).

    • Step 2. Select filter from the list below or create a new filter. Search functionality helps to find the filter 
      quicker. Select other widget options: Criteria, Items, Launch or Timeline mode (if applicable for selected widget template)

    • Step 3. Enter a widget name, description and share a widget (if need). 
      A widget name should be unique for a user on the project.

4. After you have completed all steps, click the "Save" button. The new widget will be added to the dashboard on the top.

Widgets are automatically refreshed every minute.

[ ![Image](Images/userGuide/widgets/createWidget.png) ](https://youtu.be/uRY_ihUe_oU)

### Predefined widgets types

There are 15 widget templates in ReportPortal for tracking different KPI:

| KPI  | Widget template |
| ------------- | ------------- |
|   | [Launch statistics chart](https://reportportal.io/docs/Launch-statistics-chart)  |
|  Passing rate for filter summary, and structure of problems |[Overall statistics](https://reportportal.io/docs/Overall-statistics)  |
|  Track the longest launch in the filter  | [Launches duration chart](https://reportportal.io/docs/Launches-duration-chart) |
|   Track the passing rate and structure of problems of the latest run in the system| [Launch execution and issue statistic](https://reportportal.io/docs/Launch-execution-and) |
|  Track the activity of your QA team | [Project activity panel](https://reportportal.io/docs/Project-activity-panel)  |
| Track the growth of new test cases in your build  | [Test-cases growth trend chart](https://reportportal.io/docs/Test-cases-growth-trend) |
| Track the speed of test failure analysis | [Investigated percentage of launches](https://reportportal.io/docs/Investigated-percentage-of)  |
| Follow up information about only important launches for your team  | [Launches table](https://reportportal.io/docs/Launches-table) |
| Track new BTS issues in your run  | [Unique bugs table](https://reportportal.io/docs/Unique-bugs-table) |
|  Track the most unstaoble test cases in the build | [Most failed test-cases table](https://reportportal.io/docs/Most-failed-test-cases) |
|  See the trend of number of failed test cases from build to build | [Failed cases trend chart](https://reportportal.io/docs/Failed-cases-trend) |
|  See the trend of number of failed and skipped test cases from build to build | [Non-passed test-cases trend chart](https://reportportal.io/docs/Non-passed-test-cases-trend)  |
| Compare two launches together  | [Different launches comparison chart](https://reportportal.io/docs/Different-launches-comparison) |
|  Track passing rate for one launch | [Passing rate per launch](https://reportportal.io/docs/Passing-rate-per)  |
| Track passing reate for the build  | [Passing rate summary](https://reportportal.io/docs/Passing-rate-summary) |
|  Find the most flaky test in the build | [Flaky test cases table (TOP-20)](https://reportportal.io/docs/Flaky-test-cases)  |
| Compare statistics for different builds on one graph  | [Cumulative trend chart](https://reportportal.io/docs/Cumulative-trend-chart) |
| Track the most popular failure reasons in the build  | [Most popular pattern table (TOP-20)](https://reportportal.io/docs/Most-popular-pattern)  |
| Track the passing rate of different components of your application  | [Component health check](https://reportportal.io/docs/Component-health-check) |


The template descriptions are provided below.


## Launch statistics chart

The widget can be used in two modes - Launch mode and Timeline mode:

- The widget in Launch mode shows the growth trend in the number of test cases with each selected status from run to run,
- The widget in Timeline mode shows the sum of test cases with each selected status distributed by dates.

Also you can choose different view of this widget:  Area view or Bar view.
For a deeper investigation you can use Zoom widget area functionality.

**Widget's parameters:**

- Filter: At least one filter is required
- Items: 1-150. Default meaning is 50.
- Widget Criteria: All criteria is selected by default.
- Mode: Launch or Timeline.
- View: Area/ Bar
- Widget Criteria: All criteria is selected by default.

>**Note:**
If you choose **“Total Defect type”**, the system will show the grouped statistics of a chosen standard defect type (the summary of all custom types).  
If you check a single custom defect types, the system will show just the defect type that you have chosen.
If you choose “Total Defect type” and custom defect types, the system will show and  a grouped statistics and statistic of each custom defect types.

[ ![Image](Images/userGuide/widgetTypes/launchStatisticsChart1.png) ](Images/userGuide/widgetTypes/launchStatisticsChart1.png)


**Widget view**

The widget contains agenda with selected statuses; you can click on a status to remove/add it to the chart.

The widget view in Launch mode:

- X-axis shows launches numbers and launches names (on hover).
- Y-axis shows sum of test cases with each selected statuses.

The tooltip on mouse hover over chart area shows launch details: launch name and number, launch start time and launch statistics.

Area view
[ ![Image](Images/userGuide/widgetTypes/launchStatisticsChartArea.png) ](Images/userGuide/widgetTypes/ Images/userGuide/widgetTypes/launchStatisticsChartArea.png)

Bar view
[ ![Image](Images/userGuide/widgetTypes/launchStatisticsChartBar.png) ](Images/userGuide/widgetTypes/ Images/userGuide/widgetTypes/launchStatisticsChartBar.png)

The widget view in Timeline mode:

- X-axis shows dates and weekdays.
- Y-axis shows sum of launches statistics with each selected statuses, distributed by weekdays.

The tooltip on mouse hover over the chart area shows details: date and total launches statistics. 

The widget has clickable sections; when you click on a specified section in widget, the system forwards you to launch view for appropriate selection.

Area view
[ ![Image](Images/userGuide/widgetTypes/launchStatisticsChartArea1.png) ](Images/userGuide/widgetTypes/ Images/userGuide/widgetTypes/launchStatisticsChartArea1.png)

Bar view
[ ![Image](Images/userGuide/widgetTypes/launchStatisticsChartBar1.png) ](Images/userGuide/widgetTypes/ Images/userGuide/widgetTypes/launchStatisticsChartBar1.png)

>**Note:**
The widget doesn't contain "IN PROGRESS" launches.

## Overall statistics

The panel shows a summary of test cases with each status for each selected launch.

**Widget's parameters:**

- Filter: At least one filter is required
- Items: 1-150. Default meaning is 50.
- Widget Criteria: All criteria is selected by default.
- Type of view: Panel view/ Donut view
- Mode All launches/ Latest launches


**Widget view**

The widget shows statistics of the All launches/or Latest launches for the chosen filter. Statistics are divided into the following sections:
-	Skipped, Passed, Failed
-	Product Bug, System Issue, Automation Bug, No Defect and To Investigate.

The statistics for every type are shown in percentage. On hover the exact number is shown for each type.
The Widget has clickable sections, when you click on specified section in widget, the system forwards you to launch view for appropriate selection.

If you chose *All launches* mode, the widget will show the statistics about all launches in the filter. To view only latest executions of each launch, you should choose *Latest launches*.

The widget can be viewed in two options as shown on pictures: Panel view 

[ ![Image](Images/userGuide/widgetTypes/PanelView.png) ](Images/userGuide/widgetTypes/PanelView.png)

or Donut view. 

[ ![Image](Images/userGuide/widgetTypes/DonutView.png) ](Images/userGuide/widgetTypes/DonutView.png)

>**Note:**
The widget doesn't contain "IN PROGRESS" launches.
 

##  Launches duration chart

The Launch Duration Chart shows the duration of the selected launches.

**Widget's parameters:**

- Filter: At least one filter is required
- Items: 1-150. Default meaning is 50
- Mode All launches/ Latest launches

**Widget view**

The widget shows the duration of the filtered launches.

- X-axis shows launches duration.
- Y-axis shows launches numbers and launches names on hover.

Tooltip on mouse hover over chart area shows launch details: launch name, number and duration. 

The Widget has clickable sections, when you click on specified section in widget, the system forwards you to launch view for appropriate selection.

The Widget has two states: All launches and Latest lunches. If you chose *All launches* mode, widget will show statistic about all launches in the filter. To view only latest executions of each launch, you should choose *Latest launches*.

[ ![Image](Images/userGuide/widgetTypes/launchesDurationChart.png) ](Images/userGuide/widgetTypes/launchesDurationChart.png)
 
>**Note:**
The widget doesn't contain "IN PROGRESS" launches.


## Launch execution and issue statistic

The Launch Execution and Issue Statistic chart shows the status and issues statistics for last launch of a specified range.

**Widget's parameters:**

- Filter: required

**Widget view**

The widget shows statistics of the last finished launch for the chosen filter. The statistics are divided into the following sections:

- Skipped, Passed, Failed
- Product Bug, System Issue, Automation Bug, No Defect (default and custom) and To Investigate.

The widget contains agenda with statuses, the user can click on a status to remove/add it to the chart.

Tooltip on mouse hover over chart area shows launch details: launch name, number and duration. 

The statistics for every type is shown in percentage. On hover the exact number is shown for each type.

The widget has clickable sections, when you click on a specified section in the widget, the system forwards you to the launch view for the appropriate selection.

[ ![Image](Images/userGuide/widgetTypes/launchExecutionAndIssueStatistic.png) ](Images/userGuide/widgetTypes/launchExecutionAndIssueStatistic.png)


## Project activity panel

The widget shows all activities occurring on the project.

**Widget's parameters:**

- The actions for widget are as follows: Update Project Settings, Update Defect Types, Delete Launch, Start Launch, Finish Launch, Share Widget, Dashboard, Unshare Widget, Dashboard, Post Issue to BTS, Add, Register User, Update BTS. By default all actions are checked.

- Items: 1-150. Default meaning is 50.

- Type user name: By default all user's activities. 

**Widget view**

The actions on the widget are present in a table, separated by days. Action messages have the following format:

>   *Member (name) did action.*  
>   *Time - displayed in 'time ago' format (i.e. "10 minutes ago"). On mouse hover, the system should display accurate action time.)*

[ ![Image](Images/userGuide/widgetTypes/projectActivityPanel.png) ](Images/userGuide/widgetTypes/projectActivityPanel.png)


## Test-cases growth trend chart

The widget can be used in two modes - Launch mode and Timeline mode:

- The widget in the Launch mode shows the increment of test-cases from run to run,
- The widget in the Timeline mode shows the increment of test-cases distributed by dates (in launches with the largest number of test-cases per day).

**Widget's parameters:**

- Filter: At least one filter is required
- Items: 1-150. Default meaning is 50.
- Mode: Launch or Timeline.

**Widget view**

The widget view in Launch mode:

- X-axis shows launches numbers and launches names on hover.
- Y-axis shows the increment of test-cases.

The tooltip on mouse hover over the chart area shows launch details: launch name and number, launch start time and launch statistics - total number of test cases and test cases growth.

[ ![Image](Images/userGuide/widgetTypes/testCasesGrowthTrendChart.png) ](Images/userGuide/widgetTypes/testCasesGrowthTrendChart.png)

The widget view in Timeline mode:

- X-axis shows dates and weekdays.
- Y-axis shows the increment of test-cases in launches with the largest number of test-cases per day.

The tooltip on mouse hover over the chart area shows launch details: date and launch statistics - total number of test cases and test cases growth.

The widget has clickable sections, when you click on a specific section in the widget, the system forwards you to the launch view for the appropriate selection.

[ ![Image](Images/userGuide/widgetTypes/testCasesGrowthTrendChartTimeline.png) ](Images/userGuide/widgetTypes/testCasesGrowthTrendChartTimeline.png)

>**Note:**
The widget doesn't contain "IN PROGRESS" launches.


## Investigated percentage of launches

The widget can be used in two modes - Launch mode and Timeline mode:

- The widget in the Launch mode shows the percentage of "Investigated" and "To Investigate" items by launch to sum (Product Bugs + Auto Bugs + System Issues + To Investigates).
- The widget in the Timeline mode shows the percentage of "Investigated" and "To Investigate" items to sum (Product Bugs + Auto Bugs + System Issues + To Investigates) in all runs per day, distributed by dates.

**Widget's parameters:**

- Filter: At least one filter is required.
- Items: 1-150. Default meaning is 50.
- Mode: Launch or Timeline. Default meaning is Launch mode.

**Widget view**

The widget contains agenda with "To Investigate" and "Investigated" labels.

The widget view in Launch mode:

- X-axis shows launches numbers and launches names on hover.
- Y-axis shows percent of "Investigated" and "To Investigate" items to sum. (Product Bugs + Auto Bugs + System Issues + To Investigates)

The tooltip on mouse hover over the chart area shows launch details: launch name, number, launch start time and "percentage of "Investigated" or "To Investigate" items.

[ ![Image](Images/userGuide/widgetTypes/investigatedPercentageOfLaunches.png) ](Images/userGuide/widgetTypes/investigatedPercentageOfLaunches.png)

The widget view in Timeline mode:

- X-axis shows dates and weekdays.
- Y-axis shows a percent of "Investigated" and "To Investigate" items to sum (Product Bugs + Auto Bugs + System Issues + No Defects + To Investigates) distributed by dates.

The tooltip on mouse hover over the chart area shows launch details: date and percentage of "Investigated" or "To Investigate" items.

The widget has clickable sections, when you click on a specific section in the widget, the system forwards you to the launch view for the appropriate selection.

[ ![Image](Images/userGuide/widgetTypes/investigatedPercentageOfLaunchesTimeline.png) ](Images/userGuide/widgetTypes/investigatedPercentageOfLaunchesTimeline.png)

>**Note:**
The widget doesn't contain "IN PROGRESS" launches.


## Launches table

The widget shows a configurable table of launches.

**Widget's parameters:**

 - The widget criteria is as follows: Total, Passed, Failed, Skipped, Product Bug, Automation Bug, System Issue, To Investigate, Tags, User, Description, Start time, Finish time. All criteria is selected by default. To specify them, uncheck unnecessary items in "Criteria for Widget".
 - Items: 1-150. Default meaning is 50.

**Widget view**

The widget has a table view.

The widget has clickable elements "launch name", "owner", "tags", and "number of items"; when you click on specific elements in the widget, the system forwards you to the launch view for the appropriate selection.

[ ![Image](Images/userGuide/widgetTypes/launchesTable.png) ](Images/userGuide/widgetTypes/launchesTable.png)

>**Note:**
The widget doesn't contain "IN PROGRESS" launches.


## Unique bugs table

The widget shows real identified bugs, posted to the Bug Tracking System from ReportPortal, and existing bugs, that were added to the items on ReportPortal.

**Widget's parameters:**

  - Filter: At least one filter is required
  - Items: 1-150. Default meaning is 10.

**Widget view**

The widget has a table view and bugs that are found are then sorted by the date they were posted or added.

The widget has the following data displayed:

- Bug ID  -  links to the issue in Bug Tracking System.
- Found in - links to the test item, to which the bug was posted/added.
- Submit date  - date the bug was submitted/added. Time is displayed in 'time ago' format (i.e. "10 minutes ago"). On mouse hover the system should display accurate action time.
- Submitter  - user, who submitted/added the bug.

[ ![Image](Images/userGuide/widgetTypes/uniqueBugsTable.png) ](Images/userGuide/widgetTypes/uniqueBugsTable.png)

>**Note:**
The bugs from launches "IN PROGRESS" are not shown on the widget.
In case a bug is found in multiple items, all of items will be listed in "Found in" column.


## Most failed test-cases table (TOP-20)

The widget contains a table with statistical information about the TOP-20 most problematic test cases.

**Widget's parameters:**

 - The widget criteria is as follows: Failed, Skipped, Product Bug, Automation Bug, System Issue, No Defect. Failed is selected by default.

 - Launches count: 2-150. By default, "Launches count" is 30.

 - Launch name: Is required.
 
 - Include /Exclude  Before and After methods

**Widget view**

The widget has a table view with the following data displayed:

- Test Item name - link to the Step level of the last launch
- Failed - count of found failed results
- Last failure - date and time of last run, when the test item was failed, displayed in 'time ago' format (i.e. "10 minutes ago").
On mouse hover the system will display accurate start times.

[ ![Image](Images/userGuide/widgetTypes/mostFailureTestCasesTable.png) ](Images/userGuide/widgetTypes/mostFailureTestCasesTable.png)

>**Note:**
The widget contains statistics of the most problematic tests cases in all launches, except "IN PROGRESS" and "INTERRUPTED" launches.


## Failed cases trend chart

The widget shows the trend of growth in the number of failed test cases (Product Bugs + Auto Bugs + System Issues + No Defects + To Investigates) from run to run.

**Widget's parameters:**

 - Filter.
 - Items: 1-150. Default meaning is 50.

**Widget view**

The widget contains agenda: "Failed".

- X-axis shows launches numbers and launches names on hover.
- Y-axis shows number of Failed issues (sum of Product Bugs + Auto Bugs + System Issues + No Defects + To Investigates).

The tooltip on mouse hover over the chart area shows launch details: launch name and number, launch start time and number of failed test cases.

[ ![Image](Images/userGuide/widgetTypes/failedCasesTrendChart.png) ](Images/userGuide/widgetTypes/failedCasesTrendChart.png)

>**Note:**
The widget doesn't contain "IN PROGRESS" launches.


## Non-passed test-cases trend chart

The widget shows the percent ratio of non-passed test cases "Failed + Skipped" and "Total" cases from run to run.

**Widget's parameters:**

To configure the widget, click "Add New Widget" button on the dashboard header, then select a template and specify the following settings on the second step:

- Filter.
- Items: 1-150. Default meaning is 50
 
**Widget view**

The widget contains agenda: % (Failed + Skipped) / Total.

- X-axis shows launches numbers and launches names on hover.
- Y-axis shows percent of sum Failed + Skipped test cases to Total.

The tooltip on mouse hover over the chart area shows launch details: launch name and number, launch start time and percentage of non-passed cases.

[ ![Image](Images/userGuide/widgetTypes/nonPassedTestCasesTrendChart.png) ](Images/userGuide/widgetTypes/nonPassedTestCasesTrendChart.png)

>**Note:**
The widget doesn't contain "IN PROGRESS" launches.


## Different launches comparison chart

The widget allows you to compare statistics for the 2 last launches side by side.

**Widget's parameters:**

- Filter.

**Widget view**

- X-axis shows launches numbers and launches names on hover.
- Y-axis shows percentage of test-cases by statuses.

The widget contains agenda with statuses, the user can click on a status to remove/add it to the chart.

The tooltip on mouse hover over the chart area shows launch details: launch name and number, launch start times and percentage of test cases of a particular type.

The widget has clickable sections, when you click on specific sections in widget, the system forwards you to the launch view for the appropriate selection.

[ ![Image](Images/userGuide/widgetTypes/differentLaunchesComparisonChart.png) ](Images/userGuide/widgetTypes/differentLaunchesComparisonChart.png)

>**Note:**
The widget doesn't contain 'IN PROGRESS" launches.

## Passing rate per launch


**Widget's parameters:**



**Widget view**



>**Note:**
The widget doesn't contain 'IN PROGRESS" launches.


## Passing rate summary

**Widget's parameters:**



**Widget view**



>**Note:**
The widget doesn't contain 'IN PROGRESS" launches.

## Flaky test cases table (TOP-20)
Shows the TOP-20 the most flaky test cases within the specified previous launches. The widget defines test cases with the most high percentage of switching their status in the execution. So that you can click on the test cases and be redirected to the last test item in execution to check the reasons. 

**Widget's parameters:**

- Launches count: 2-150. Default meaning is 30.

- Launch name. Is required

- Include /Exclude  Before and After methods

**Widget view**

The widget has a table view with the following data displayed:

- Test Item name - link to the Step level of the last launch

- Switches - count of found results with often switches;

- % of Switches - the per cent of the fact switches and the possible;

- Last switch - date and time of a last run, when the test item switches the status, displayed in 'time ago' format (i.e. "10 minutes ago").

On mouse hover the system will display accurate start times.

[ ![Image](Images/userGuide/widgetTypes/flakyTestCasesTableWidget.png) ]( Images/userGuide/widgetTypes/flakyTestCasesTableWidget.png)

## Cumulative trend chart

Shows the growth trend of summary statistics of launches with the same attribute key. 
You can see a growth of statistics from the build to the build, or from version to version. 
A widget does not require an edit or new filter creation. If new version (build, release or other) is added to ReportPortal, new information will be added to the graph.

[ ![Cumulative Video](Images/userGuide/widgetTypes/CumulativeFirstLevelView.png) ](https://youtu.be/F51a1JpEITo)


**Widget's parameters:**
- Filter
- Parameters: only Latest launches
- Number of shown attrinutes on the widget: 1 - 15
- Attribute key for the first level (mandatory)
- Attribute key for the second level (optional)

[ ![ImageName](Images/userGuide/widgetTypes/CumulativeCreation.png) ](Images/userGuide/widgetTypes/CumulativeCreation.png)

**Widget view**
A widget have two levels.

**For the first level**  the system uses the last 600 launches from the chosen filter. 
Then  system searches all launches which have attributes with the key specified on the widget wizard for the first widget level (for example attribute key - BUILD).
Then system combines launches into groups around unique attribute value (BUILD:3.6, BUILD:V3.7, BUILD:3.8…..).
After that the system should keep in each group **only latest executions** (e.g.  the latest launches for BUILD:3.6,  the latest launches  BUILD:V3.7,  the latest launches  BUILD:3.8…. ) and reflects statistics for all unique attributes on the graph for the first widget level.

First level view - summ statistics of launches with attributes BUILD: 3.20.8.0 / 3.20.8.1 / ... / 3.20.8.9

> **Note:**
Statistics for bars BUILD: 3.20.8.0 is calculated as - a summ of latest launches with attribute 3.20.8.0 

[ ![ImageName](Images/userGuide/widgetTypes/CumulativeScheme1.png) ](Images/userGuide/widgetTypes/CumulativeScheme1.png)

[ ![ImageName](Images/userGuide/widgetTypes/CumulativeScheme2.png) ](Images/userGuide/widgetTypes/CumulativeScheme2.png)

[ ![ImageName](Images/userGuide/widgetTypes/CumulativeScheme3.png) ](Images/userGuide/widgetTypes/CumulativeScheme3.png)

[ ![ImageName](Images/userGuide/widgetTypes/CumulativeScheme4.png) ](Images/userGuide/widgetTypes/CumulativeScheme4.png)

[ ![ImageName](Images/userGuide/widgetTypes/CumulativeScheme5.png) ](Images/userGuide/widgetTypes/CumulativeScheme5.png)

[ ![ImageName](Images/userGuide/widgetTypes/CumulativeFirstLevelView.png) ](Images/userGuide/widgetTypes/CumulativeFirstLevelView.png)



A user has an ability to drill down to the second level of the widget. For that he should click on the bar. And the system shows two buttons: Drill Down and Show filter.
And a user should  click on **"Drill down"**.

**For the second level** the system again analyzes the 600 launches from the filter.
Then it leaves only launches which have attribute, that have been clicked by user (f.e. BUILD: 3.20.8.0 ).
From these launches systems chooses ones with attributes  that have key attribute  form the section Level 2 (detailed view) on widget wizard.
After the system groups launches with the same attribute and leaves for each selection only the “latest” launches (launches with unique launch name and with the biggest launch number in ReportPortal).
Others should be removed from a group. Each unique group should be reflected  on the graph on the second widget level.


For each group there is shown a set of bars: Passed, Failed, Skipped, group Product Bug, group Auto Bug, group System Issue, group No defect, group To investigated.

On the hover on the bar, a user can see detailed information about sample. Also user can see a list of attributes with attribute key from the first and from the second levels which have launches, which have been used for a hovered bar.


**Visual options**

**Focus on defect types**
If option is enabled, a user can see only information about defect types for each sample. 
If option is disabled, a user can see information about statuses and defect types.

**Totals**
If option is enabled, a user can see an info about number of test cases in each sample. 

**Staked area / Separete bars**
Staked area chart - is shown a one bar for statuses, and one bar for defect types for each sample. 
Separete bars - is shown a separate bar for  each status, and for each  defect type group. 

**Tests / Per cent**
Test mode - OY axsis is calculated in test cases.
Per cent mode - OY axsis is calculated in per cent. OY = 100%. 

A user can combine different options together. Options are saved per user.

>**Note:**
The widget doesn't contain 'IN PROGRESS" launches. The widget statistics calculated only in items with method type TEST.


## Most popular pattern table (TOP-20)

**Widget's parameters:**
- Filter
- Parameters: All launches/ Latest launches
- Number of shown patterns on the widget: 20
- Attribute key for the first level (mandatory)


For this widget the system chooses 600 last launche by start time from the filter.
Then it leaves only launches  which have attribute with mentioned key and groups launches by attribute value.
System leaves only latest launches in each group (if user has chosen option Latest launches in the widget wizard).
For each group of launhces a list with pattern aggregated.




**Widget view**
On the widget a user can view a table which shows: 

* 20 patterns with the biggest number of test cases in each defined group.

Via drop-down user can transit from group to group.
A pattern name is clickable. By clicking on pattern name a user is redirected to a list with all test cases which have clicked pattern. A list with test cases includes test cases from different launches. 

>**Note:**
The widget doesn't contain 'IN PROGRESS" launches.


## Component health check

Shows the passing rate of the application components which are indicated by the specified attributes. 

>**Note:** for using this widget you need to report (or add manaully) attributes to test items.

[ ![ComponentHEalthCheckWidgetVideo](Images/userGuide/widgetTypes/ComponentHealthCheckView.png) ](https://youtu.be/T98iy0mJk0s)

**Widget's parameters:**
- Filter
- Parameters: All launches/ Latest launches
- The min allowable passing rate for the component: Possible value from 50 - 100%. Default value 100%.
- Attribute key for the first level (mandatory)
- Attribute key for the 2-10 levels (optional)

[ ![ComponentHEalthCheckWidgetVideo](Images/userGuide/widgetTypes/ComponentHealthCheckCreation.png) ](Images/userGuide/widgetTypes/ComponentHealthCheckCreation.png)

**Widget view**


> **Use case:**
>
> **Situation:** As a Project Manager or Test Lead, a I want to see the most unstable place in my product ( application). 
> 
> **Solution:** All test cases in my project in ReportPortal have an attributes. For example `function: (order, team, configure, administrative)`, `type: (backend, API, Unit, UI)`, ...., `marketstate: (open, close)`, `role: (ProjectManager, Member, Admin)` and other. The attributes can be different and dependend on your project needs.
>  
> 
> A user  can create a Component Health Check Widget and set attribute key = `function` for the 1st level, for the 2nd -`type` and for the 3rd - `marketstate`
> 
> So that a user will see on the first level a several groups: order, team, configure, administrative.  All groups will contains only 
> test cases with attribute which contain attribute key `function`. Each group has been grouped by attribute value: order, team, 
> configure, administrative.
> If a user clicks on the group `function: order`, the system will show the second level of the widget. All test items on the second 
> level will be contain the attribute `function: order`and attributes which contain attribute key: `type`. And these items will be 
> grouped by attribute values: backend, API, Unit, UI.
> The same logic will be applied for the next levels.



[ ![ComponentHEalthCheckWidgetScheme](Images/userGuide/widgetTypes/ComponentHealthCheckScheme1.png) ](Images/userGuide/widgetTypes/ComponentHealthCheckScheme1.png)

[ ![ComponentHEalthCheckWidgetScheme](Images/userGuide/widgetTypes/ComponentHealthCheckScheme2.png) ](Images/userGuide/widgetTypes/ComponentHealthCheckScheme2.png)

[ ![ComponentHEalthCheckWidgetScheme](Images/userGuide/widgetTypes/ComponentHealthCheckScheme3.png) ](Images/userGuide/widgetTypes/ComponentHealthCheckScheme3.png)

[ ![ComponentHEalthCheckWidgetScheme](Images/userGuide/widgetTypes/ComponentHealthCheckScheme4.png) ](Images/userGuide/widgetTypes/ComponentHealthCheckScheme4.png)

[ ![ComponentHEalthCheckWidgetScheme](Images/userGuide/widgetTypes/ComponentHealthCheckScheme5.png) ](Images/userGuide/widgetTypes/ComponentHealthCheckScheme5.png)

[ ![ComponentHEalthCheckWidgetScheme](Images/userGuide/widgetTypes/ComponentHealthCheckScheme6.png) ](Images/userGuide/widgetTypes/ComponentHealthCheckScheme6.png)

[ ![ComponentHEalthCheckWidgetScheme](Images/userGuide/widgetTypes/ComponentHealthCheckScheme7.png) ](Images/userGuide/widgetTypes/ComponentHealthCheckScheme7.png)

[ ![ComponentHEalthCheckWidgetScheme](Images/userGuide/widgetTypes/ComponentHealthCheckScheme8.png) ](Images/userGuide/widgetTypes/ComponentHealthCheckScheme8.png)

[ ![ComponentHEalthCheckWidgetScheme](Images/userGuide/widgetTypes/ComponentHealthCheckScheme9.png) ](Images/userGuide/widgetTypes/ComponentHealthCheckScheme9.png)


**Widget level**
Each level shows all available atrributes with corresponded his level attribute key.
For each level system analyze last 600 launches.

**Widget sectin**
Widget has two sections: Passed and Failed
**Failed section has:** all groups (test cases with the same attribute) which have passing rate less than passing rated which has been specified on widget wizard

**Passed section has:** all groups which have passing rate higher than passing rated which has been specified on widget wizard

Each group on the widget has an name which equals to attribute value, passing rate = passed test cases with attribute / total test cases with attribute
number of test cases with attribute 
link to the widget list view: Filter list view + test method: Test + status: Passed, Failed, Skipped, Interrupted, InProgress; the number of items is equal to the number of Test cases in the widget
color line which depends on passing rate (see sectin Widget legend)
Widget legend

Widget legend has two lines: Passed and Failed
 Failed

Failed line has four colors:
-    
-  
-  
-  
And have values - less than specified on widget wizard -1
Passed

Passed line has only two color:

  slightly green  
green = Passed
And have values - from specified on widget wizard to 100%
Depends on this color scheme each group on the widget has own color. 
Groups which have passing rate 100% - has color passed green
Groups whith passing rate from 99 - specified on widget wizard  - has color slightly green
from 3* (Value specified on WW -  1)/4  to (Value specified on WW -1)   
from (Value specified on WW- 1)/2  to 3* (Value specified on WW- 1)/4 - 
from  (Value specified on WW- 1)/4 to  2*(Value specified on WW- 1)/4  
0  - ((Value specified on WW- 1)/4 -1) -



[ ![ComponentHEalthCheckWidgetVideo](Images/userGuide/widgetTypes/ComponentHealthCheckView.png) ](Images/userGuide/widgetTypes/ComponentHealthCheckView.png)

>**Note:**
The widget doesn't contain 'IN PROGRESS" launches.
