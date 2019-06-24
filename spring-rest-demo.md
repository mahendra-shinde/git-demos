## Preparing Eclipse for Spring Framework

1. Start eclipse with NEW workspace
2. Goto "Help" Menu > Eclipse Marketplace > Search for 
        " Spring "
3. Install Spring Tools 3 or STS 
4. Accept the EULA and Client certificates 
5. You may have to restart eclipse after plugins are installed.


## Create new Spring Starter Project (Based on Spring Boot)

1. File Menu > New > Spring Starter Project 
    or
   File Menu > New > Other > Spring Starter Project 

2. Enter project details:
    
        Name project:   demo
        Language:       Java
        Version:        8
        Packaging:      JAR
    
    Click Finish

3.  Wait for few minutes for maven to download all dependencies.
   
    Open "Markers" View to list all errors and warning
    
    If there is ANY error for any JAR file, 
    
    Open "C:\Users\{NAME}\.m2\repository in file explorer.
    
    Locate the folder which gave you maven error and delete it!

    Go back to eclipse, Right click on project > Maven > Update Project

4.  Create a model class "Product" in package "com.example.demo.models"
    NOTE: A Wrong package means your REST service wont work!!

    Properties:  id, name, price and description
    Create Getters/Setters and Constructors

    ```java
    @XmlRootElement //Mark this class for XML conversion
    public class Product {

	private int productId;
	private String name;
	private double price;
	private String description;
    //Getters, Setters and Constructors...
    ```
5.  Create Controller class "ProductController" 
    in package "com.example.demo.controller"

    ```Java
    @RestController
    public class ProductController {

	@RequestMapping(value="/find",method = RequestMethod.GET,produces= {"application/xml","application/json"})
	public Product find(@RequestParam int id) {
		    return new Product(id, "Dummy Product",123.23,"A product you cant afford!");
	    }
    }
    ```

6.  Goto "DemoApplication.java" and Righ click -> Run As -> Java Application

7.  Open browser and visit page:

        http://localhost:3000/find?id=101
