# HOTEL-BOOKING-ANALYSIS-EDA
EXPLORATORY DATA ANALYSIS ON HOTEL BOOKING DATA
# Objective
The main objective is that to perform EDA on the given dataset and draw useful conclusions about general trends in hotel bookings and how factors governing hotel bookings interact with each other and which is the best time for booking .
# Dataset
1) hotel: Name of hotel ( City or Resort)

2)  is_canceled: Whether the booking is canceled or not (0 for no canceled and 1 for canceled)

 3) lead_time: time (in days) between booking transaction and actual arrival.


 4) arrival_date_year: Year of arrival

 5) arrival_date_month: month of arrival

 6) arrival_date_week_number: week number of arrival date.

7)  arrival_date_day_of_month: Day of month of arrival date

8) stays_in_weekend_nights: No. of weekend nights spent in a hotel

9) stays_in_week_nights: No. of weeknights spent in a hotel

10) adults: No. of adults in single booking record.

 11) children: No. of children in single booking record.

12) babies: No. of babies in single booking record.

13) meal: Type of meal chosen

14) country: Country of origin of customers (as mentioned by them)

15) market_segment: What segment via booking was made and for what purpose.

16) distribution_channel: Via which medium booking was made.

17) is_repeated_guest: Whether the customer has made any booking before(0 for No and 1 for Yes)

18) previous_cancellations: No. of previous canceled bookings.

19)  previous_bookings_not_canceled: No. of previous non-canceled bookings.

20) reserved_room_type: Room type reserved by a customer.

21) assigned_room_type: Room type assigned to the customer.

22) booking_changes: No. of booking changes done by customers

23) deposit_type: Type of deposit at the time of making a booking (No deposit/ Refundable/ No refund)

24) agent: Id of agent for booking

25) company: Id of the company making a booking.

26)  days_in_waiting_list: No. of days on waiting list.

27) customer_type: Type of customer(Transient, Group, etc.)

28) adr: Average Daily rate.

29) required_car_parking_spaces: No. of car parking asked in booking.

30) total_of_special_requests: total no. of special request.

31) reservation_status: Whether a customer has checked out or canceled,or not showed.

32) reservation_status_date: Date of making reservation status.

# Libraries used: Numpy, Pandas, Matplotlib, Seaborn

# Data preparing and cleaning

check is there any null value or missing values a.  In this dataset we get 112593 null value in 'company' column so I have replaced the null values with 0. b.  In the 'agent' column I have also get 16340 so I have replaced it with 0. c.  In country I can not set the country values as 0 becuase it contains country codes representing different countries. So instead of replacing it with zero we have replaced it with the mode value in country column. Mode is nothing but just the most repeating value. d.  Children Column has the count of children then I replaced missing values with mean values.
Dropping some coloumn which does not make any sense Several rows in the dataset contains values that does not make any sense like having no adults, children and babies so we directly deleted it by using drop.
Change the data type Check the types of datatypes and converting it into int64.

# Exploratory data analysis
Hotels type ratio?

which month has maximum arrival in the year ?

Yearwise booking ?

From which country the most guests came?

Most Number of Guest ?

How many booking cancelled ?

monthly cancellations?

market segment wise booking?

What is the Percentage of repeated guests?

Which type of food is mostly preferred by the guests?

which is the busiest month for hotel booking?

Which is the busiest month for Resort and City Hotel?

night stay?

Which is the home country of guest?
# conclusion

1) The pie chart reveals that 66% of the hotels in the dataset are city hotels and the other 34% are resort hotels.

(2) the months of November to March are off-peak periods for hoteliers. Between June and the end of August, attendance is at its peak, it is the high season.

(3) the booking for city hotel is higher than resort yearwise.

(4) Most of the guests came from european countries, with most of guests coming from Portugal.

(5) the most number of guests are 48483 which is from Portugal.

(6) more than 30000 booking were cancelled in city hotel followed by more than 10000 in resort hotel.

(7) most of the transient customers had cancelled the booking.

(8) Most of the market_segment used Online TA and Offline TA/TO

(9) Repeated guests are very few which is only 3.1 %. In order to retained the guests , hotels/resort management should take feedback from the guests in order to imporve their services.

(10) most preferred meal type by the guests is BB.

(11) most of the busiest months are July and August

(12) City hotel has maximum booking from the month April to September but after that there is fall down in booking Now for the Resort hotel March-May,June-August and November-January is busiest month.

