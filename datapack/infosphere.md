---
layout: default
title: Infosphere
parent: Datapacks
nav_order: 2
---

# Infosphere

## Infosphere node generator

1. Identify or roll security class
2. Specify abilities and security features
3. Select or roll the appearance if you wish
4. Select or roll the data stored in the node

[Online generator](https://oswida.github.io/cyber/app/dist/#/gen?lang=en&mode=Infosphere)

## Security class

1. Public
2. Private
3. Private secured
4. Government
5. Corporation
6. Military
7. AI

## Abilities and security features

Every Infosphere node has HP, INF abilities and additional parameters related to its security procedures.
Reducing a node's HP to zero means taking control, reducing INF to zero means destroying data.
The following table describes the abilities and protection mechanisms for each security class.

- The `HP` and `INF` specify the die to be used to roll the value of the ability (along with the modifier)
- The `ICE` determines the attack die for the Intrusion Countermeasure Electronics and determines the chance that a given ICE will be black (we roll the Fate Dice, x/6 means that the results from 1 to x give a positive answer).
- The `Activation Threshold` informs about the maximum value that activates additional protection program in a given round.

| Security class  |  HP   |  INF  | Activation Threshold | ICE attack die  |
| --------------- | :---: | :---: | :------------------: | :-------------: |
| Public          | d4+1  |  d4   |          1           |       d4        |
| Private         | d4+1  |  d4   |          2           |       d4        |
| Private secured | d6+2  |  d6   |          3           |       d6        |
| Government      | d8+3  |  d8   |          5           | d8, 1/6: Black  |
| Corporation     | d10+4 |  d10  |          7           | d10, 2/6: Black |
| Military        | d12+5 |  d12  |          9           | d12, 3/6: Black |
| AI              | d20+6 |  d20  |          12          | d20, 4/6: Black |

### Additional protection software

Each node may have additional protective software. Its activation is not necessarily inevitable and depends on the result of the roll during the ICE attack.
The procedure does not require any additional dice roll - the value is taken from the ICE attack, if the roll result is less than or equal to the activation threshold, in the same round the program is launched and its type is taken from the protective software table, also based on the value of attack.

| d4 - d20 | Protective Software                                     |
| :------: | ------------------------------------------------------- |
|    1     | HP +1 (*)                                               |
|    2     | HP +2 (*)                                               |
|    3     | HP +3 (*)                                               |
|    4     | Armor +1                                                |
|    5     | Armor +2                                                |
|    6     | Armor +3                                                |
|    7     | Dispersion: the hacker's next attack is impaired        |
|    8     | Critical damage: additional d4 damage                   |
|    9     | Critical damage: hacker's attack impaired for d4 rounds |
|    10    | Critical damage: hacker disconnected for d4 rounds      |
|    11    | Firewall: inability to hack in the next round           |
|    12    | Double attack (roll two dice, choose the higher result) |

(*) If the hacker controlled the node,at the time of the HP increase, he loses that control until he reduces the node's HP to zero again.

> Example of protective software activation
>
> Ian attacks the corporate node, which means the ICE has d10 attack die.
> Additionally, d6 roll gives the result of 2 which means that the attacked ICE is "black" (in case of failure in the critical damage test, Ian will receive additional PSY damage)
> At the time of the attack, ICE rolls 5. It means that:
>
> - Ian will receive **5 points of damage** (at first he subtracts it from his HP and then from his INF).
> - An additional protection program has been **activated** (activation threshold 7)
> - The effect of the protection program is **+2 armor** in this round (**item 5** in the table), the damage dealt to the node by Ian will be reduced by 2 (the attack of the hacker and the node are resolved simultaneously)  

## Appearance (3d20)

| d20 | Shape                 | Color and/or material           | Details                                        |
| --- | --------------------- | ------------------------------- | ---------------------------------------------- |
| 1   | Sphere                | Ruby, transparent               | Laser beams filling the shape                  |
| 2   | Pyramid/ziggurat      | Transparent                     | Mathematical symbols displayed on the surface  |
| 3   | Infinity symbol       | Black, matte                    | Burning with bright light                      |
| 4   | Cube                  | Silver                          | Luminous rings swirling around                 |
| 5   | Mock-up of a building | Green, neon                     | Advertising slogans displayed on the surface   |
| 6   | Mask                  | White, glossy                   | Reminiscent of origami                         |
| 7   | Menhir                | Black, glossy                   | Filled with lightning bolts                    |
| 8   | Circle                | Blue, glowing                   | Filled with ice crystals                       |
| 9   | Model of an atom      | Gray, stony                     | Without any additional markings                |
| 10  | Logo                  | Blue, hazy                      | Large company/owner logo                       |
| 11  | Moebius ribbon        | Green, luminous                 | Glowing cubes inside                           |
| 12  | Rubik's cube          | Red, flaming                    | Mystical symbols swirling around               |
| 13  | Screen                | Multicolored                    | Randomly appearing specks of light             |
| 14  | Vortex                | Gold                            | Random grid images displayed inside            |
| 15  | Column                | Metallic, shiny                 | Wrapped in a metallic grid                     |
| 16  | Triangle              | Dark blue, covered with streaks | Flashing regularly with dim light              |
| 17  | Eye                   | Glass, transparent              | Spinning around its own axis                   |
| 18  | Gate                  | Dappled, brown                  | Rotating segments continuously                 |
| 19  | Trapezoid             | Orange, bright                  | Dynamic fractals drawn on the surface          |
| 20  | Perpendicular         | Steel, covered with symbols     | Every now and then it disappears and reappears |

## Data to be acquired (d20)

If your hackers are breaking into Infosphere nodes to get their hands on valuable data, the following tables may provide inspiration.

### Public

1. A set of old computer games
2. Big book of recipes
3. Plans of a public building
4. Answers to questions in the upcoming multimedia quiz
5. Cheats for a popular online game
6. Recipe for homemade stimulants
7. A volume of poems of questionable quality
8. Very interesting designs of fashionable clothes
9. List of winners of a beauty contest that has not yet taken place
10. The world's largest collection of music
11. Unknown encrypted data
12. Public building security camera recording
13. Timetable of a well-known media star
14. Footage of violent police intervention
15. Footage of activist protests at the factory gate
16. Footage of a terrorist group's manifesto
17. Official statement of the hacker group
18. Full medical data on a drug for a known disease
19. Technical plans for a police drone
20. List of corrupt police officers

### Private

1. Medical data stolen from Administration hospital
2. Technical plans of an unknown cybermod
3. Collection of videos ... of various kinds
4. A collection of articles about mysterious genetic experiments
5. 1k4 tickets to a famous sporting event
6. A set of 1k4 computer viruses
7. Manuscript of an unpublished novel (could be good)
8. Entry codes to a private apartment
9. Correspondence with a corporation regarding compensation
10. Data archive on a well-known celebrity
11. Medical records indicating an incurable disease
12. Launch codes for a private vehicle
13. Redacted manifesto of a terrorist group
14. Guide on how to make a bomb
15. A collection of love emails
16. Authorized Last Will
17. Wedding invitations and guest list
18. Photos of an illegal cyber clinic
19. Amateur footage of a hack
20. Unknown song by a famous music band

### Private secured

1. A set of fake documents
2. 1k4 false signatures for vehicles of any type
3. Bank account details with 1k4 thousand credits
4. 1k4 tickets for an upcoming concert at the opera house
5. 1k6 hacking programs of various types
6. Codes for hacking power lines in the selected district
7. Input codes for several apartments in a regular high-rise building
8. Addresses of families of known gang bosses
9. Two passes to an exclusive restaurant
10. Entry codes to a private garage
11. Passwords to corporate email account
12. Electronic key for k6 weapons cache
13. Diary of an important politician
14. Media star's contact list
15. Network address of a corporate executive
16. Input code to one of the corporate arcologies
17. Password for an account with a platinum basic subscription
18. Access codes for a cache of illegal stimulants
19. Contact address for a known fixer
20. Receipt document for cybermod / combat drone

### Government

1. Codes to open all doors of the selected Administration office
2. Security camera record with recorded crime
3. Evacuation plans in the event of an epidemic of a publicly unknown infectious disease
4. Report on mutant animals encountered by municipal workers
5. Financial testimonies of well-known politicians
6. Ultimatum from terrorist group threatening chemical contamination
7. Financial data indicating an impending economic crisis
8. Report on radioactive contamination in one of the city's districts
9. Information on the termination of the corporation's rights to the land occupied by the factory
10. Detailed plans of the selected city district
11. Property deed of a small city property
12. Input codes for the Administration hospital system
13. Report on the bizarre behavior of the AI managing city transportation
14. 1k6 permissions to operate public transport (blank)
15. Calendar of power line shutdowns in different parts of the city
16. Draft of the new tax law for citizens
17. Input codes for the warehouse of the city hospital
18. Passwords and codes that enter an epidemiological emergency
19. 1k4 blank forms that allow identity registration
20. Access codes for the control system of selected municipal services

### Corporation

1. The latest yet-to-be aired episodes of a popular series
2. Compromising recordings of an important corporate employee
3. Detailed plans of one of the corporation's arcologies
4. Personal information of an entire corporate department
5. List of bank accounts of a well-known corporate employee
6. Production documentation of a rare vaccine
7. Data of employees suspected of espionage
8. Personal files of employees of a rival corporation
9. Set of entry passes for arcology
10. Compromising data of politicians
11. Technical data of the company's latest product
12. Information on the financing of terrorist groups
13. List of police officers in the service of the corporation
14. List of Administration officials at the service of the corporation
15. Plans to take control of gangs in the district
16. Contacts to individuals/companies hired for 'wet work'
17. Documentation of illegal genetic experiments
18. Passwords to a warehouse full of the corporation's products
19. Orders to transport unknown materials to a research facility
20. Plans for a corporate research facility

### Military

1. Technical plans of the combat drone
2. Input codes for military base
3. Remote control codes for a military fighter jet
4. Program decrypting transmissions on tactical network
5. Technical plans for a military robot
6. Weapons storage input codes
7. Pass codes to the military cybermod warehouse
8. Address data of important military commanders
9. Production documentation of military stimulants
10. Military satellite control codes
11. Satellite images showing illegal research facilities
12. List of competitor spies in a selected corporation
13. Orders to exterminate the population in case of an unknown disease threat
14. Documentation of a deadly virus grown in a laboratory
15. Nuclear warhead deployment plans
16. Transcripts of discussions of meetings of the board of directors of a selected corporation
17. List of corporate AIs perceived as a threat
18. Technical plans for a super-light EMP weapon
19. Technical plans for the EMP-emitting cyber-arm
20. List of military spies in corporations

### AI

1. Construct (personality record) of a deceased celebrity
2. Atomic Energy Agency node technical data
3. Source codes of another AI
4. Input codes to all police systems
5. Set of 1k6 powerful computer viruses
6. Password for a node that is completely resistant to hacking
7. Password to an anonymous account with 1k20k credits
8. Procedure for one-time access to any node in the Infosphere
9. A virus that shuts down security systems in the indicated building for 1k20 minutes
10. Automatic military vehicle control codes
11. Control codes of the public transportation system
12. Recipe for addictive stimulant k10
13. Codes for an intercontinental missile with nuclear warheads
14. Medical data of an experiment related to human immortality
15. Data of a secret research facility breeding human mutants
16. Virus completely blocking transmissions of selected media network
17. Secret military plans to attack one of the corporations
18. Evidence that one corporation is completely run by AI
19. Plan of attack on the Infosphere to be carried out by rogue AIs
20. A destructive virus, instantly deleting all data on the node on which it was launched

# Basic algorithms

## PC actions

![PC actions](img/PC%20actions.svg)

## Physical combat

![Physical combat](img/Physical%20combat.svg)
![Physical attack](img/Physical%20attack.svg)

## Infosphere node attack

![Infosphere attack](img/Infosphere%20attack.svg)

## ICE attack

![ICE attack](img/ICE%20attack.svg)

# Additional algorithms

Several additional mechanisms to expand Infosphere gameplay.

## Clashes between hackers

The basic version of the game assumes that hackers can attack nodes in the Infosphere and be attacked by Intrusion Countermeasure Electronics.
But what happens if several hackers from opposite sides meet?
The neuroprocessor gives the hacker a much greater ability to operate the Infosphere but at the same time exposes him to direct attacks from the network.

It is possible to attack the hacker's mind in a similar way to the Infosphere node.
Such an action has to be performed by another hacker; no software can do it. There are rumors that some AI also happened to attack the human mind.

The clash follows the same rules as for nodes. The opponents **attack with neuroprocessors** and the damage is dealt first in the opponent's HP and then INF. Attacks take place simultaneously.
Reducing the hacker's OCHR to zero or below means that the other side can **take control of the stimuli** received by the defeated party for **as many rounds as their current INF**.

Taking control only applies to the hacker's sensorium (sight, hearing, smell), it does not include motorics, i.e. you cannot control the opponent's body. But you can instead completely control his perception.

## Supporting

If two or more hackers wish to coordinate their actions when attacking a node, their actions are accounted for similarly to multiple attackers in the combat rules.
Roll **all** damage dice and keep one **chosen** result.
The difference with physical combat (where the highest score is chosen) is that hackers can modify the effect of an attack with programs. When resolving the attack, **only those programs** that belong to the **owner of the selected roll** can be activated.

## Passengers

Any hacker can connect any number of ordinary access devices to his neuroprocessor. This way, outsiders who do not have a neuroprocessor can have constant contact with him and even observe his online activities. However, none of the passengers can take any action in the Infosphere; their participation is limited only to passive observation or communication with the hacker.
