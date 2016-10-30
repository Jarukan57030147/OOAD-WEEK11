# OOAD-WEEK11
State Diagram

     *     รูปที่1 การปิดเครื่องคอมพิวเตอร์
 code
[*] --> Ready

Ready : waiting for instructions

Ready -right-> off : switch is turned off

off : shut down the power

off --> [*]


[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/BOqx3e0m34Ftdi8pKY_0m25O4KFL3ysIe3HLnUtvYCM3txEyJJkyNx3ca2xt9MQCG4Pye8Y2k9dsQ2JSVi4h7TMUbPJos6sGnGfgiAwSqrkx7zLkI38OLZDE6La_ybvkq-vk)



   * รูปที่ 2 การเปิดเครื่องคอมพิวเตอร์
   
code

[*] -right-> off

off : shut down the power

off -right-> on : turn on the computer

on -down-> Boot :switch on computer

off : shut down the power

Boot : loading the system

Boot -left-> Ready : Booting computer

Ready : waiting for insttuctions

Ready --> [*]

[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/TSqx3eCm30RWdLDuHie563hq25qHGvG7YGGsIXn5tBvnQClKmPBb_xCzZmke5DV0wW7a_T0A9iYXC5Yg21mS75HTwibDiIak2QKJOsW_2Wj3KBBPq9E8OSeriWdYRlFtoRK26saRSUr1FZEx_KhKvhoyVpbjp-PaAEvt-HjK7NlWAK74p5mCHyBy0QhTcCTbU0C0)


  * รูปที่ 3 การเล่น Disc
  
code

[*] -right-> ldle

ldle : no disc

ldle -right-> waitingAction : Insert Disc

waitingAction --> PlayDisc : Play

PlayDisc --> [*]


[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/YzQALT0joapFAD6rKyX9oKdb0X4ALWfv-GefcSN942vSHNbYPabcNhfZSabcVXvGbMTUSMfHYO8BI2Mgd2vGTK1EOYL82gWGnEI2yq6IqLgnN000)

