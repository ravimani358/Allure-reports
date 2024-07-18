# Allure-reports

https://github.com/allure-framework/allure2/releases

this is the link we need to refere in allure reports and easy to assess

path C:\Users\ravisankar.n\Eclipse Code\allure-2.30.0\bin

I. Enviroment variable

window button -> Enviroment variable -> path -> edit -> past (file location of extracted allure report locations) -> New Okay


II. Syatem variable

Path -> edit -> new -> past (file location of extracted allure report locations)

1. move to eclipse -> your project package -> POM .xml file -> check testng dependency is there are not

2. and add another one "properties" -> maven compiler -> should be past in between "Version" and "dependencies"

3. and dependencies for allure dependencies

4. and need build plugin 
	-> need to wright build plugin
	-> after dependencies ( open the build tag)
	-> <build>
	<plugins>
	past the plugin ***here***
	</plugins>
	-> </build>
	
5. after that we need apochi maven plugin (surefire plugin)
	-> apochi maven plugin
	in this we need <configuration> files point to testng.xml file
	
after that need to add the @Step in all @Test tag

open the terminal and search 

1. allure serve
2. navigate to root progect folder in file manager and launch cmd
3. allure serve ./allure-results


navigate to the allure path............

C:\Users\ravisankar.n\OneDrive - Everi Payments, Inc\Desktop\Eclipse Code\Everi_Concierge\allure-results

open the commend prompt 
-> allure serve

