RaceDay Database Business Rules

1. Introduction

The RaceDay database is designed to store information relating to users, sporting events, event categories, participant enrolments, results and event routes.

The following business rules were identified during Part 1 — Planning and System Design.



2. User Rules

BR01

A user must have a unique user account.

BR02

A user must have an assigned role.

BR03

A user can be an Organiser or a Participant.

BR04

An Organiser can manage events.

BR05

A Participant can enrol in events.



3. Event Rules

BR06

An Organiser can manage multiple events.

BR07

Each event is associated with an Organiser.

BR08

An event can contain multiple categories.

BR09

An event can have multiple participant enrolments.

BR10

An event can have zero or one route associated with it.



4. Category Rules

BR11

Each category belongs to an event.

BR12

An event can have multiple categories.

BR13

A category can be selected by multiple Participants through enrolments.



5. Enrolment Rules

BR14

A Participant can have multiple enrolments.

BR15

An event can have multiple enrolments.

BR16

Each enrolment is associated with one Participant.

BR17

Each enrolment is associated with one Event.

BR18

Each enrolment is associated with one selected Category.

BR19

An enrolment may have zero or one result.



6. Result Rules

BR20

A result belongs to an enrolment.

BR21

An enrolment can have no result until the participant’s result is captured.

BR22

A result should only be managed by an authorised Organiser.

BR23

Participants should only be able to view their own results.



7. Route Rules

BR24

An event can have zero or one route.

BR25

Route information belongs to a specific event.

BR26

Authorised Organisers can manage route information.



8. Data Integrity

BR27

Primary keys shall uniquely identify records.

BR28

Foreign keys shall be used to maintain relationships between related tables.

BR29

Required information should not be allowed to contain NULL values where the database design identifies the field as mandatory.

BR30

The database should prevent invalid relationships between records.



9. Part 2

These business rules support the database design created during Part 1.

The database structure and relationships will be implemented and further tested during Part 2.
