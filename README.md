DEX401 - Anypoiont Development Fundamentals Classroom Reference - 260608 - EDT

Vincent Lowe

vlowe@salesforce.com

Cloudshare Virtual Machines: https://use.cloudshare.com/Class/90jk1

Cloudshare Passphrase: Shumba the Running Hummingbird

-------------------------------------------------------------------------------------------------------------------
Trailhead Academy:						https://trailheadacademy.salesforce.com/my-learning


Salesforce Mimeo:							https://salesforce.mimeo.digital/MuleSoft

eBook Redemption Key:					US7HRFV3SWSA

-------------------------------------------------------------------------------------------------------------------
Survey Link:									https://www.research.net/r/trailheadacademy

Survey ID:										TASM-2138960

-------------------------------------------------------------------------------------------------------------------
Zoom Link:
https://trailheadacademy.salesforce.com/instructor-classes#class-id=a8yRf000001V9UfIAK

Meeting ID: 84520209233

Class System Setup (pre-class): https://trailhead.salesforce.com/help?article=Computer-Setup-Guide-for-MuleSoft-Expert-Led-Classes#DEX401

Advanced REST Client:
https://github.com/advanced-rest-client/arc-electron/releases/tag/v17.0.9

Self paced course: 
https://trailhead.salesforce.com/users/strailhead/trailmixes/getting-started-with-anypoint-platform-dex-401

Postman:
https://www.postman.com/downloads/

-------------------------------------------------------------------------------------------------------------------

Kyle Burke on Error Handling:
https://blogs.mulesoft.com/dev-guides/how-to-tutorials/mule4-error-handling/

Vincent's Blog
https://techwhine.panreality.com/

Help:
https://help.mulesoft.com/

Docs:
https://docs.mulesoft.com
   
------------------------------------------------------------------------------

Java VM: https://docs.mulesoft.com/general/java-support

MuleSoft Pricing & Support: https://www.mulesoft.com/anypoint-pricing

------------------------------------------------------------------------------

%dw 2.0
output application/json
---
payload map ( payload01 , indexOfPayload01 ) -> {
	ID: payload01.ID,
	code: (payload01.code1
default "") ++ (payload01.code2 default ""),
	price: payload01.price default 0,
	departureDate: payload01.takeOffDate as String default "",
	origin: payload01.fromAirport default "",
	destination: payload01.toAirport default "",
	emptySeats: payload01.seatsAvailable default 0,
	plane: {
		"type": payload01.planeType default "",
		totalSeats: payload01.totalSeats default 0
	}
}

------------------------------------------------------------------------------


|Track Title|Artist|Notes|
|-----------|------|-----|
|The Streetb3eater|Quincy Jones|TV theme from Sanford & Son|
|I Was Doing All Right|Louis Armstrong||
|Just Breathe|Willie Nelson feat. Lukas Nelson||
|Stairway to Heaven|Luca Stricagnoli|One man and a guitar with three necks|
|Sixteen Tons|Geoff Castellucci||
|Good Morning American|Arlo Guthrie||
|California|Rebecca Loebe||
|Ain't Misbehavin'|Leon Redbone||
|Tupeo Honey|Elle Cordova||
