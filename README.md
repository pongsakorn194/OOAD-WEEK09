# OOAD-WEEK09 Homework
##class Diagram

###class Diagram1
Code
```
@startuml
shoppingcenter <|-- foodland
shoppingcenter <|-- shop
shoppingcenter <|-- person
shoppingcenter <|-- park
shoppingcenter <|-- toilet

@enduml
```
Diagram
<img src="https://github.com/pongsakorn194/OOAD-WEEK09/blob/master/Homework/class%20diagram01.png?raw=true ">

###class Diagram2
Code
```
@startuml
scale 750 width
package Data1 <<Node>> {
  class name
}
package Data2 <<Rect>> {
  class address
}
package Data3 <<Folder>> {
  class phonenumber
}
package Data4 <<Frame>> {
  class sex
}
package Data5 <<Cloud>> {
  class age
}
package Data6 <<Database>> {
  class birthday
}
@enduml
```
Diagram
<img src="https://github.com/pongsakorn194/OOAD-WEEK09/blob/master/Homework/class%20diagram02.png?raw=true ">

###class Diagram3
Code
```
@startuml
stone -* cement
Sand --* cement
water --* cement
mortar --* cement
@enduml
```
Diagram
<img src="https://github.com/pongsakorn194/OOAD-WEEK09/blob/master/Homework/class%20diagram03.png?raw=true">

###class Diagram4
Code
```

@startuml
class Account {
  bumber
  balance
  transaction
  deposit()
  withdraw()
  updateaccount()
}
class customer{
  firstname
  lastname
  cardname
  pinnumber
  account
  verifypassword()
}
class transaction{
  transactionid
  transactiondate
  transacttime
  transactiontype
  account
  amount
  postbalance
}

Account "*" *-- "1" customer:has
Account "1" *-- "*" transaction:perform

@enduml
```
Diagram
<img src="https://github.com/pongsakorn194/OOAD-WEEK09/blob/master/Homework/class%20diagram04.png?raw=true ">

###class Diagram5
Code
```
@startuml
class customer {
  name
  surname
  age
  sex
  checkin()
  checkout()
  reserve()
}
class certificate{
  pressindomitory
  signofcustomer
  useiscertificate()
}
class owner{
  name
  surname
  sex
  age
  security()
  recive reserve()
}
class room {
  numberroom
  idroom
  roomdata
  checkin()
  checkout()
}
class domitory {
  domitoryname
  address
  roomprice
  amountofroom
  searchdata()
  searchemptyroom()
}
customer -> owner:reserve
customer -> room:checkin
customer -> certificate:use
certificate -> owner:give
owner -> domitory:maintenance
room -> domitory:in

@enduml
```
Diagram
<img src="https://github.com/pongsakorn194/OOAD-WEEK09/blob/master/Homework/class%20diagram05.png?raw=true ">


 
 
 
