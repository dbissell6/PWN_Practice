# OpTinselTrace

![image](https://github.com/dbissell6/PWN_Practice/assets/50979196/387100e3-e261-4b9a-bb8c-4454ec3166c8)


HTB 2023

Hack The Box Sherlocks. 


[OpTinselTrace-1](https://github.com/dbissell6/PWN_Practice/blob/main/OpTinselTrace-1-5.md#optinseltrace-1)

[OpTinselTrace-2](https://github.com/dbissell6/PWN_Practice/blob/main/OpTinselTrace-1-5.md#optinseltrace-2)

[OpTinselTrace-3](https://github.com/dbissell6/PWN_Practice/blob/main/OpTinselTrace-1-5.md#optinseltrace-3)

[OpTinselTrace-4](https://github.com/dbissell6/PWN_Practice/blob/main/OpTinselTrace-1-5.md#optinseltrace-4)

[OpTinselTrace-5](https://github.com/dbissell6/PWN_Practice/blob/main/OpTinselTrace-1-5.md#optinseltrace-5)



# OpTinselTrace-1

![image](https://github.com/dbissell6/PWN_Practice/assets/50979196/dd66259c-9c36-413e-a3dc-150c50e8b2ff)


## Sherlock Scenario

An elf named "Elfin" has been acting rather suspiciously lately. He's been working at odd hours and seems to be bypassing some of Santa's security protocols. Santa's network of intelligence elves has told Santa that the Grinch got a little bit too tipsy on egg nog and made mention of an insider elf! Santa is very busy with his naughty and nice list, so he’s put you in charge of figuring this one out. Please audit Elfin’s workstation and email communications.

## Abstract

# OpTinselTrace-2

![image](https://github.com/dbissell6/PWN_Practice/assets/50979196/130ef1be-1cf8-4269-923d-f4c53f2c4c5f)


## Sherlock Scenario

It seems our precious technology has been leaked to the threat actor. Our head Elf, PixelPepermint, seems to think that there were some hard-coded sensitive URLs within the technology sent. Please audit our Sparky Cloud logs and confirm if anything was stolen! PS - Santa likes his answers in UTC...

## Abstract

# OpTinselTrace-3

![image](https://github.com/dbissell6/PWN_Practice/assets/50979196/271c475d-d7b2-4c1c-833c-7c186fcb65e3)


## Sherlock Scenario

Oh no! Our IT admin is a bit of a cotton-headed ninny-muggins, ByteSparkle left his VPN configuration file in our fancy private S3 location! The nasty attackers may have gained access to our internal network. We think they compromised one of our TinkerTech workstations. Our security team has managed to grab you a memory dump - please analyse it and answer the questions! Santa is waiting…

## Abstract


# OpTinselTrace-4

![image](https://github.com/dbissell6/PWN_Practice/assets/50979196/0dd0e014-56c4-42b3-a789-de449ea32f48)


## Sherlock Scenario

Printers are important in Santa’s workshops, but we haven’t really tried to secure them! The Grinch and his team of elite hackers may try and use this against us! Please investigate using the packet capture provided! The printer server IP Address is 192.168.68.128

## Abstract


## Task 1

### Question

`The performance of the network printer server has become sluggish, causing interruptions in the workflow at the North Pole workshop. Santa has directed us to generate a support request and examine the network data to pinpoint the source of the issue. He suspects that the Grinch and his group may be involved in this situation. Could you verify if there is an IP Address that is sending an excessive amount of traffic to the printer server?`

### Answer
`172.17.79.133`

## Task 2

### Question

`Bytesparkle being the technical Lead, found traces of port scanning from the same IP identified in previous attack. Which port was then targeted for initial compromise of the printer?`

### Answer

`9100`

## Task 3

### Question

`What is the full name of printer running on the server?`

### Answer

`Northpole HP LaserJet 4200n`

## Task 4

### Question

`Grinch intercepted a list of nice and naughty children created by Santa. What was name of the second child on the nice list?`

### Answer

`Douglas Price`

## Task 5

### Question

`The Grinch obtained a print job instruction file intended for a printer used by an employee named Elfin. It appears that Santa and the North Pole management team have made the decision to dismiss Elfin. Could you please provide the word for word rationale behind the decision to terminate Elfin's employment?`

### Answer

`The addressed employee is confirmed to be working with grinch and team. According to Clause 69 , This calls for an immediate expulsion.`

## Task 6

### Question

`What was the name of the scheduled print job?`

### Answer

`MerryChristmas+BonusAnnouncment`

## Task 7

### Question

`Amidst our ongoing analysis of the current packet capture, the situation has escalated alarmingly. Our security system has detected signs of post-exploitation activities on a highly critical server, which was supposed to be secure with SSH key-only access. This development has raised serious concerns within the security team. While Bytesparkle is investigating the breach, he speculated that this security incident might be connected to the earlier printer issue. Could you determine and provide the complete path of the file on the printer server that enabled the Grinch to laterally move to this critical server?`

### Answer

`/Administration/securitykeys/ssh_systems/id_rsa`

## Task 8

### Question

`What is size of this file in bytes?`

### Answer

`1914`

## Task 9

### Question

`What was the hostname of the other compromised critical server?`

### Answer

`christmas.gifts`

## Task 10

### Question

`When did the Grinch attempt to delete a file from the printer? (UTC)`

### Answer

`2023-12-08 12:18:14`

## Discussion



# OpTinselTrace-5

![image](https://github.com/dbissell6/PWN_Practice/assets/50979196/ae00e4a4-c646-40d6-a300-3837fcade3b5)

## Sherlock Scenario

You'll notice a lot of our critical server infrastructure was recently transferred from the domain of our MSSP - Forela.local over to Northpole.local. We actually managed to purchase some second hand servers from the MSSP who have confirmed they are as secure as Christmas is! It seems not as we believe christmas is doomed and the attackers seemed to have the stealth of a clattering sleigh bell, or they didn’t want to hide at all!!!!!! We have found nasty notes from the Grinch on all of our TinkerTech workstations and servers! Christmas seems doomed. Please help us recover from whoever committed this naughty attack!

## Abstract



## Task 1
`Which CVE did the Threat Actor (TA) initially exploit to gain access to DC01?`

### Answer 1
`CVE-2020-1472`

## Task 2
`What time did the TA initially exploit the CVE? (UTC)`

### Answer 2
`2023-12-13 09:24:23`

## Task 3
`What is the name of the executable related to the unusual service installed on the system around the time of the CVE exploitation?`

### Answer 3

`hAvbdksT.exe`

## Task 4 
`What date & time was the unusual service start?`

### Answer 4

`2023-12-13 09:24:24`

## Task 5
`What was the TA's IP address within our internal network?`

### Answer 5

`192.168.68.200`

## Task 6
`Please list all user accounts the TA utilised during their access. (Ascending order)`

### Answer 6

`Administrator, Bytesparkle`

## Task 7
`What was the name of the scheduled task created by the TA?`

### Answer 7

`svc_vnc`

## Task 8
`Santa's memory is a little bad recently! He tends to write a lot of stuff down, but all our critical files have been encrypted! Which creature is Santa's new sleigh design planning to use?`

### Answer 8

`Unicorn`

## Task 9
`Please confirm the process ID of the process that encrypted our files.`

### Answer 9

`5828`

## Discussion
