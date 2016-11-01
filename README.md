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

 * รูปที่ 4 เครื่องทำขนมปัง
 
code

state "Toaster on" as long1

[*] -right-> long1 : turn on

long1 -right-> working

working --> ldle : [upper limit]

ldle -down-> working : [lower limit]

state "shut down" as close

working -right-> close : shut down

ldle --> close : shut down

close --> [*]


[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/RO-n3iCW34HtliBAM8cXQuTyHRSe0seGGQKumaRyVWsaOUc4k7ldiuaDMvYUQ8Xj0emJ68A0qTtLSbj19-zsrdENu06SKnHCzVzb5qnl7vqwNz0riWKhYIKVXumE_kDvLKtK6vOuKXKAM0P4VIlQCqD5srAlW6H7mQ-voJBXWi-AlrPNgYV7VG40)


  * รูปที่5 วงจรชีวิตของไก่

code

[*] --> chicken

chicken --> egg : lay

chick -left-> chicken : grow

egg --> omelet : cook

egg --> chick : hatch

omelet -left-> [*]

chicken --> [*]


[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/YzQALT3LjLD8piXCpaxDuuBIOB7Kz7G5AuMSn4g8g89kJcfQ2K8jK2wzAB-S2wGCf3m_DpKdjGGecfoVdmqNXMYrKiX8B4dEu8AgWPaKhHMBOYE83m00)








Activity Diagram

  * รูปที่1 การตัดสินใจหลังตื่นนอน
  
code

(*) --> "wake up"

if then

--> [hungry] "Eat breakfast"

--> (*)

else

--> [not hungry] "go back to sleep" 

--> (*)

end if


[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/HOjD3a0m44RtFSMNMQd45UoSGYm6KwHDApeYRYz8sBwVehIegXfqi1ViAvd5GMU9vgRjlCTfEpjGmuf-4_QEiz8ZYz8Q2LdUCYR5Lqy9FGyUcf23o4huZpXYSUO2)


