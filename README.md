<h1 align = 'center'> Medical Appointment No Shows </h1>

<p align = 'center'><img src = 'assets/no-show_image.png'></p>


<b>Image Source</b> - https://afootdoctorsjournal.wordpress.com/2018/02/14/dont-be-a-no-show-what-happens-when-you-miss-your-doctor-appointment/
<br><br>
• <b>Problem Statement</b> - Many patients book the appointment with the doctor and then failed to attend scheduled appointments. The average No-Show is 20% leading to <b>lower clinical efficiency</b> and loss of <b>20 million</b> every year to the Brazilian economy.<br><br>

• <b>Objective</b> - To investigate the reason why some patients do not show up to their scheduled appointments.<br><br>

• Data was gathered from <b>kaggle’s</b> [Medical Appointment No Show](https://www.kaggle.com/joniarroba/noshowappointments) dataset and loaded in <b>google colaboratory</b> for analysis.<br><br>
• Dataset has more than <b>100K</b> records/rows.<br><br>
• In <b>data-wrangling</b> major time was devoted to <b>assessing</b> and <b>cleaning data</b>. Data was <b>dirty</b> and <b>messy</b> with issues in its content.<br><br>
• Cleaning <b>invalid data</b> like float datatype for PatientID and AppointmentID, negative values in age column which is impossible.<br><br>
• Removing <b>irrelevant data</b> like Appointment Time which was <b>00:00:00</b> (HH:MM:SS) in all the rows, some records have appointment day before the scheduled day.<br><br>
• Transforming <b>messy data</b> like ScheduledDay and AppointmentDay having <b>multiple variables</b> in date-time format (dd-mmm-yyyy HH:MM:SS) in a single column. They were separated into different columns such that there is <b>one variable per column</b>.<br><br>
• Renaming column name in <b>snake case</b> to access the column using period with data frame like df.column_name <br><br>
• Summarizing features and finding <b>descriptive statistics</b> like a <b>five-number summary</b> for the age column.<br><br>
• Handling <b>outliers</b> in age column using <b>68–95–99.7 rule</b>.<br><br>
• Undertaken <b>exploratory data analysis</b> (EDA) to find the important feature responsible for the no-show.<br><br>
• To support our analysis used libraries like <b>matplotlib</b> and <b>seaborn</b> to make <b>clean, uncluttered design</b> with <b>easy-to-interpret</b> data visualization.<br><br>
• Both <b>categorical</b> and <b>quantitative</b> variables were used for visualization.<br><br>

<h3>Conclusion - </h3>

• <b>Important features</b> to predict no-shows are age, hypertension, diabetes, neighborhood, and scholarship<br><br>

• Showing rate for appointment is more at older age group than younger age group maybe because people are more concerned for their health in old age than than in younger age.<br><br>

• Hypertension is an important characterstic of patients with higher attendance frequency<br><br>

• Showing rate for men and women are similar<br><br>

• Their is no relation of showing up wrt alcholism and handicaps<br><br>

• Enrolment in Bolsa Familia program or scholarhip is an important feature to determine patients with higher attendance frequency<br><br>

• There is no preference for specific weekday over the other when it comes to attendance frequency.<br><br>

• There is no direct relation of No-Show with shorter or longer waiting days between appointment and schedule day.<br><br>

<h3><b>Improvement opportunities at administration level - </b></h3>

• Their were no appointments at sundays and appointments at saturday's were signifigantly low in comparison to weekdays. Administration should spread the appointments across months and weekdays regardless of weekends.<br><br>

• Administration should avoid scheduling multiple appointments in the same day for a single patient unless their is emergency. Giving everyone a chance to get second appointment after missing first appointment gives patient a relief of anyway getting another appointment.<br><br>

• Administration should charge a part of fees in advance while patient is scheduling appointment. This may reduce no-show rate.<br><br>

• Administration should follow a systematic approach when sending reminders to patients while closely monitoring the associated costs of sending follow-up reminders<br><br>

<h3><b>Limitations - </b></h3>
• Appointment Time in all the rows is same that is 00:00:00.If appointment time was specified properly then we could have find time intervals over which people prefer to miss scheduled appointment<br><br>

• Handicap section has five different values(0,1,2,3,4) but on Kaggle author describes it as column with boolean values where 0 represents person with no-handicap and 1 with handicap.We have assumed that 1,2,3,4 are handicaps and changed them all to 1 to represent person with handicap. While 0 represents person with no handicap.<br><br>

• Distance from neighbourhood to the hospital is not given which may prove to be very effective in determining neighbourhoods which are far away from hospital<br><br>

• Dataset only have data for month April, May and June. If data for other months was provided then we could have find months with least show-up rates.
