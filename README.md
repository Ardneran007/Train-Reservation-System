# Train-Reservation-System

Overview:

•	Used AVL Trees to implement.
•	A Train Database of 10 trains is maintained in a Tree to maintain the SEAT MATRIX and allocate proper seat to User.

•	The Trains are given id from 25671 to 25680(a try to make it real)

•	Seat Allocation
    o	When a user wants to allocate a seat in a certain class a SEAT is allocated to him in the proper coach and Train No and the seat number is CLASSNAME-SEATNUMBER (eg. 2AC-4).

•	Seat Deallocation
    o	When a User cancels his Reservation then his seat is deallocated from the SEAT-MATRIX from Train Database and the seat is made available for next reservations.

•	INSERTION:
    o	The First Comparision is made wrt  train_id as we want to keep Data sorted according to Train_id  But if the Train id is same The comparision is Done wrt 
        Passenger id as it would be beneficial for searching and Cancellation of Reservation.
        
    o	When a USER makes a RESERVATION in a certain Train a proper seat is allocated using the SEAT ALLOCATION method.

•	DELETION
    o	As done in Insertion first comparision is done wrt Train_id and then Passenger_id to find the Passenger and Cancel its Reservation
    
    o	If Reservation is cancelled successfully then seat is deallocated using the SEAT DEALLOCATION method.

•	GETLISTDESTINATION
    o	Comparision is firstly done wrt Trainid and then wrt Destination station due to which the passengers having same Trainid and Destination will come together and using 2 pointers a LIST with passengers having same destination and Train is made.

•	SORT BY TRAVEL DATE 
    o	A compare function is implemented to compare the dates and accordingly passenger Node is inserted in TREE

•	SORT TRAINS
    o	The SEAT MATRIX of Train also maintains Number of Reservations Done due to which it is easy to SORT TRAIN

•	RANGESEARCH
    o	The Trainid are within (25671-25680) so input must be given accordingly.
    
    o	 A simple scan of TrainDatabase is done and the Trains are displayed when it is in given Range.  
