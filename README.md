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

#Technology Checking#
This step is to be done because Engineer need to assure that technology Lib file is attached to the design files.
Got to *Assura* Then *Technology* then give the directory 
/home/buet/cadence/gpdk090_v4.6/assura_tech.lib

Press Ok 

#DRC#
Got to *Assura* the *Run DRC*
![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/b618c743-1c64-422f-8e49-103ad504e772)

Mention the GPDK lib and Layout Directory as mentioned in the Image

Press OK 

![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/d4886e89-e20f-4aa3-9d3f-85782d6ea621)

Then this will appear Press ok or yes

![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/18269a92-e5c4-420a-ac8a-a7d5338c454d)

then this will arrive
![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/6fe8dbdd-1305-4a0b-8dca-66801b60c951)
That means No DRC Violations.
We are ok to go further.

#Checking LVS#

Got to *Assura* then *LVS*

then follow my screenshot

![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/bd30b0ce-cf08-4211-bc7b-078f71f84abd)

after pressing ok this will arrive 
![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/f2cb060d-c272-4d13-be19-aa8918430e01)

![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/9ddaed55-db0d-4c60-8cdd-c3b52c556dd8)

Then press yes

![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/29968591-51c3-4dfb-8ffe-18038725cf31)

Wish u good Luck!

Layout Vs Schematic is all good.

#Run RCX Or the Ultimate RC extraction of our Layout#
Got to *Assura* then go to  *RUN RCX*
![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/9d243748-349a-4167-b5c2-e3a38b2758dc)

![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/9c02659e-9b1a-477a-a2a0-823f77d364fd)

then 
press OK 
![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/904c0431-2a4e-4b45-8546-bdf7adb518fe)

Then 
go to CDS.LOg window to view

File - Open_ your library (in my case 'inv_layout')_
select the the layout file and change the view mode to *av Extracted*

![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/96f41cf7-4dc7-4d63-95ed-80dfbe12e107)

Press OK 

![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/9530698e-9aef-4cae-9574-45099c7f1aa8)

It will arrive 


Press Shif+F and view the RC VAlues 

![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/46170fc5-c0d4-4f2f-9527-e5b7878f477e)

![image](https://github.com/Caprio2000/Invereter-design-using45nm_tech_using-Cadenece_virtuoso/assets/71349997/c4108fce-3e95-4ea1-a6a8-994344809311)


Thank you to 
#Dr Madhumita Das Sarkar (MAKAUT)
#Dr Mihir Kumar Mahata (MAKAUT)
#Dr Ria Bose (MAKAUT)
#Mr. Rajesh Yadav (Samsung) 
#Team VLSI 
#VLSI For ALL
#Mr.Samanway Ghosh (MAKAUT)
#Mr. Arpan Konar







