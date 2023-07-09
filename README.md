# Invereter-design-using45nm_tech_using-Cadenece_virtuoso#
Invereter-design-using45nm_tech_using Cadenece_virtuoso_stepby_step

Start VMware
Start Cadence OS
Os will turn on 
like this 
![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/7ab89cc7-40a3-4a79-8174-64c28d01d1f2)

Turn on terminal and write *Virtuoso &* and press ENTER

![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/54391e9f-535b-4f2b-aa24-417a977ffee0)

CDS.log window will appear

![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/28cc56bd-6ba9-49be-96fc-6dc1bb858e46)

After that we need to make our own library
#Go to *New* and *Library*# 
![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/fcde9d7e-0372-4745-9ef1-a7dd8bb37035)

give the name of your Library in my case *inv_layout*
Put the Radio buttons to *attach to an existing library* 

and then select the GPDK technology file In my case, I took 90nm GPDK
Press Ok 
Then again go to CDS.Log
got to New and CellView
Type a name for your CellView in my case I had *inv_scheme_test_layout* and while creating Cellview  see if the library or the directory is right made by you or not! in my case, it is *inv_layout* 

![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/904643c8-fabc-41f6-94f3-68d3b776038b)

now the schematic will arrive put Nmos and Pmos instances set the pins and connect it via wire
![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/0bd97afd-1df8-496c-9929-2f43fc14eb8c)

Now coming to the Layout 
*1 Lunch Layout XL
and after layout, it will be like this 
![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/ee2ff778-4ed7-4f82-b02d-cc9a8a29e610)

After Creating the Layout 
we need to check the 
1. Checking Technology 
2. DRCs
3. ERCs
4. LVS
5. Extraction of RLC (over here I prefer only RC)




