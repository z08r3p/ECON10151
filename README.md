java c
Lecture   8:   Data   Analysis
Example:   Exploring UK Travel-To-Work Patterns
ECON10151:   Computing   for   Social   Scientists
November   17, 2024
In   this   lecture,   we’ll   walk   through   an   informal   example   of   what   you’re   expected   to   do   in   your   second   assessment,   the   "Integrated Excel Assignment".   The aim of this assignment is to apply the   skills you’ve learned   to   analyse   data   effectively.
1          Choosing   a   Topic   for   Data   Analysis
A critical part of the assessment is selecting the right   topic   for   your   analysis.   Here’s   how   to   choose   one   that   is   both   interesting   and feasible.
•    Start with a research question:   Begin by identifying a research question that interests you, or even   just some key terms   or concepts you’d like to explore.   This will serve as   the   foundation   for   your   analysis.
•    Check data availability and relevance:   Before   you   settle   on   a   specific   topic,   make   sure   relevant   data   is   accessible   and   comprehensive enough to support your analysis.
–    Data   Availability:   Make   sure   that   sufficient   data   for   your   chosen   topic   is   available   through   the   ONS   (Office   for   National   Statistics)   website.         The   ONS   provides   trusted,   government-collected   data   on   a   wide   range   of   topics, including economics, demographics, and social factors.
Check if the data is up-to-date and whether it   directly aligns with your research   question.
–    Scope of Topic:   The   scope   of your topic   should   align with   the   assignment’s   constraints.    If the topic is   too   broad,   you might   struggle to focus your analysis.   Conversely,   a   very   narrow   topic   might   not   have   enough   data   to   explore   thoroughly.
•    Refining   your   question:    After   confirming   a   general   topic,   refine   your   specific   research   question   to   ensure   it   is   clear,   achievable,   and researchable with the available data.   This   step   often   involves   narrowing   the   focus   of a   broader   question   or shifting to a more   specific   aspect   of the topic.
Key   takeaway:   While   it’s   important   to   choose   a   topic   you’re   genuinely   interested   in,   also   ensure   it’s   relevant   to   the   course   content.   A topic that ties in with your studies will make the project both more   engaging   and   academically   valuable.
Today,   we’ll explore   an example related to   urban planning   or   environmental   studies   —   travel-to-work   methods   and   dis-   tances in the UK.
2          Navigating   the   ONS   Website   and   Accessing   the   Dataset
1.    Access   the   ONS   Website:   Go   tohttps://www.ons.gov.uk.
2.    Select   Data   Category:    For   our   purpose,   we   will   use   the   census   2021   data.    Click   on   Data   and   analysis   from      Census 2021.

You   can   also   use   specific   search   terms   related   to your   topic   to   find   relevant   data.    For   example,   if you’re   interested   in   commuting patterns, you   could search   for terms   like    "method of   travel   to work" or   "distance   travelled to   work".      Using   precise search terms will help you narrow down the datasets that are most   relevant to your analysis.
3.    Find the Specific Data:   Navigate through the following options:
•    Census   2021   dictionary > Variables   by   topic >   Travel   to   work   variables   >   Method   of   travel   to   workplace.
4.    Understand the Data:   Review the definitions   and   explanations   of the variables   to   ensure   you   fully   understand   the   data   before proceeding.
5.    Download   the   Data:
•    For   pre-set   data,   simply   click   on   get   the   method   of   travel   to   workplace   dataset.
•    For   custom   data, click   create   a   custom   dataset, and   follow   these   steps:
(a)    Select   population   type:   Choose   your   desired   population, for   example, All   usual   residents, and   click   Continue.
(b)    Add Variables:   Select Add   a   variable >   Browse   available   variables >   Method   used   to   travel   to   workplace >   Continue.
(c)    Customise   Your   Data:   Use   the   Change   button   to   adjust   options   such   as   area   types   (e.g.,   Regions   instead   of Lower   tier   local   authorities) or the number of categories   (e.g., 5   categories instead   of   12   categories).
(d)    Finalise   and   Download:   Click   Get   the   data   and   select   the   Excel   (XLSX)   format   for   download.
3          Method   of   Travel   to   WorkIn   this   analysis,   we   will   explore   the   various   methods   of travel   to   work   across   the   UK,   focusing   on   how   different   transporta-   tion   modes   are   used   in   different   regions.    By   comparing   travel   frequencies   and   regional   variations,   we   can   gain   insights   into   transportation   trends   and   regional   differences   in   commuting   behaviour.    This   analysis   can   inform   decisions   on   transportation   planning, environmental policy, and infrastructure investment.
1.    Preserving   Original   Data:
•    Open the downloaded Excel file and name   the   sheet   containing   the   data   Travel   Method   Data.
•    Create a duplicate sheet called   Travel   Method   Data_Raw to preserve   the   original   dataset.
2.    Data   Cleaning   and   Preparation:
•    Remove duplicated entries or irrelevant   data.
For   instance,   category   code   5,   which represents   "Not   in   employment   or   aged   15   years   and under",   is   not relevant   for our analysis, as we are   focusing   on   the   workforce.
•    To   remove   this   category:
–    Convert the range containing data   into   a   table by   selecting   Insert   >   Table.   A   window   will   appear   asking   you   to confirm the data range and   whether the   table   has   headers.   Ensure   the   correct   range   is   specified   and   tick   the   box if the table has headers.
–    Sort the dataset by   the Method of travel to   work   code   in   ascending   order,   then   filter   for   rows   where   the   code   is 5.   Select and delete those rows (ensure only the   correct rows   are   deleted).
3.    Data   Analysis:
For example, use a   PivotTable to summarise the data and   identify trends   in   commuting   methods:   




(a)    Select   any   cell   and   click   Insert   >   PivotTable.
(b)    By default, Excel will use the entire table.   Choose where to place   the   PivotTable,   such   as   in   the   existing   worksheet   (e.g., cell   H1).
(c)    A   Field   List   will   appear   on   the   right, displaying   all   columns   from   the   table.
(d)    To   analyse   regional   differences, we   need   a   two-way   table:
•    Drag   Regions to the   Rows area   and   Method   used   to   travel   to   workplace   (the   text   variable,   not   the   code)   to   the   Columns area.
•    Drag Observation to the Values area to display total observations   for   each   commuting   method   by   region.
(e)    By default, the PivotTable   shows   sum totals.    However, we   are   more   interested   in   relative   figures,   such   as   percent-   ages, rather than the absolute total observations.   For example, instead of   the total number of   people driving a car to   work in the East Midlands, we want to know the percentage of   people in the East Midlands   who   drive   to   work.
•    Right-click a value in the PivotTable   >   Summarise   Values   By   >   More   Options.
•    Click   on   Show   Data   As   and   select   %   of   Row   Total   from   the   dropdown   list,   then   click   OK.
4.    Visualising   the   Data:
To   further   analyse   the   data, we   can   insert   a   Pivot   Chart:
(a)    Click   any   cell   in   the   PivotTable   to   activate   the   PivotTable   Analyse   tab.
(b)    From there, select   Pivot   Chart, which will create a bar   chart for   each   commuting   method,   grouped   by   region.
(c)    Customise   the   Chart:
•    Add   data   labels   by   clicking   Chart   Design   >   Add   Chart   Element   >   Data   Labels.   Choose   the   desired   position (e.g.,   Outside   End).
•    Give the chart an appropriate   title,   such   as   Methods   of   Travel   to   Work   by   Region.
(d)    To   add   interactivity,   insert   a   Slicer   for   a   more   detailed   view   of   each   region   by   selecting      Insert   Slicer   from   the PivotChart   Analyse tab.
4          Distance   to   Work   vs   Working   Hours
In this analysis, we will examine   the   relationship   between   the   distance   travelled   to   work   and   working   hours.   This   information   is crucial for studying work-life balance and urban planning.
1.    Data   Download:
Go back to the ONS website to download the dataset for the relevant   variables.
(a)    Select   Population   Type:   Choose   your   desired   population, for   example, All   usual   residents, then   click   Continue.
(b)    Add Variables:   Select Add a variable >   Browse available variables, then add   Distance travelled to   work and   Hours   Worked.   Click   Continue.
(c)    Customise   Your   Data:   Use   the   Change   button   to   adjust   options   such   as   area   types   (e.g.,   select   Regions   instead   of Lower   tier   local   authorities).
(d)    Finalise   and   Download:   Click   Get   the   data   and   choose   the   Excel   (XLSX) format   for   download.Note that,   in   practice, you should download data   for all the variables you’re   interested   in   analysing   in   a   single   dataset.   However,for the   purpose of this lecture and to make it easier to   follow, I   have downloaded the data   for   "method of travel   to   work" as   well   as   "distance   travelled" and   "working   hours" separately.
2.    Preserving   Original   Data:


•    Open the downloaded Excel file and copy the dataset into your previous workbook on a new spreadsheet.   Name the   sheet   Distance   and   Hours.
•    Create   a   duplicate   sheet   named   Distance   and   Hours_Raw   to   preserve   the   original   dataset.
3.    Data   Cleaning   and   Preparation:
(a)    Removing   Irrelevant   Data:Remove   irrelevant   categories,   such   as   code   -8   ("Does   not   apply")   for   Hours   Worked,   and   codes   -8   ("Does   not apply")   and   7   ("Works   mainly   at   a代 写ECON10151: Computing for Social Scientists Lecture 8: Data AnalysisR
代做程序编程语言n   offshore   installation,   in   no   fixed   place,   or   outside   the   UK")   for   Distance   travelled to work.
•    Click   any   cell   in   the   dataset.
•    Go   to   the   Data   tab   and   click   on   Filter   to   enable   filtering.
•    Sort   the   dataset   by   the   Hours   Worked   column   in   ascending   order,   then   filter   for   rows   where   the   code   is   -8.   Select and delete these rows   (ensure only the correct rows   are   deleted).
•    Repeat   the   process   to   remove   rows   where   Distance   travelled   to   work   is   coded   as   -8   or   7.   (b)    Data   Recoding:
The variables in the dataset are categorical, which means their codes don’t represent quantitative values.   To perform   meaningful analysis, we need to recode these variables into numerical values.
•    For   Hours   Worked,   the   data   is   binary:   full-time   (2)   or   part-time   (1).    We   can   convert   this   into   a   0/1   format using the   IF function for easier analysis.
Recall that the IF function performs a conditional test, returning one value if   the condition is TRUE and another   if   it   is   FALSE:
= IF(logical_test,value      if      true,value      if      false)
To create   a binary variable for   Hours   Worked,   where   1 represents   full-time   and   0   represents   part-time,   enter   the   following   formula   in   a   new   column   (e.g.,   cell   H2):
= IF(C2   = 2,   1,   0)
Label column   H as Full Time Dummy.
•    For Distance travelled to   Work,   the   data   is   categorical but   has   an   inherent   order.    We   can recode   these   cate-   gories using meaningful numeric values, such as midpoints.
–    For   instance, category   1   ("less   than   5km") can   be   recoded   using   the   median   value   between   0   and   5.   First,   filter   the   rows   where   the   distance   is   coded   as   1, then   in   a   new   column   (e.g.,   I),   enter:
= MEDIAN(0,   5)
–    Apply   the   same   method   for   categories   2,   3,   and   4.
–    For   category   5 ("60km   and   over"),   recode   it   as   60.   For   category   6   ("Works   mainly   from   home"),recode   it as   0.
–    Label   column   I   as   Distance.
(c)    Conditional   Formatting:
To visually distinguish between part-time and full-time observations, we can use conditional formatting to highlight   the relevant cells.
i.    Select   the   Range   of   Cells:   Highlight   the   cells   you   want   to   apply   conditional   formatting   to,   e.g.,   column   H.   ii.    Open   the   Conditional   Formatting   Menu:   Navigate   to   Home   →   Conditional   Formatting.
iii.    Create   a   Rule   for   Part-Time   Observations:   Select   New      Rule...   from   the   drop-down   menu,   then   choose   the Classic style.   Select   Only   format   cells   that   contain and choose Specific   Text.   In the text   box,   type   0.
iv.    Choose a Format:   In the   Format with dropdown, choose   a   fill   colour   (e.g.,   Green   Fill   with   Dark   Green   Text) to highlight part-time entries.   Click OK to apply the rule.
v.    Create   a   Rule   for   Full-Time   Observations: Repeat   the   steps   for   full-time   observations   (Full   Time   Dummy=1),   but   select   a   different   fill   colour   (e.g.,   Red   Fill   with   Dark   Red   Text) to   distinguish   them   from   part-time   entries.
4.    Data   Analysis:
(a)    Compute   the   Average   Distance   Travelled   for   Each   Work   Mode
i.    First, create a column to compute the total distance travelled   for   each   category.   This   is   calculated   as:   Total   Distance   = Number   of   observations   ×   Distance
i.e., we calculate the total distance travelled for   each   category   by   considering   how   many   observations   fall   into
that category and multiplying   by the distance associated with that category.   In   cell   J2,   enter   the   formula:
= G2   * I2
Then, drag the cell down to copy the formula for   all rows.   Label   column   J as   Total   Distance.
ii.    Next,   create   a   summary   table   that   shows   the   total   number   of   observations   for   part-time   and   full-time   work   modes,along with theirrespective average distances:
•    In   cell   N2,   compute   the   total   number   of part-time   observations   using   the   SUMIF   function.    The   SUMIF   function takes three inputs:
SUMIF(range,   criteria,   sum_range)Range   refers   to   the   cells   you   want   evaluated   by   criteria, for   example,   where   the   values   in   H2:H121 equal 0 for   part-time   workers.   The   sum_range   is   the   range   of   values   to   sum,   in   this   case,   column   G.   In   cell   N2,   type:
= SUMIF(H2 :   H121,   “0”   ,   G2 :   G121)
In   cell   N3, do   the   same   for   full-time   workers, replacing   the   criteria   "0"   with   "1".
•    In cell   O2, compute the average distance   travelled   for   part-time   workers.   Use   the   SUMIF function   to   sum   the total distances for part-time workers,   and then   divide   it   by   the   total   number   of part-time   observations.   In   cell   O2,   enter:
= SUMIF(H2 :   H121,   “0”   ,   J2 : J121)/N2
Similarly, in   cell   O3, calculate   the   average   for   full-time   workers.   (b)    Analysis   ToolPak:
We   can   compute   the   correlation   between   work   mode   and   distance   travelled   using   the   Correlation   tool   in   the   Analysis   ToolPak.
i.    Open   the   Data   Analysis   dialog   box:
•    Mac:   Go to   Data   >   Data   Analysis.
•    Windows:   On   the   Data   tab, in   the   Analysis   group, click   Data   Analysis.   ii.    Select   Correlation   from   the   list   and   click   OK.
iii.    In   the   Correlation   dialog   box, set   the   following   options:
A.    Input   Range:   Select   the   range   of   data   you   want   to   analyse.
Note that only   adjacent columns can be   selected,   so   copy   the   values   from   column   H   (Full   Time   Dummy)   into   column   K   to   make   the   columns   adjacent.   Then   select   the   range   J1:K121.
B.    Grouped   By:   Set   this   to   Columns.
C.    Labels   in   First   Row:   Tick   this   box   if   the   first   row   contains   column   headers.
D.    Output   Range:   Choose   where   you   want   the   results   to   be   displayed   (e.g.,   M8),   ensuring   there   is   enough space for the   output.
E.    Click OK. Excel will generate a table   showing the   correlation   coefficients between   the   variables.
(c)      PivotTable and   Pivot   Chart:
We can use   PivotTables and   Pivot   Charts to explore the relationship   between   distance   travelled   to   work   and   work   mode.
i.    Select   any   cell   and   click   Insert   >   PivotTable.
ii.    Ensure   the   correct   data   range   is   selected   and   choose   where   to   place   the   PivotTable,   such   as   in   the   existing   worksheet   (e.g., cell   M16).
iii.    To analyse differences by distance travelled, create a two-way   table:
•    Drag   Distance   to   the   Rows   area   and   Full   Time   Dummy   to   the   Columns   area.
•    Drag Observation to the Values area to   display the   total   number   of observations   for   each   work   mode   and   distance category.
iv.    Again, we are more interested in relative figures, such as percentages, rather than absolute totals.   For example,   we want to know the percentage of   part-time workers who work from home.
•    Right-click a value in the PivotTable   >   Summarise   Values   By   >   More   Options.
•    Click   Show   Data   As   and   select   %   of   Column   Total   from   the   dropdown   list,   then   click   OK.   To insert a   Pivot   Chart:
i.    Click   any   cell   in   the   PivotTable   to   activate   the   PivotTable   Analyze   tab,   and   select   Pivot   Chart.   ii.    Customise   the   chart:
•    Add   data   labels   by   clicking   Chart    Design    >   Add   Chart    Element   >   Data   Labels.    Choose   the   desired   position (e.g.,   Outside   End).
•    Title   the   chart   appropriately,   such   as   Distance   to   Work   and   Work   Mode.
•    To   make   the   distance   categories   on   the   x-axis   clearer, click   anywhere   in   the   chart   to   activate   the   PivotChart Fields, and   drag   Distance   travelled   to   work   (the   text   variable,   not   the   code)   to   the   Axis   area.
You   can   also   drag   Hours   worked   (the   text   variable,   not   the   code)   to   the      Legend   area   to   differentiate   between   0   and   1.
5          Creating   a   Dashboard   in   Excel   to   Present   Results
To create a clear and effective dashboard in Excel,   follow   these   steps   to   summarise   your   findings   and   visualise   the key   results:
1.    Create   a   New   Worksheet:
Start by creating a new worksheet to serve   as your   dashboard.
2.    Remove   Gridlines:
To   give   the   dashboard   a   clean,   professional   look,   remove   the   gridlines.      Go   to   the   View   tab   and uncheck the   Gridlines   box under the Show group.
3.    Add   a   Title:
Insert a text box for the title of your dashboard.   Go to the Insert tab and click on Text Box.   A   suitable title   could be   UK   Travel-To-Work Patterns or something relevant   to your analysis.
4.    Insert   Key   Tables, Figures,   or   Charts:To make your dashboard more visual,   copy   key   tables,   results,   or   charts   from   other   worksheets.    Simply   select the   chart   or   table,   right-click,   and   choose   Copy.    For   tables,   format   them   as   needed   and   use   the   Copy   as   Picture   option.    Then   paste these elements into the dashboard.
5.    Add   Descriptive   Text:
Insert additional text boxes to describe and explain the chosen topic and data analysis, while summarising and discussing   the key findings.   Keep the text concise, focusing on the most important insights   from the   data.
6.    Format   the   Dashboard:
Organise the dashboard by grouping related content together.   Adjust the font   sizes,   styles, and   the   size   of the text boxes,   tables, and charts to ensure everything   fits neatly.
To   improve   the   layout   and   make   it   visually   appealing,   remove   the   outlines   from   charts   and   text   boxes   by   selecting   the   element,right-clicking, and choosing Format Shape > No Line.

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
