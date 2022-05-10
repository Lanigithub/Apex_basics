### Apex_basics
####// In this Apex class we will learn how to declare a list and apply the basic list methods: add(), addAll() to add elements to an existing list,
####//  contains() method  and equal() method for a boolean statement : true or false when compare two lists or checking existance of an element
####//  clone() method to copy a list and clear() to delete all the elements of a list

public class Apex_list_and_Method {                //declarr a class Apex_list_and_Method
    public void listMethod(){                    //declare a method listMethod
        List<String> nameList= new List<String>{'Annie','Vince','Brian'};    //Declare nameList with type String
        List<Integer> ageList =new List<Integer>{35,18,15};             //Declear ageList with type Integer
            //Declare two more lists
        List<String> nameList2= new List<String>();   
        List<Integer> ageList2 =new List<Integer>();
             //declare a set
        Set<Integer> ageSet= new Set<Integer>{21,25};
            //Declare a boolean boo and res
          Boolean boo, res;
          // use contains() method to find out if an element exist in a list
          boo=ageList.contains(7);
          // use equals() method to find out if two lists are equal
          res=ageList.equals(ageList2);
        
            
        nameList.add('Eddie');  // using add() method to add new elements to the list
        nameList2.add('John');
        nameList2.addAll(nameList); //use addAll() method to all all elements from first list to 2nd list
        
        ageList.add(10);
        ageList2.add(5);
        ageList2.addAll(ageList);
        ageList2.addAll(ageSet);     //using addAll method() add elements from a set to list 2
         
        
        
        
        
        // System.debug('nameList: '+nameList);                    // output nameList  and call on the debug execute Annonymous window
          //System.debug('ageList: '+ageList);  
          // Checking boolean:
         System.debug('7 in ageList =>'+boo);    
          System.debug('ageList eqial to ageList2 =>'+res); 
             
            System.debug('nameList2: '+nameList2);                    // output nameList  and call on the debug execute Annonymous window
            System.debug('ageList2: '+ageList2);                      // Call to execute: Apex_list_and_Method L=new Apex_list_and_Method();  L.listMethod()
        
        //Using list.clone() method to cleara list
        List<Integer> ageList3= new List<Integer>();
        ageList3=ageList2.clone();
        //System.debug('ageList3: '+ageList3);
        
        //Use clear() to clear a list
        ageList3.clear();
        System.debug('ageList3: '+ageList3);
        
        
                
        
    }

}
