# Gruppe 3 - Uptight Wealth
*Ikke vores valg af gruppenavn*

**Gruppemedlemmer:**
- Cahit
- Marcus
- Michael

Vi benytter datasættet: [Italian Surnames](https://raw.githubusercontent.com/Micniks/Python-Week9-Group-3-Assignments/main/italian_surnames.txt)

Dette github repository er tilrettet opgavestillinger, så udspecifieret her: [Uge7 Opgave](https://docs.google.com/document/d/1ojSiBWwLo4-Rc7763vx6aVEYdNluATOMja9qqk4dodU/edit#) 


# The Mafia Graph

<img src="https://media.thenationaldigest.com/wp-content/uploads/2019/12/02113803/Italian-Mafia-400x400-1.jpg" alt="Italian Mafia" style="max-width: 250px">

### Assignment 1: Identify the Families
*This assignment is meant to make a setup for the two others below, and needs to be completed before the assignement 2 & 3*
1. Read in the surnames from the file ***[italian_surnames.txt](https://raw.githubusercontent.com/Micniks/Python-Week9-Group-3-Assignments/main/italian_surnames.txt)*** into a list.
2. Make two support method ***make_enemies*** & ***owes_money***, that should take a list of surnames (from Assignment 1.1), and return a mafia_graph where surnames have been randomly connected to each other as following:
3. ***make_enemies*** will connect each surname with a list of 5 other randomly selected surnames. These will be considered rival mafia families, like this:
`{'Tony' : ['Giovanni', 'Rizzi']}`
4. ***owes_money*** will connect each surname with a dict of 5 other randomly selected surnames as keys, and a random amount between 10.000 and 100.000 as values. These will be considered what the family owes other families, like this:
`{'Tony' : {'Giovanni' : 10000, 'Rizzi': 20000}}`

## Choose between Assignement 2 and 3:

### Assignment 2: Defeat a Rival
1. Draw a graph made with the ***make_enemies*** method
2. Make a ***defeat_rival*** method that takes a mafia_graph, and a two surname (our_family, our_rival) as parameters.
3. The method should return a list of all surnames that have ***our_rival*** as rivals as well, excluding all surnames that are rivals to ***our_family***.
4. Make a method ***predict_war***, that should use the ***defeat_rival*** method for two families, and return the size for both families, and state which family has the bigger alliance, or if they are at a stalemate.

<img src="https://i.pinimg.com/originals/e0/cc/1d/e0cc1dce1fb78bbe2e18e59a8fb2b441.jpg" alt="Italian Mafia" style="max-width: 50px">


### Assignment 3: Pay the dept
1. Draw a graph made with the ***owes_money*** method
2. Make a method ***pay_dept*** that takes a mafia_graph, and checks the *balance* for each surname, if all depts where to be payed.
3. Make a method ***make_business_empire***, that uses the ***pay_dept*** method to find out the smallest list of richest surnames, that would together control over 50% of all the wealth.

<img src="https://www.nationalcrimesyndicate.com/wp-content/uploads/2020/01/winnings-777x437.jpg" alt="Italian Mafia" width="500px">
