# CampusEats_group15

Group members
    1)Maniparthu Manne 
    2)Poornima pulakandam
    3)Vineela Punuru
    4)Koosha Sharifani
    
Project Introduction: 
Students love using food delivery services to order food on campus. CampusEats is website to deliver food on a college campus which provides food delivery 
services to students and staff of the college. The main idea is that the delivery personnel are the students or other authorized employee’s of the university. 
We have an existing database for this website to which we add extra tables and attributes to provide ratings for the drivers and restaurants. 
The ratings are useful for the customers to judge the restaurants,their menu and driver.A customer can be a student, faculty, or staff member on campus. 

Business Rules: 
• All drivers will be students, but not all students are drivers. Drivers will beasubtype of student. 

• Customers are subtype of persons, but are represented by the entities of staff, faculty, and student 

• All Restaurants will have a menu and a menu will have menu item(s) withnutritional information. Orders will pull nutritional information frommenu item(s) inthe order.

• Customers (student, faculty, staff) can view their order details. ● Customers (student, faculty, staff) can rate a driver/delivery person after deliveryof an order.

• Customers (student, faculty, staff) can rate a restaurant from which they orderedfood. 

• All ratings will be from 1 – 5 stars, with 1 representing terrible food/service and5representing great food/service. 

• Customers will be able to view the average ratings of restaurants.

Data Dictionary:
Person: 
Person_id- Unique id for a person 
Person_name- Name of a person 
Person_email- person’s email address 
Cell- Person’s phone number 

Faculty: 
Faculty_id- Unique id for a faculty 
Person_id- Id for certain type of person Title- Title of a faculty 
Degree_college- College name of a faculty Highest_degree- Highest degree earned by a faculty 

Staff: 
Staff_id- Unique id for a staff 
Person_id- Id for certain type of a person Position- Position of the staff 
Is_admin- Checking whether the staff is admin or not 

Student: 
Student_id- Unique id for a student 
Person_id- Id for certain type of a person Graduation_year- Student graduation year Major- Major study by a student 
Type- To know the student is undergraduate or graduate 

Driver: 
Driver_id- Unique id for a driver 
Student_id- Id of a student 
License_number- Driver’s license number 
Date_hired- Date of enjoying 
Rating- Rating of a driver 

Delivery: 
Delivery_id- Unique id for a delivery 
Driver_id- Id of a driver 
Vehicle_id- Id of a vehicle 
Delivery_time- The time of delivery 

Location: 
Location_id- Unique id for a location Location_name- Name of the location Location_address- Address of the location Latitude- Latitude of a location
Longitude- Longitude of a location Drop_off_point- The package drop-off point 

Restaurant: 
Restaurant_id- Unique id of a restaurant Location- Location of the restaurant Restaurant_name- Name of the restaurant Schedule- Working hours of the restaurant Website- Website of a particular restaurant 

Orders: 
Order_id- Unique id for an order Person_id- Unique id for a person Delivery_id- Unique id for a delivery Location_id- Unique id for a location Driver_id- Unique id for a driver 
Restaurant_id- Unique id for a restaurant Total_price- Overall price of the order Delivery_charge- Cost for a delivery Driver_rating- Rating of the driver Restaurant_rating- Rating of a restaurant 

Vehicle: 
Vehicle_id- Unique id for a vehicle Vehicle_plate- Number plate of a vehicle Model- Model of the vehicle Make- Vehicle made year

Ratings: 
Rating_id- id of the rating 
rating- Overall rating 
Order_id- Order id for the ratings 
Driver_ratings: 
Rating_id- Id of the rating 
Ontime_rating- Rating for being ontime 
Restaurant_ratings: 
Restaurant_rating_id- Id for rating the restaurant Rating_id- Id of the rating


EERD is uploded separatley in other file

