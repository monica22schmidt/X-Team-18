# Phone Book (X-Team 18 Project Proposal) 

See https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#code for tips on using *Markdown* tags to format __.md__ files

## Goal

Work as a team to create a project proposal for your X-team to complete together.
The project does not have to be extremely difficult,
but there must be work to do for each member of your team.
You may reference figures using "See figure 1".  
Be sure to submit corresponding image files, i.e. figure1.png (or figure1.jpg) for each figure.

## Grading: To earn full credit, your team's proposal must include:

* (md) documentation: [this file] describing purpose and use of your program

* Description of a program that has:

  ** a main Java program class in a file named Main.java
  
  ** a custom data structure designed and built by your team
  
  ** comprehensive testing of individual units
  
 Caution: You are not being asked to implement this program, at least not yet. 
 We just want your group to make a proposal or pitch for your program.
 
 Tip: Your custom data structure can be composed of or extensions of data structures that you have learned and used in previous programming assignments.  We're looking for decisions about how to build a high-level data structure that will likely have lower-level components.

## Problem Description

The company in question has all of the contact info from their employees, being their name, number, and address. All of this information is in an excel spreadsheet. However, this is not a particularly efficient way of storing that information. Just last week, there was an emergency, and because of the inefficient manner of the excel spreadsheet, valuable time was wasted. We need to find a more efficient way to store the contact info.</br>

### Problem Context  
**A company of 5,000 people is in need of a search engine that acts as a directory of all employees and their contact information. The best way for quick and direct communication between the employees is by phone. The team of software engineers in the company hope to design a system that stores all the phone numbers (home, mobile, work, etc.) of all the employees.**</br>

### Main class  
**The main class will construct an instance of hashtable and also create a mode of retrieving data such as an instance of Scanner to read from System.in. Main will also act as a potential interface, prompting the user to enter their information. Main should ultimately output the requested information for a particular name.** </br>

### Custom Data Structure 
**The custom data structure will be based on the implementation of a hashtable. The idea is to use hashing as a mechanism for distributing the entries (key/value pairs) across an array of buckets. Given a key, the hash function algorithm computes an index that suggests where the entry can be found. In this context, given that the keys are names of String type, the hash function will first convert every character in a name to their respective ASCII values, and then the (sum of the first three and last three characters) % (table size) will map to the index in the hashtable array that stores all information (value) for the name (key). Information includes name, department, and several phone numbers. Separate chaining will be implemented to account for collisions where multiple keys map to the same index.**

### Unit Tests 
**Tests the functionality of the methods insert, remove, lookup, resize, and hashindex calculation. Also tests empty and parameterized constuctors. There will also be test for checking if a hashtable is empty or not.**</br>

## Questions to answer for Exercise #2

1. Name: Give your project proposal a name (and edit the top line of this file)</br></br>
   **Phone Book** 



2. Output: Describe the output your program will produce.  Include an example format of the output produced.</br></br>
   **The output of our program includes a listing of basic information (name, department, phone numbers) for a name the program's user input.**
   
   **/\* EXAMPLE OUTPUT FORMAT \*/**</br>
   **Name: \<*name*>**</br>
   **Department: \<*department*>**</br>
   **Phone Number:**</br>
   **Home - \<*home number*>**</br>
   **Mobile - \<*mobile number*>**</br>
   **Work - \<*work number*>"**</br>


3. Input: Describe the data that is needed to solve your problem. Include an example format of the input data.</br></br>
   **/\* EXAMPLE INPUT FORMAT \*/**</br>
   **Please enter your name (First Last): \<*firstName lastName*>**</br>
   **Please enter the department you belong to: \<*department*>**</br>
   **For the following, please enter "N/A" if not applicable.** </br>
   **Please enter your home number: \<*home number*>**</br>
   **Please enter your mobile number: \<*mobile number*>**</br>
   **Please enter your work number: \<*work number*>**</br>  


4. User Interface: Describe a user interface for your program.  Use text menus or a simple graphic user interface.

   **At this point, our team will simulate a simple user interface in Main to exemplify the foundational blueprint of the phone book  system. Eventually, the team will make visual and interactive enhancements to the system by implementing an online user interface similar to a survey form.**

5. Types List: Break your solution idea down into units that you think can be implemented with a single class.
Hashtable - Acts as the actual phone book. Has insert, lookup, and remove methods. Also deals with resizing and hashIndex generating.
Node - Holds the information for each phone book entry. Has instance variables for Name, Department, Home, Mobile, Work. Has mutator and accessors to allow us to use the information stored inside. 


Name each interface or class and briefly describe its function or purpose.
Main - Acts as the user interface. Asks for input and calls different methods to store and organize the input.
HashTableADT - Outlines the different methods we will use in our hashtable implementation
HashTable - Creates the functionality of the hashtable. Stores the information gathered from the phone book input. Acts similar to a phone book.
Node - hold the information for each entry into the phone book (name, department, home, cell, and work phones)

## Edit and Submit this file and any figures referenced by this document.

