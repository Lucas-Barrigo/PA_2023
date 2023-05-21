# Library JsonObject
Convert classes to json and manipulate JSONObject's.

# How Execute the project
    Install IntellIJ and open the porject, dependecies will install automatically and then run the main method's of the classes in the project.
# Functionalities
  ## Add properties
    Add a new property to the Json
        addProperty("uc", JSONString("PA"))
  ## Remove properties
    Remove a property from the Json
        val el: Pair<String, JSONValue> = jsonObject.get()[0]
        jsonObject.remove(el)
  ## Update properties
    Update the value of a property
        update("uc", "DB")
  ## Automatically identifies the type of the porperty
     Automatic detect the type os the property 
        val json = JSONObject().mapObject(student)
  ## Search for properties
    Search and return the Objects with the value that was searched.
        search(propertyName, propertyValue)
  ## Map a class XPTO to JSONObject
        Will map a class to Json  
            mapObject(o: Any): JSONValue
# Explicação das anotações
  ## Exclude
    Will exclude the object below
  ## ToString
    Will force the typf of the object below to String
  ## ChangeName
    Will rename the object below
  
# Tests
  ## testAddPropertyToJSONObject
    Will take inicial size of the JsonObject and aply a remove to verify if the size of the JsonObject decrease 1.
  ## testRemovePropertyFromJSONObject
    Will take inicial size of the JsonObject and aply a add to verify if the size of the JsonObject encrease 1.
  ## testUpdatePropertyInJSONObject
    Will add a value PA to the UC and execute a update to DB, then will verify if the UC has been updated for DB.
  ## testValidateJSONStructure
    Will validade the Json structure
# diagrama de classes
![image](https://github.com/Lucas-Barrigo/PA_2023/assets/81224139/d55d5d7c-5727-436f-b945-52dbbfbf19ab)


