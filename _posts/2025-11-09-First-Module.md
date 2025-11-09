---
layout: post
title: Launch into Computing
subtitle: Each post has a subtitle
categories: Module for Data Science
tags: [Github, Modules]
---
## 1.	A summary of the learning outcomes of the module
•	Learned in depth concepts of Computing, Software Engineering, Artificial Intelligence, Data Science, and Cyber Security.

•	Studied the basic principles, processes, and procedures of software design and implementation methodologies.

•	The technologies and principles that form the basis of Artificial Intelligence implementations were also studied.

•	Explored the current and future challenges, limitations, and opportunities in the field of computing.

•	An understanding of how computing concepts and devices can be used to overcome barriers to equality, diversity and inclusion

•	Developed a presentation where the presentation focused on Artificial Intelligence presenting critical arguments for specific actions and outcomes to a diverse audience.

## 2.	The artefacts created during the module

Collaboration discussion: The Evolution of Computing and Its Impact on Business and Society

### Initial Post

#### Introduction
Data Science is a computing field that brings together computational methods, data analysis, and scientific methods to extract meaningful insights from big and complex datasets. This computing discipline uses tools from mathematics, computer science, and statistics to solve real world problems, make predictions, and support decision making.

#### How Data Science transformed industries and societies in recent decades
Data Science has transformed industries and societies in aspects such as: Digital banking, and streaming services have now replaced the traditional ways of doing things, have increased turnaround time, and created an environmentally friendly business process. Different social media platforms, messaging applications, emails, and internet have completely changed how societies across the world communicate and share information. 

There are positive influences from how computing has transformed industries and societies, however this transformation has also brought in negative impact such as data security, cybersecurity, and replacement of human jobs. 
In conclusion, smart city initiatives in South Africa are pushing for smart city development in major cities such as Cape Town and Johannesburg. Companies specialising in network sensors, urban management systems for water and electricity, and traffic monitoring can play a critical role in these projects. These companies can provide advanced sensor technology for monitoring environmental conditions, traffic patterns, and other data intensive applications (Digital Economy Report 2024, United Nations Publications).

#### The impact of computing in the banking sector
Banks have jumped on the opportunities offered by internet, and mobile banking applications. It is possible to do everything online these days, starting from a simple transaction to complicated matters such as applying for a mortgage bond. Some banks are now only available virtually, and banks like Smile in the UK and Simple in the US do not have any physical branches at all.

#### References:

Lou Brodie, M.L., 2019. What is data science?. In Applied data science: Lessons learned for the data-driven business (pp. 101-130). Cham: Springer International Publishing.

Digital Economy Report 2024. Shaping an environmentally sustainable and inclusive digital future. United Nations Publications.

Wise Mission Report Q2 2018. Available at: https://wise.com/us/blog/transferwise-mission-report-q2-2018. (Accessed: 03 August 2025).

Van Der Aalst, W., 2016. Data science in action. In Process mining: Data science in action (pp. 3-23). Berlin, Heidelberg: Springer Berlin Heidelberg.

### Summary Post
The collaborative discussion was based on the topic “The Evolution of Computing and Its Impact on Business and Society”, and my focus was on Data Science (DS). Big data or DS happened early in the 20th century where there was a shift from traditional statistics to predictive modelling, and business intelligence (Rosenberg, 2020). The United States Data Science Institute argues that “A significant 59% of organisations across the world believe that Data Science analytics is a key factor in gaining a competitive advantage in business”. 

Two peer responses were received for the discussion. Daniel Lopez agreed with my definition of DS including elements mentioned as components of DS. Daniel advised that practical examples on how DS transformed some cities in South Africa should have been included, and I completely agree with the suggestion.

The second peer response was from Kyle Au, and Kyle’s response was in agreement with my discussion on how DS has transformed the banking industry. Kyle suggested that DS professionals must always upskill themselves as to keep updated with changes in the field. 

Summary of unit 1 to 4 includes learnings from how Artificial Intelligence (AI) revolutionised industries, but this came with challenges such as algorithms bias in AI, for example, machine learning models mistakenly discriminating against certain groups due to biased training data, and lack of accountability in such incidents is a problem. Logical, and mathematical principles supporting computing such as Boolean logic, logic gates, and set theory were also deliberated in the past four weeks. It was interesting to learn how Boolean algebra and set theory work in computing. The fundamental principles of computer science such as algorithms, data structures, and computational complexity were also discussed in-depth, and how these principles support problem solving, and an efficient storage and retrieval of data. Lastly, Software engineering was studied, where Software Development Life Cycle (SDLC) phases were discussed in detail across different aspects of computing.  
To sum up, computing will continue to change and shape every aspect of modern life across the globe, and creating opportunities for innovation, but this will also come with increased challenges in cybersecurity, privacy and digital inequality.

#### References:

Elliott, S., 2021. Projecting the Impact of Computers on Work in 2030. In National Academies Workshop on Research Evidence Related to Future Skill Demands.

Rosenberg, R.S., 2020. The social impact of computers. Elsevier.

United States Data Science Institute (January 28, 2025): Data Science Evolution over the Decades and Future Advances. Available at: https://www.usdsi.org/data-science-insights/data-science-evolution-over-the-decades-and-future-advances#: (Accessed: 20 August 2025).

Wempen, F., 2014. Computing fundamentals: Introduction to computers. John Wiley & Sons.

### Feedback from the Tutor for the collaboration discussion 
Veli provided a solid and contextually relevant contribution to the discussion, particularly focusing on the importance of data science and data quality. The initial post was articulate, with clear structure and appropriate referencing, demonstrating understanding of technical aspects such as statistical methods and data mining. However, while the peer responses were respectful and added value, they leaned toward general agreement and lacked deeper critical engagement or probing questions. The summary post effectively reflected on personal learning and highlighted connections across peers’ posts, but would benefit from a more analytical tone. Overall, the submission shows good understanding and effort, with room for improvement in critical depth.

### SAS program to use to develop a Bubble sort algorithm
/*Create a dataset named "Algorith_Bubble_Sort" in a temp library called work*/; 

data Algorith_Bubble_Sort 

 /*Defining an array with 10 unsorted integers*/;
 
 array bubble_array[10] (88, 92, 12, 28, 79, 3, 33, 52, 68, 47); 
 
    length sorted_bubble_array $80;
    
/*Function to return the number of elements in a one-dimensional array*/;   

    a = dim(bubble_array); 
    
    /* Start with the Bubble sort algorithm using the do loop*/
    
    do x = 1 to a-1;
    
        do y = 1 to a-x;
        
            if bubble_array[y] > bubble_array[y+1] then do;
            
                /* If the condition above is true, then swap the elements in the array*/
                
                Bin_array = bubble_array[y];
                
                bubble_array[y] = bubble_array [y+1];
                
                bubble_array[y+1] = Bin_array;
                
            end;
            
        end;
        
    end;
    
/*Print the final results of the sorted array of 10 numbers*/

title "Sorted bubble array numbers";

proc print data=Algorith_Bubble_Sort;

### Comparing two software development methodologies
Comparing two software development methodologies, Waterfall, and DevOps, highlighting their flexibility and adaptability to changing requirements, projects’ suitability, risk management and quality assurance.

### Evaluation  the security position of Artificial Intelligence (AI) systems
Developed a report evaluating the security position of Artificial Intelligence (AI) systems deployed within an organisation, identifying vulnerabilities, threats, and mitigation strategies. The main objective is to ensure ethical, transparent, safe, and robust AI operations within organisations. Artificial Intelligence is defined as the simulation of human intelligence in machines that are programmed to think, learn, and make decisions like human beings. The AI programmed systems can perform tasks that naturally require human understanding, such as understanding language, recognising patterns, making decisions, and learning from data. 

### Disaster recovery plan (DRP)
Develop a disaster recovery plan (DRP) for the organisation, including:

•	Steps to restore operations during and after a disruption.

•	Tools and technologies for example AWS Elastic Disaster Recovery, Bacula for backups.

•	Methods to ensure data integrity and minimise downtime.

### IT Governance Framework Analysis
Select an enterprise IT governance framework between  COBIT, ITIL, or TOGAF and analyse how the framework can be applied in a hypothetical organisation to achieve the following:

•	Align IT goals with business objectives.

•	Mitigate IT-related risks.

•	Optimise IT resources for competitive advantage.

Consider a hypothetical medium to large enterprise called Cloud Operations Ltd in South Africa, whose operations are heavily depended on cloud services. Cloud Operations Ltd has outsourced all its computing infrastructure, applications, and data storage to external cloud provider, that uses Google Cloud Platform. The company’s mission revolves around providing real time analytics and AI driven insights to clients globally, necessitating scalable, distributed, and highly reliable computing resources.

### Evaluating the development models of two programming languages
Developing and comparing two programming languages based on two small utility applications that perform the same function in both languages.

### The Python code
This Python program is developed using the Google Colab platform to display a calendar for 2 given months and year. The user is prompted to input the year, first month and second month and once the program is executed, the calendar for the 2 months in the specific given year.

#/ This statement imports the calendar module.
import calendar

#/ The statements below prompt the user to input the year, month 1 and 2.

year = int(input("Input a year and then press Enter (e.g., 2018): "))

month1 = int(input("Input the first month and then press Enter (1 - 12): "))

month2 = int(input("Input the second month and then press Enter (1 - 12): "))

#/ The statements below display the calendar for month 1.

print(f"\nCalendar for {calendar.month_name[month1]} {year}")

print(calendar.month(year, month1))

#/ The statements below display the calendar for month 2.

print(f"\nCalendar for {calendar.month_name[month2]} {year}")

print(calendar.month(year, month2))

### The Ruby code
The Ruby code below is developed using the Online Ruby Compiler platform to display a calendar for 2 given months and year. The user is requested to input the year, first month and second month and once the program is executed, the calendar for the 2 months in the specific given year.

#/ The statement code calls the date library into the program code.
require 'date'

#/ The statements below ask the user to input the year, month 1 and 2.

print "Input the year and then press Enter (e.g., 2015): "

year = gets.chomp.to_i

print " Input the first month and then press Enter (1 - 12): "

month1 = gets.chomp.to_i

print " Input the second month and then press Enter  (1 - 12): "

month2 = gets.chomp.to_i

#/ The programming statements below print the calendar for a given year and month. 
def print_calendar(year, month)

#/ The (1) creates a new date object representing the first day of a specific month in a given year.

  first_day = Date.new(year, month, 1)

#/ The (-1) defines the last day of the month in using the Ruby date library.

  last_day = Date.new(year, month, -1) 

#/ The statement below "\n#{Date::MONTHNAMES is a constant array defined in the 
Ruby date library to hold the full names of the months, indexed from 1 to 12. 
  puts "\n#{Date::MONTHNAMES[month]} #{year}"

  puts "Su Mo Tu We Th Fr Sa"

  #/ The statements below print all leading space for a proper display.

  print "   " * first_day.wday

  (first_day.day..last_day.day).each do |day|

     print day.to_s.rjust(2) + " "

     first_day = first_day.next_day

     puts if first_day.wday == 0
  end

  puts "\n"

end

#/ The programming statements below display the calendars for month 1 and 2 together with the year.

print_calendar(year, month1)

print_calendar(year, month2)

### The presentation
#### Introduction
In 2023, a private hospital in Johannesburg, South Africa tested an Artificial Intelligence (AI) system to detect early signs of eyes disease, trying to improve early detection of eyes’ diseases in patients and also improve patients experience in healthcare. Today, we will explore in-depth the AI environment. 

### What is (AI)?
It is important to first understand AI as a field in computer science. Artificial Intelligence is defined by Abbass (2021: pp 94-95) as “a social and cognitive phenomena that enables a machine to socially integrate with a society to perform competitive tasks requiring cognitive processes and communicate with other entities in society by exchanging messages with high information content and shorter representations”. 

Expanding the definition by Abbass, it is imperative to know that AI involves creating systems that can perform tasks that require human intelligence, for example learning, problem solving, and decision making at different levels. AI uses different technologies to enable machines to learn, see, understand human language, analyse big data, and make recommendations.

## 3.	What exactly have I learnt and how
### 3.1 What to Learn
•	Computing Fundamentals

•	Programming basics in Python

•	Digital literacy

•	Data and information

•	Computational thinking

•	Professional and academic skills

### 3.2 The how part of learning the above
•	Hands-on practice from unit 1 to 12

•	Project based learning

•	Critical reflection and collaboration discussions

•	Blended learning

•	Assessment preparation 

## 4.	Professional skills gained and enhanced as a result of the module 
•	Identify and critically analyse computing challenges and processes in business systems, accounting for the current enterprise landscape.

•	Gather and synthesise information from multiple sources (including internet resources and business publications) to aid in the systematic design and analysis of computing challenges.

•	Critically evaluate appropriate methodologies, tools and techniques to mitigate and/or solve computing issues and their business impact.

•	Communicate the legal, social, ethical, and professional issues faced by computing professionals.
