### Importing Fundraisers
#####Fundraiser Import Definitions & Instructions

* indicates a required field

For bulk importing of fundraisers prior to importing monthly donations or launch prepare a csv with the following headers and values. A sample csv and template are provided as part of our import downloads.

#####Name*
This is the name as it appears on the fundraiser. Ex: “Water for Malawi”

#####Fund ID
This is the preferred reference id used by your organization to track this fundraiser as it relates to monthly online donations or internal tracking. If you do not have a preferred reference id one will be generated.

#####URL
The URL is the vanity name given to the web address. This makes the fundraiser easy for donors to find. Ex: “water-malawi” would create the url http://purecharity.com/water-malawi. If no URL is provided one will be generated from the fundraiser name.

#####Founder Reference ID
If you want to add an existing Pure Charity user as a founder for any of the fundraiser their reference ID can be added here. If no ID is provided we will assign the organization or admins as the founder.

#####Anonymous Funding
This is a value of TRUE or FALSE. If you would like funding goals to be private add the value TRUE, if you would like funding goals to be public add the value FALSE.

#####Anonymous Recurring Funding
This is a value of TRUE or FALSE. If you would like monthly funding goals to be private add the value TRUE, if you would like monthly funding goals to be public add the value FALSE.

#####Personal ID
The personal ID is an optional field provided to the organization for tracking purposes. This field will be displayed on the downloaded transactions csv.

#####Campaign ID
The personal ID is an optional field provided to the organization for tracking purposes. This field will be displayed on the downloaded transactions csv. Contact the development team with questions about campaign IDs that are used to filter displayed results in the WordPress plugins.

#####About*
This is a short description about the Fundraiser. Maximum length: 255 characters.

#####End date
End date for the fundraiser provided in the format mm/dd/yyyy. Ex: ’01/25/2014′ To set the fundraiser as an unlimited fundraiser you can enter the date ’12/31/2099′

#####Funding Goal*
The funding goal is an integer value and can be set to any amount with at least a 1 dollar minimum. A fundraiser can be set as unlimited by entering a value of 999999. Round the funding goal to the nearest dollar.

#####Recurring Funding Goal
The monthly funding goal is an integer value and can be set to any amount with at least a 1 dollar minimum. A fundraiser can be set as unlimited by entering a value of 999999. Round the monthly funding goal to the nearest dollar.

#####Location
The location is the city and state or province where the fundraiser will provide support. Ex: ‘Dallas, TX’

#####Location Private
The location private value is a boolean and accepts a TRUE or FALSE setting. To keep the location of the fundraiser private set the value to TRUE. To keep the location of the fundraiser public set the value to FALSE. If no value is entered the default will be FALSE.