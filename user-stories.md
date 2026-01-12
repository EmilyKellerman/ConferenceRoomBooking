## Story #[1]: [Basic room booking for employee]
**As a** [Employee]
**I want to** [be able to book a room for use]
**So that** [I can reserve a room for a conference or meeting]
### Acceptance Criteria:
- [ ] Given [a room is shown to be available for booking], When [an employee selects the room], Then [they should be given the option to book the room and make it unavailable at the times they stipulate]
- [ ] Given [a room has been booked by an employee], When [the room is marked as booked], Then [the system notes which user made the booking privately]
### Story Points:
[3]
### Priority:
[High]
### Dependencies:
- None
### Technical Notes:
- Assuming there is a log in system to have access to the booking features
### Design Notes:
- UI / UX considerations or edge cases
_______________________________________________________________________________________

## Story #[2]: [Recurring meetings setup]
**As a** [Employee]
**I want to** [view a meeting timetable]
**So that** [I can access a timetable showing which rooms are booked on a weekly basis and which times they're booked]
### Acceptance Criteria:
- [ ] Given [an employee has access to the terminal], When [they select the timetable], Then [they should be able to view and download the timetable with recurring meetings]
### Story Points:
[3]
### Priority:
[Medium]
### Dependencies:
- [1]
### Technical Notes:
- Assuming there is a log in terminal for employees and that booking is done per week and that employees will be able to download files on their device
### Design Notes:
- UI / UX considerations or edge cases
_______________________________________________________________________________________

## Story #[3]: [Room Capacity Filtering]
**As a** [Employee]
**I want to** [filter the rooms by capacity of each room]
**So that** [I can book a room based on how many people are in attendance]
### Acceptance Criteria:
- [ ] Given [the employee has access to the booking system], When [they toggle the filter], Then [the rooms should be ordered in order of least to most, or most to least capacity]
### Story Points:
[1]
### Priority:
[Medium]
### Dependencies:
- None
### Technical Notes:
- Assuming there is a log in terminal for employees
### Design Notes:
- UI / UX considerations or edge cases
_______________________________________________________________________________________

## Story #[4]: [Booking cancellation]
**As a** [Employee]
**I want to** [be able to cancel a booking]
**So that** [the room becomes available to others if plans change]
### Acceptance Criteria:
- [ ] Given [an employee has access to the system and has booked a room], When [they view the room they hace booked], Then [they should have the option to cancel their booking]
- [ ] Given [an employee is the one who created the booking], When [they choose to cancel the booking], Then [it should only work if it's the employee who created the booking]
- [ ] Given [an employee did not create a booking], When [they choose to cancel a booking they did not make], Then [an error should show and redirect them to the home page]
### Story Points:
[3]
### Priority:
[High]
### Dependencies:
- [1]
### Technical Notes:
- Assuming there is a log in terminal for employees and that each booking notes the user who created the booking
### Design Notes:
- UI / UX considerations or edge cases
_______________________________________________________________________________________

## Story #[5]: [Room Equipment Requirements]
**As a** [Employee]
**I want to** [be able to view the room equipment requirements]
**So that** [I can come to the venue prepared with the neccessary equipment]
### Acceptance Criteria:
- [ ] Given [the employee has access to the system], When [they select the room they want to book], Then [the equipment requirments should show in the description of the room]
### Story Points:
[1]
### Priority:
[Medium]
### Dependencies:
- None
### Technical Notes:
- Assuming there is a log in terminal for employees
### Design Notes:
- UI / UX considerations or edge cases
_______________________________________________________________________________________

## Story #[6]: [Admin dashboard Viewing]
**As a** [Admin]
**I want to** [log into the administrator dashboard]
**So that** [I can make changes to information or edit access control]
### Acceptance Criteria:
- [ ] Given [the administrator has access to the admin dashboard], When [the correct username and password is entered], Then [the dashboard should be made available to them]
- [ ] Given [an employee tries to log in], When [an invalid username and password is entered], Then [an error should inform the user that it is invalid information]
### Story Points:
[2]
### Priority:
[High]
### Dependencies:
- None
### Technical Notes:
- Assuming there is a log in terminal for employees and admins
### Design Notes:
- UI / UX considerations or edge cases
_______________________________________________________________________________________

## Story #[7]: [Room Maintenance Scheduling]
**As a** [Facilities Manager]
**I want to** [be able to schedule rooms for maintenance]
**So that** [rooms become inaccessible while maintenance is in progress]
### Acceptance Criteria:
- [ ] Given [Facilities managers have access to the system], When [they select the room that needs maintenance], Then [the room should become inaccessible to employees and get marked down as under maintenance]
- [ ] Given [facility manager have finished maintenance], When [they select the room that has finished maintenance], Then [they should be able to change the state of the room to available]
### Story Points:
[Choose from: 1, 2, 3, 5, 8, 13]
### Priority:
[High]
### Dependencies:
- None
### Technical Notes:
- Assuming there is a log in terminal for employees and that there is a way for the system to differentiate between them and facilities managers
### Design Notes:
- UI / UX considerations or edge cases
_______________________________________________________________________________________

## Story #[8]: [Visito Booking Assistance]
**As a** [Receptionist]
**I want to** [be able to assist an employee in the booking process]
**So that** [I can book a room on their behalf or aid a visitor in the process if they need access to the service]
### Acceptance Criteria:
- [ ] Given [The reseptionist wants to assist someone], When [they select a room that they want to book], Then [they should be able to select who has booked the room]
- [ ] Given [someone that isnt the receptionist wants to book for someone else], When [they select a room to be booked], Then [they should not be able to book for anyone other than themself]
### Story Points:
[3]
### Priority:
[Low]
### Dependencies:
- [1]
### Technical Notes:
- Assuming there is a log in terminal for employees and that there is some way for the system to differentiate the receptionist from other employees
### Design Notes:
- UI / UX considerations or edge cases
_______________________________________________________________________________________

## Story #[9]: [Booking Conflict Resolution]
**As a** [Admin]
**I want to** [receive notification if there are booking conflicts]
**So that** [I can log into the administrator dashboard to resolve the conflict]
### Acceptance Criteria:
- [ ] Given [there is a system error or conflict with booking], When [the notification is sent to the administrator], Then [the admin should be given a link to the problem to be resolved]
- [ ] Given [the admin has resolved the conflict], When [the admin has done], Then [the relevant people should be notified of the fix]
### Story Points:
[8]
### Priority:
[High]
### Dependencies:
- [1, 6]
### Technical Notes:
- Assuming there is a log in terminal for employees and administrators and that the system is able to send communication between users
### Design Notes:
- UI / UX considerations or edge cases
_______________________________________________________________________________________

## Story #[10]: [Usage Reports Generation]
**As a** [Admin]
**I want to** [Be able to generate a report on the usage of rooms during the month]
**So that** [I can share the data with relevant team members and make changes to the system if neccessary]
### Acceptance Criteria:
- [ ] Given [the admin has access to the administrator dashboard], When [they select to receive a usage report], Then [a document with a summary on the usage of rooms should be downloaded to the selected location on the admin's device]
### Story Points:
[3]
### Priority:
[Low]
### Dependencies:
- [1, 6]
### Technical Notes:
- Assuming there is a log in terminal for employees and admins and that the employees are able to download documents
### Design Notes:
- UI / UX considerations or edge cases
_______________________________________________________________________________________