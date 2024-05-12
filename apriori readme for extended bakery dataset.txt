The XXXX-out1.csv file format is: receipt# followed by item #'s that are on that receipt. (sparse vector representation) 
The XXXX-out2.csv file format is: receipt# followed by 0's and 1's indicating if an item was on a given receipt. (full binary vector representation). 
The XXXXi.csv file format is: receipt# followed by item number and quantity ( CSV version of the Items tables ) 


-------------------
Based on what is discussed in class:

--------------------------
for XXXXi.csv 
Following steps may be followed :
###Import the dataset
###Apply column names

#if you are Applying column names as
"Receipt_Number","Food","Quantity"

#then for preprocessing you can Create a dataframe containing each item and map it to its corresponding id like this
for id 1,2,3,4,5
food names : "milk","sugar","chocolate","apples","curd"

-------------------
or
------------------

#if you are applying column names as
"Receipt_Number","Quantity","Food"

#then for preprocessing you can Create a dataframe containing each item and map it to its corresponding id like this
for id 0 to 49
food names : "Chocolate Cake","Lemon Cake","Casino Cake","Opera Cake", "Strawberry Cake", "Truffle Cake", "Chocolate Eclair", "Coffee Eclair", "Vanilla Eclair", "Napolean Cake", "Almond Tart", "Apple Pie", "Apple Tart","Apricot Tart", "Berry Tart", "Blackberry Tart", "Blueberry Tart", "Chocolate Tart", "Cherry Tart", "Lemon Tart", "Pecan Tart", "Ganache Cookie", "Gongolais Cookie", "Raspberry Cookie", "Lemon Cookie", "Chocolate Meringue", "Vanilla Meringue", "Marzipan Cookie", "Tuile Cookie", "Walnut Cookie", "Almond Croissant", "Apple Croissant", "Apricot Croissant", "Cheese Croissant", "Chocolate Croissant", "Apricot Danish", "Apple Danish", "Almond Twist", "Almond Bear_Claw", "Blueberry Danish", "Lemon Lemonade", "Raspberry Lemonade", "Orange Juice", "Green Tea", "Bottled Water", "Hot Coffee", "Chocolate Coffee", "Vanilla Frappucino", "Cherry Soda", "Single Espresso"



##After Mapping IDs to its text representation, review the dataset using describe, head etc.
###Convert it into basket format to run in apriori
###check the rules for specified Support and Confidence
###try plots



