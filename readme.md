# No_Show_Appointments
## by Amos Moses Omofaiye (UDACITY DAND SCHOLAR)


## Dataset

>The *no_show_appointments dataset* contains information from over 100 thousand medical appointments in Brazil. It is focused on the question of whether or not patients show up for their appointment. A number of characteristics about the patient are included in each row. The dataset consists of 14 variables in total. The *independent variables* are 13 and the *dependent variable* is **No-show** 
>
>The independent variables are: 
<ol>
    <li>PatientId: This is a number identifying the patient.</li>
    <li>AppointmentId: This is a number identifying the appointment(s) made by patients. A patient may make more than one appointment.</li>
    <li>Gender: This variable stores the sex of the patient making appointment.</li>
    <li>ScheduledDay: This variable captures the day the appointment was made by the patient.</li>
    <li>AppointmentDay: This is the actual day the appointment is scheduled to occur. It will be later than the  ScheduledDay.
    </li>
    <li>Age: This is the age of the patient who makes the appointment.</li>
    <li>Neighbourhood: This is the place where the hospital is located. As such it is the location where the appointment takes place.</li>
    <li>Scholarship: This captures whether the patient is a beneficiary of the <strong>Bolsa Familia Programme</strong>. This is a federal conditional cash transfer programme in Brazil tied to some responsibilities on the part of the receiver. You can click <a href='https://en.wikipedia.org/wiki/Bolsa_Fam%C3%ADlia'> here </a> to read more on the programme online. Values here are either True or False.</li>
    <li>Hipertension: This variable captures whether a patient has hypertension or not. It can be True or False.</li>
    <li>Diabetes: This variable captures whether a patient has diabetes or not. It can be True or False.</li>
    <li>Alcoholism: This variable captures whether a patient is suffering from alcoholism or not. It can be True or False.</li>
    <li>Handcap: This variable captures whether a patient suffers from one form of physical disability or not. It can be True or False.</li>
    <li>SMS_received: This variable notes whether a patient receives at least an SMS reminding him or her of the appointment before the appointment time.</li>
</ol>

The *dependent variable* is: 
<ul>
    <li>No-show: This captures whether a patient shows up on the day of the appointment or not. If a patient did not show, he/she gets a 'Yes' and a 'No' if he/she shows up.
    </li>
</ul>



#### Research Question
Over the course of the analysis, I explored the following questions:
<ol>
    <li> How does each independent variable except the identification variables correlates with the dependent variable?
    </li>
    <li> What factors are important to predict whether a patient will show up for their scheduled appointment?
    </li>
</ol>

## Summary of Findings

> Conclusively, the following factors appears to be important in determining whether a patient show on the appointment day or not. They are:
<ul>
    <li>neighbourhood</li>
    <li>age (that is age_category)</li>
    <li>hipertension</li>
    <li>sms_received</li>
    <li>scholarship</li>
    <li>delay_days (that is hour_category</li>
    <li>gender</li>
</ul>

## Limitations

> The dataset is massive but has more appointments from some regions. In some of these regions, a great percentage failed to show up. I think it will be better if the dataset is expanded to include more appointments from other regions. Perhaps all appointments in a district or administrative region for a specified period of time should be documented and analyzed in order to be sure of the influence of neighbourhood. An alternative I could have explored is to group some neighbourhoods together but I don't know much about each neighbourhood to warrant this.

> Second, some appointments have the age zero. I want to believe this is not a mistake but it could be. If it is a mistake then those columns should have been dropped. If they are dropped, I believe it will have an impact on this analysis. Such impacts may negate some of the findings here.

> Third, most of the patients that are in the dataset enjoys scholarship. This makes it difficult to conclude on the real influence of scholarship. The data set may be expanded to include a substantial percentage of those that did not enjoy scholarship in order to make the influence of scholarship clearer.