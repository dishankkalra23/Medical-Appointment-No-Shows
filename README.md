<h1 align = 'center'> Medical Appointment No Shows </h1>

<img src = 'assets/no-show_image.png'>

• <b>Problem Statement</b> - Many patients book the appointment with the doctor and then failed to attend scheduled appointments. The average No-Show is 20% leading to <b>lower clinical efficiency</b> and loss of <b>20 million</b> every year to the Brazilian economy.<br>
• <b>Objective</b> - To investigate the reason why some patients do not show up to their scheduled appointments.<br>
• Data was gathered from <b>kaggle’s</b> [Medical Appointment No Show](https://www.kaggle.com/joniarroba/noshowappointments) dataset and loaded in <b>google colaboratory</b> for analysis.<br>
• Dataset has more than <b>100K</b> records/rows.<br>
• In <b>data-wrangling</b> major time was devoted to <b>assessing</b> and <b>cleaning data</b>. Data was <b>dirty</b> and <b>messy</b> with issues in its content.<br>
• Cleaning <b>invalid data</b> like float datatype for PatientID and AppointmentID, negative values in age column which is impossible.<br>
• Removing <b>irrelevant data</b> like Appointment Time which was <b>00:00:00</b> (HH:MM:SS) in all the rows, some records have appointment day before the scheduled day.<br>
• Transforming <b>messy data</b> like ScheduledDay and AppointmentDay having <b>multiple variables</b> in date-time format (dd-mmm-yyyy HH:MM:SS) in a single column. They were separated into different columns such that there is <b>one variable per column</b>.<br>
• Renaming column name in <b>snake case</b> to access the column using period with data frame like df.column_name <br>
• Summarizing features and finding <b>descriptive statistics</b> like a <b>five-number summary</b> for the age column.<br>
• Handling <b>outliers</b> in age column using <b>68–95–99.7 rule</b>.<br>
• Undertaken <b>exploratory data analysis</b> (EDA) to find the important feature responsible for the no-show.<br>
• To support our analysis used libraries like <b>matplotlib</b> and <b>seaborn</b> to make <b>clean, uncluttered design</b> with <b>easy-to-interpret</b> data visualization.<br>
• Both <b>categorical</b> and <b>quantitative</b> variables were used for visualization.
• <b>Important features</b> to predict no-shows are age, hypertension, diabetes, neighborhood, and scholarship
