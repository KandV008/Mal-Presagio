# :video_game: Mal Presagio :video_game:

## :bookmark_tabs: Table of Contents

1. [Introduction](#ledger-introduction)
    1. [Start-up the applicaction](#rocket-start-up-the-applicaction)
    2. [Preview](#circus_tent-preview)
2. [Functional Analisis](#black_nib-functional-analisis)
    1. [Entities](#large_blue_circle-entities)
    2. [Users](#bust_in_silhouette-users)
    3. [Functional requirements](#wrench-functional-requirements)
    4. [No Functional requirements](#pushpin-no-functional-requirements)
    5. [Use cases diagrams](#bar_chart-use-cases-diagrams)
3. [Application Design](#art-application-design)

---

## :ledger: Introduction

This game is the final project of the Programming Methodology course.

The objective is to develop software in all its phases, being the following:
1. Analisis
2. Design
3. Implementation
4. QA

### :rocket: Start-up the applicaction

### :circus_tent: Preview

## :black_nib: Functional Analisis

### :large_blue_circle: Entities

| Entities |  | Subentities | |
| :-: | :-: | :-: | :-: |
| Character | Vampire | Lycanthrope | Hunter |
| Special Skill | Discipline | Gift | Talent
| Equipment | Weapon | Armour |
| Modifier | 
| Minion | Human | Ghoul | Daemon |
| User | Registered User | Operator |
| Challenge |
| Combat |

### :bust_in_silhouette: Users

- Unregistered User -> This user can't use the application, it has to create an account to access to the system.
- Registered User -> This user use all the actions related to challenges and combats.
- Operator User -> This user only can administrates the users and validate challenges.

### :wrench: Functional Requirements

| Function | Unregistered User | Registered User | Operator |
| :-: | :-: | :-: | :-: |
| Create Account | :white_check_mark: |  |  |
| Delete Account | | :white_check_mark: | :white_check_mark: |
| System Access | | :white_check_mark: | :white_check_mark: |
| Recover password | | :white_check_mark: | :white_check_mark: |
| System Exit | | :white_check_mark: | :white_check_mark: |
| Register Character | | :white_check_mark:| |
| Edit Character | | | :white_check_mark: |
| Unsubscribe a character | | :white_check_mark: | |
| Select active weapon | | :white_check_mark: | | 
| Select active armour | | :white_check_mark: | |
| Add weapon to a character | | | :white_check_mark: |
| Remove weapon to a character | | | :white_check_mark: |
| Add armour to a character | | | :white_check_mark: |
| Remove armour to a character | | | :white_check_mark: |
| Add modifier to a character | | | :white_check_mark: |
| Remove modifier to a character | | | :white_check_mark: |
| Challenge a user | | :white_check_mark: | |
| Accept a challenge | | :white_check_mark: | |
| Decline a challenge | | :white_check_mark: | |
| See battle log | |:white_check_mark: | |
| See global ranking | |:white_check_mark: | |
| Validate a challenge | | | :white_check_mark: |
| Ban user | | | :white_check_mark: |
| Unban user | | | :white_check_mark: |
| See gold | |:white_check_mark: | |
| Combat | | :white_check_mark: | |

### :pushpin: No Functional Requirements

#### Operational Requirements

* Persistence
    * The information will be saved in a local folder and file system.
    * The data is saved when the account is created, logged out, a challenge, accept a challenge and perform the combat of a challenge.
    * If it is considered necessary to save it at another time it can be done.

#### Security Requirements

* To access the system the user must register. 
* The user can only access the system with his account by entering his nickname and password.
* The user can recover password with the name he entered when he created his account.

#### Performance requirements

* Number of users: Many users, but only one active user.

### :bar_chart: Use Cases Diagrams

![system access](/readme-files/Functional-Analisis/system_acces.svg)
<small> Figure 1 System Acces </small>

![operator actions](/readme-files/Functional-Analisis/operator_actions.svg)
<small> Figure 2 Operator Actions </small>

![user actions](/readme-files/Functional-Analisis/user_actions.svg)
<small> Figure 3 User Actions </small>

![challenges](/readme-files/Functional-Analisis/challenges.svg)
<small> Figure 4 Challenges

![character selection](/readme-files/Functional-Analisis/character_selection.svg)
<small> Figure 5 Character Selection </small>

![character edit](/readme-files/Functional-Analisis/character_edit.svg)
<small> Figure 6 Character Edit </small>


## :art: Application Design
