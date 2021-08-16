<h1 align = 'center'> Medical Appointment No Shows </h1>

<p align = 'center'><img src = 'assets/no-show_image.png'></p>


<b>Image Source</b> - [afootdoctorsjournal.wordpress.com](https://afootdoctorsjournal.wordpress.com/2018/02/14/dont-be-a-no-show-what-happens-when-you-miss-your-doctor-appointment/)
<br><br>

<h2><b>Kaggle Notebook</b></h2>

[Why Patients DO NOT Show-up? Wrangling, EDA & Viz](https://www.kaggle.com/dishankkalra/why-patients-do-not-show-up-wrangling-eda-viz)
<br><br>

<h2><b>Google Colaboratory</b></h2>

[Medical-Appointment-No-Shows.ipynb](https://colab.research.google.com/drive/1L-CfqAo2XCJVNcLWFeF-E7Kp0Lkpflcn?usp=sharing)
<br><br>

<h2><b>Problem Statement</b></h2> 

Many patients book the appointment with the doctor and then failed to attend scheduled appointments. The average No-Show is 20% leading to `lower clinical efficiency` and `loss of 20 million` every year to the Brazilian economy.<br><br>

<h2><b>Objective</b></h2> 

To investigate the reason why some patients do not show up to their scheduled appointments.<br><br>

<h2><b>Source of dataset</b></h2>

Data was gathered from `kaggle’s` [Medical Appointment No Show](https://www.kaggle.com/joniarroba/noshowappointments) dataset and loaded in `google colaboratory` for analysis.<br><br>

<h2><b>Important Points</b></h2>

• Dataset has more than `100K` records/rows.<br><br>
• In `data-wrangling` major time was devoted to `assessing` and `cleaning data`. Data was `dirty` and `messy` with issues in its content.<br><br>
• Cleaning `invalid data` like float datatype for PatientID and AppointmentID, negative values in age column which is impossible.<br><br>
• Removing `irrelevant data` like Appointment Time which was `00:00:00` (HH:MM:SS) in all the rows, some records have appointment day before the scheduled day.<br><br>
• Transforming `messy data` like ScheduledDay and AppointmentDay having `multiple variables` in date-time format (dd-mmm-yyyy HH:MM:SS) in a single column. They were separated into different columns such that there is `one variable per column`.<br><br>
• Renaming column name in `snake case` to access the column using period with data frame like df.column_name <br><br>
• Summarizing features and finding `descriptive statistics` like a `five-number summary` for the age column.<br><br>
• Handling `outliers` in age column using `68–95–99.7 rule`.<br><br>
• Undertaken `exploratory data analysis` (EDA) to find the important feature responsible for the no-show.<br><br>
• To support our analysis used libraries like `matplotlib` and `seaborn` to make clean, uncluttered design with easy-to-interpret `data visualization`.<br><br>
• Both `categorical` and `quantitative` variables were used for visualization.<br><br>

<h2><b>Conclusion</b></h2>
  
• Important features to predict no-shows are `age`, `hypertension`, `diabetes`, `neighborhood`, and `scholarship`<br><br>

• Showing rate for appointment is more at older age group than younger age group maybe because people are more concerned for their health in old age than than in younger age.<br><br>

• Hypertension is an important characterstic of patients with higher attendance frequency<br><br>

• Showing rate for men and women are similar<br><br>

• Their is no relation of showing up wrt alcholism and handicaps<br><br>

• Enrolment in Bolsa Familia program or scholarhip is an important feature to determine patients with higher attendance frequency<br><br>

• There is no preference for specific weekday over the other when it comes to attendance frequency.<br><br>

• There is no direct relation of No-Show with shorter or longer waiting days between appointment and schedule day.<br><br>

<h2><b>Improvement opportunities at administration level</b></h2>

• Their were no appointments at sundays and appointments at saturday's were signifigantly low in comparison to weekdays. Administration should spread the appointments across months and weekdays regardless of weekends.<br><br>

• Administration should avoid scheduling multiple appointments in the same day for a single patient unless their is emergency. Giving everyone a chance to get second appointment after missing first appointment gives patient a relief of anyway getting another appointment.<br><br>

• Administration should charge a part of fees in advance while patient is scheduling appointment. This may reduce no-show rate.<br><br>

• Administration should follow a systematic approach when sending reminders to patients while closely monitoring the associated costs of sending follow-up reminders<br><br>

<h2><b>Limitations</b></h2>
  
• Appointment Time in all the rows is same that is 00:00:00.If appointment time was specified properly then we could have find time intervals over which people prefer to miss scheduled appointment<br><br>

• Handicap section has five different values(0,1,2,3,4) but on Kaggle author describes it as column with boolean values where 0 represents person with no-handicap and 1 with handicap.We have assumed that 1,2,3,4 are handicaps and changed them all to 1 to represent person with handicap. While 0 represents person with no handicap.<br><br>

• Distance from neighbourhood to the hospital is not given which may prove to be very effective in determining neighbourhoods which are far away from hospital<br><br>

• Dataset only have data for month April, May and June. If data for other months was provided then we could have find months with least show-up rates.
