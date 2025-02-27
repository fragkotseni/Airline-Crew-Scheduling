# Airline-Crew-Scheduling
Problem Description: Airline Crew Scheduling
Airlines need to assign pilots and flight attendants to flights while ensuring that the total number of crew hours and costs are minimized, while adhering to strict regulations regarding crew work hours and rest periods. The challenge is to balance operational efficiency, costs, and crew well-being by scheduling the right number of pilots and flight attendants for a set of flights.

Given the constraints on working hours and rest periods, the airline needs to minimize the cost of crew assignments while satisfying the required crew availability for each flight.


Data and Assumptions:

Pilot Wage: $300 per flight

Flight Attendant Wage: $150 per flight

Flights: 3 flights (Flight A, Flight B, Flight C)

Required Crew per Flight:

Flight A: 1 Pilot, 2 Flight Attendants

Flight B: 1 Pilot, 3 Flight Attendants

Flight C: 1 Pilot, 2 Flight Attendants


Constraints:

Pilot Work Hours: A pilot can work a maximum of 8 hours per day.

Flight Attendant Work Hours: A flight attendant can work a maximum of 8 hours per day.

Crew Rest Period: A pilot and flight attendant must have at least 10 hours of rest between shifts.


Objective Function:

Minimize the total cost of crew assignments, where the cost is calculated based on the number of pilots and flight attendants assigned to flights.

Linear Programming Model
Objective Function:
Minimize the total cost of pilots and flight attendants: 
Minimize
 
𝐶
=
300
⋅
𝑃
𝐴
+
300
⋅
𝑃
𝐵
+
300
⋅
𝑃
𝐶
+
150
⋅
𝐹
𝐴
+
150
⋅
𝐹
𝐵
+
150
⋅
𝐹
𝐶

MinimizeC=300⋅P 
A
​
 +300⋅P 
B
​
 +300⋅P 
C
​
 +150⋅F 
A
​
 +150⋅F 
B
​
 +150⋅F 
C
​

  where:

𝑃
𝐴
,
𝑃
𝐵
,
𝑃
𝐶
P 
A
​
 ,P 
B
​
 ,P 
C
​
  are the number of pilots assigned to flights A, B, and C.
𝐹
𝐴
,
𝐹
𝐵
,
𝐹
𝐶
F 
A
​
 ,F 
B
​
 ,F 
C
​
  are the number of flight attendants assigned to flights A, B, and C.
Constraints:
Pilot Work Hours: Each pilot can work only 8 hours per day: 
𝑃
𝐴
+
𝑃
𝐵
+
𝑃
𝐶
≤
8
P 
A
​
 +P 
B
​
 +P 
C
​
 ≤8

Flight Attendant Work Hours: Each flight attendant can work only 8 hours per day: 
𝐹
𝐴
+
𝐹
𝐵
+
𝐹
𝐶
≤
8
F 
A
​
 +F 
B
​
 +F 
C
​
 ≤8

Rest Period: Each pilot and flight attendant must have at least 10 hours rest: This can be represented by ensuring no overlap in the work hours or by modeling specific timing between shifts.

Flight Crew Requirements: For each flight, we need the specified number of pilots and flight attendants:
For Flight A: 
𝑃
𝐴
=
1
P 
A
​
 =1 and 
𝐹
𝐴
=
2
F 
A
​
 =2
For Flight B: 
𝑃
𝐵
=
1
P 
B
​
 =1 and 
𝐹
𝐵
=
3
F 
B
​
 =3
For Flight C: 
𝑃
𝐶
=
1
P 
C
​
 =1 and 
𝐹
𝐶
=
2
F 
C
​
 =2
