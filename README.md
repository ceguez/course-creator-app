# CourceCreatorApp
Online Course App

Course Creator App is a Java Web App created based on the MVC design pattern concept; it has the following features:
-	Allows users to register or existing members to login.
*If a member with the same email exists, it displays message:  "Error: This user account already exists."
**Currently each member can only see their unique profile based on the courses each one creates etc. However, the idea is to eventually create special features for admin members and special features for regular members. The very basic base for this was already set up within the code by creating: public class Authorities implements GrantedAuthority.
-	To encrypt the passwords of all members.
-	To display a list of all the unique courses as soon as the member signs in or display no courses if there is none in her/his account.
-	To allow members to create a Course, a Section and a Lesson within each course respectively.
-	To allow the removal of a course.
-	Allow members to sign out.

After some research on how to simplify the developing process, I decided to use Spring Tool Suite as the IDE to create a microservice with the Spring Boot Framework. Spring allows to wire in (through auto-wiring) dependencies and this allows to make a very de-coupled program. Decoupled in the sense that there are not a lot of objects that depend on each other; by breaking up the dependencies a bit, when changing an object, it is not going to be fully affecting another object. 
The following main dependencies were used to create this app: 
-	Thymeleaf to integrate HTML5 at the view layer of the MVC.
-	JPA => Java Persistence to connect the data to the database MySQL.
-	JQuery => Ajax to include asynchronous features and make the web app dynamic. 
-	Spring Security Authentication and Authorization for login process.

Feature Expansion

The plan is to expand this project so that the app can:
-	Allow members to upload files: text, image, video and audio types.
-	Allow members to choose from different templates to structure the view of their profile.
-	Allow members to rate courses based on stars.
-	To create a general display in which all courses can be displayed and members can search for courses available to purchase or try for free. 
-	To make 2 type of Admin roles: 
	One that maintains the site

	One that is uploading courses material and can manage who gets access to their material by setting up to free or a price to access etc. 
