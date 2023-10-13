# 5320
IN5320 project built on the DHIS2 platform  
Sierra Leone: Kono: Lei: Komba Yendeh CHP  


This is the DHIS2 app of Group 15. Our additional requirements are:
1. Store management
5. Stock recounts

The app has three main pages:
Commodity dispensing
Stock overview
Transaction history

Commodity dispensing lets you dispense multiple commodities to a recipient. The app automatically fills out the fields that it can, and the user fills out the form by using a searchable dropdown menu and setting an amount for each commodity. On submit the app is supposed to send the data to the API and updates the current period end balance and consumption for each of the commodities that were included. Due to bad time management and server downtime we were not able to create a successfull mutate function in dispensing. (HOWEVER: We made it work last second in STOCK RECOUNT). We believe we are very close, but we could not do it in time. Please take a look at the code in Registry or Recount to see our attempt. Due to being stuck at this point we also were not able to produce a Transaction successfully. Our Datastore is set up to support it, but it is not generated properly. 

The stock overview main page gives an overview over the current life-saving commodity stock balances for the current period. The user can then choose to register new stock that has been delivered or complete a stock recount. They were also supposed to be able to export to PDF. Stock registry lets the user easily register incoming stock by choosing commodities from a searchable dropdown menu and writing the amount that has been recieved. The stock recount page follows a similar pattern, and by filling out the form in the same way the end balance and consumption is adjusted on submit. Stock Recount submits data on submit to the api, however we did not have time to do this on stock registry.

Transaction history gives the user an overview over transactions that have been completed at the facility. The table shows who completed it, the recipient (when applicable), what type of transaction it is, and when.

The app is completed using the DHIS2 UI library most places where it is possible. We structured our app using main pages and components, however it is not perfect as we ran a little short on time where we wanted to rewrite some code to reduce redundancy in the different parts of the system, and create more generalised components. 
