
The History App 

Weve been tasked with making a mobile app for a close friend Sarah she would like a special android mobile application; she is massive history buff who wants to inspire the new generation in an interactive history app comparing the users age to famous figures in history . her vision is to bring a fresh experience of history to the next generation. 
The design 

In today’s day and age, we must have an incredible eye-catching design to attract people an keep them engaged having a boring design even if your app is amazing can turn people away. An engaging user interface improves the user’s experience. I used a historical themed background that works well (https://unsplash.com/). The interface is easy to use and very straight forward which is a must the user should not have to try and figure how to use your app, the more straight forward the better. I’ve added a hint for the user to know exactly what to do, with the use of the hint the user just needs to enter their age without the need to erase the text making it seamless the user could be encouraged to try and enter different ages to see all the possible results and learn a small, interesting fact about the famous person. A clear button was inserted to let the user quickly remove the age they’ve entered and try a new one adding to the seamless interaction
The use of github and github actions 
 
Github actions is integration and continuous delivery (CI/CD) this allows you to automate your build, test, and development pipeline. You can create workflows that build  and test every pull request repository, merged pull requests to production (GitHub Docs,2024)
Github Actions does more than just Devops and let run workflows when other events happen in your repository e.g., you can run a workflow to automatically add the appropriate labels whenever someone creates a new issue in your repository.(GitHub Docs, 2024)  

 
GitHub. (2024). [Workflow]. GitHub. [https://docs.github.com/en/actions/learn-github-actions/understanding-github-actions]
A workflow is a automated process that will run one or more jobs. Workflows are defined by a YAML file in your repository and will run when triggered by an event in your repository, or they can be triggered manually, or a defined schedule. (GitHub Docs, 2024)  
The code 
We start with declaring our variables that we will be using , textViewDisplay, editTextAge, buttonGenerate, buttonClear its important to remember to use camel casing when deciding what to name our variables 
textViewDisplay – this variable is used to display our message to the user which will be ‘’Find out what historical figure you’re the same age as when they passed away.’’
editTextAge - this variable will display our hint to the user which is “Please enter your age.”
buttonGenerate – this variable is used as a button which when clicked it will generate the information which will display in the textViewDisplay. 
buttonClear – this variable is used to as a quick way to remove the text the user has entered in the editTextAge.
According to the IIE Module manual(2024) The code inside the listeners brackets, will only get executed when the user clicks the button we call this setOnClickListener. The “a Toast.” Is a message that comes up for a while before it goes away
In our buttonGenerate we have set code which allows the computer to understand what we want from it this includes the range for the age that may be entered which is any age between 20 and 100 in the button we use if, when, in and else statements 
When you declare a variable, you need to assign it a value for example if you where to put favouriteFootballer variable you would need to assign it a “Lional Messi” string value immediately but what if you don’t have a favourite footballer, you might want to assign a variable a “nobody” or “None” value. This wouldn’t be a good idea because the program will interpret the favouriteFootballer variable to have a “Nobody” or “none” value rather than making it have no value at all. In this case you would use null to indicate that there’s no value at all. In the code ive set it to be “ageEntered 1= null)” (android developers, 2024) 
Our when statements are used to tell the machine that “when” something is equal to the number you have entered for example in our app we say if the users age is equal to 24 then output this message “the famous person Dorris Miller passed away at this age”.
I’ve added multiple statements to make it easier to find a match. 23 different famous people have been added 
24 years old - Doris Miller “Dorie” – passed away at this age he was an American naval cook who was the first black recipient of the naval serviceman for his bravery(Britannica, 2024)
25 years old – Tupac Shakur – passed away at this age he was an American rapper and actor who was one of the leading names in 1990s gangsta rap.
32 years old – Bruce Lee – passed away at this age he was an American born film actor who was renowned for his martial arts and who helped popularise the genre.
34 years old – king Henry v – passed away at this age he was a fictional character written by William Shakespeare’s play.
36 years old – Bob Marley – passed away at this age he was a Jamaican singer-songwriter whose thoughtful ongoing reggae music.
40 years old – Paul Walker – passed away at this age he was a famous actor in the franchise fast and furious.
41 years old – Kobe Bryant – passed away at this age he was a famous basketball player who tragically died in a helicopter accident.
42 years old – Elvis Presely – passed away at this age and was a American popular singer widely known as the “King of rock and roll”     
43 years old – Chadwick Boseman- passed away at this age and was a American actor who was most known for his role as black panther.
46 years old – J.F.Kennedy – passed away at this age he was the 35th president of the united states of America.
49 years old – James Garfield – passed away at this age he was the 20th president of the united states of America.
50 years old – Micheal Jackson – passed away at this age and was an American singer who was very well known for his popular music such as thriller.
We end this passage of code with  a else statement. 
Using an in statement we set the range for the age input from the user which is from 20 to 100 using a “const val MAX_VALUE: Int” its used to return the greater of two given values(Codeacedemy, 2024) 
Ending off the code we have a clear button to improve useability of the app making it quick and easy to add another age keeping the user engaged we achieve this by using a buttonClear.setOnClickListerner in this we add both the editTextAge and textViewDisplay variable from earlier where we say setText(“”) this clears the code.
Error handling 
When a user inputs an input which is either outside of our range or an incorrect age like “Seventy” we want the app to display an error message for a number within the age range that does not have a anything set to that age we would like the message “Please enter  another age this age does not have an historical figure.” This is not the only error message we want the program to display as earlier stated if the user inputs “Seventy” we would like the message to display “incorrect age format” .

Referencing
1.	Stack Overflow Question: Title: Incompatible types: IntRange and Int error in Kotlin URL: https://stackoverflow.com/questions/63722733/incompatible-types-intrange-and-int-error-in-kotlin Accessed: [26 march 2024]

2.	Kotlin Standard Library Documentation: Title: Int.MAX_VALUE - Kotlin Programming Language URL: https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/-m-a-x_-v-a-l-u-e.html Accessed: [28 march 2024]


3.	Codecademy Documentation: Title: Kotlin Math Methods: max() URL: https://www.codecademy.com/resources/docs/kotlin/math-methods/max Accessed: [30 march 2024]
LInk to video
https://youtu.be/gids7T27L7Y 
<!---
MustafaaSchmidt/MustafaaSchmidt is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
