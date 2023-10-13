# MAPS-AND-SETS-IN-JAVASCRIPT
This is a basic beginner friendly text file to learn about maps and sets in javascript

A)MAPS
//----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
                                                                                          MAPS

//creating or initializing new values to our map  OR CREATING A NEW MAP
let myMap = new Map ([ ["a1", "ajay"] , ["a2" , "aditya"] , ["a3" , "savan"] ]);
console.log(myMap);
//output-> Map(2) {'a1' => 'ajay', 'a2' => 'aditya'}

//-----------------------------------------------------------------------------------------

// .set method -> syntax -> mapName .set (" key name " , "value for this new key");

//as map allows to have duplicate values we can update the same value using .set method 
//or we can simply say that map takes in the updated values 
myMap.set("a2", "ajay");
console.log(myMap);
//output-> Map(2) {'a1' => 'ajay', 'a2' => 'ajay'}

//-----------------------------------------------------------------------------------------


//-----------------------------------------------------------------------------------------
// .get method -> syntax -> mapName .get ("keyName")
//fetching specific key values from our map 

console.log( myMap.get("a3") );
//output-> savan

//-----------------------------------------------------------------------------------------

//-----------------------------------------------------------------------------------------
//iterating over the map using for each loop
myMap.forEach( (key,value)=>{
console.log( key , value);
}) 
//output:- 
//ajay a1
//ajay a2
//savan a3
//-----------------------------------------------------------------------------------------

//deleting everything  using .delete method -> syntax -> mapName.clear();
myMap.clear();
//----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------





B)SETS
//--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- 

                                                                                          SETS

SET store only unique elements and even if we try to store a duplicate element it won't have any affect onto the set 
//and this duplicate element won't be shown in the set values 

//creating a new set syntax -> var set1 = new Set(); and to add elements in this empty set we use .add()method 

//moving an array to set 
// example :-
 let myArray = [1,2,3,4];
 let obj = new Set (myArray);
 console.log(obj);

//------------------------------------------------------------------------------------------------------------------------------ 
//checking size of our set syntax -> setName.size
//------------------------------------------------------------------------------------------------------------------------------

//adding elements to out set syntax -> setName.add(element to be added);
obj.add(5);
//now 5 is appended to our set and also the size became 4 from previously being 3 

//------------------------------------------------------------------------------------------------------------------------------
//checking if the element is present inside the set syntax -> setName.has(value to be checked inside the set)
//this .has() method of our set responds with true or false 
console.log( obj.has(5) );
//output -> true 


//------------------------------------------------------------------------------------------------------------------------------
//deleting a specific element from the set synatx -> setName.delete(element to be deleted);
obj.delete(5);
//this will delete 5 from the set 
//------------------------------------------------------------------------------------------------------------------------------


//------------------------------------------------------------------------------------------------------------------------------
//iterating over the set using for each loop syntax -> setName.forEach((element) =>{
// console.log(elements);
//})

obj.forEach((elements)=> {
  console.log(elements);
})

//output-> 1,2,3,4

//------------------------------------------------------------------------------------------------------------------------------
//deleting / clearing everything from the set syntax -> setName.clear();
                                                                                          
