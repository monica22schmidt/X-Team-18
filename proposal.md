# Employee Phone Directory (X-Team 18 Project Proposal) 

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

### Problem Context  
**A young company of 5,000 people is in need of a search engine that acts as a directory of all employees and their contact information (name, department, phone numbers). Company management believes this will facilitate quick and direct communication between the employees. The company has most employees' contact information, but these entries are stored in an outdated Excel spreadsheet, which is not the most efficient and accessible platform for employees to search for each other. In addition, it wouldn't hurt for employees to re-input their information to reflect the most current and accurate details. The team of software engineers in the company hope to design a new system that stores all employees' relevant information.**</br>

### Main class  
**The main class will construct an instance of hashtable and also create a mode of retrieving data such as an instance of Scanner to read from System.in. Main will also act as a potential interface, prompting the user to enter their information. If the available data is raw in the form of a spreadsheet, Main calls methods to process the file and organize the data into their respective fields. Main should ultimately output the requested information for a particular name.** </br>

### Custom Data Structure 
**The custom data structure will be based on the implementation of a hashtable. The idea is to use hashing as a mechanism for distributing the entries (key/value pairs) across an array of buckets. Given a key, the hash function algorithm computes an index that suggests where the entry can be found. In this context, given that the keys are names of String type, the hash function will first convert every character in a name to their respective ASCII values, and then the (characters summed on base 256 such that "cab" can be represented by 99\*256^2 + 97\*256^1 + 98\*256^0) % (table size) will map to the index in the hashtable array that stores all information (value) for the name (key). Information includes name, department, and several phone numbers. Separate chaining will be implemented to account for collisions where multiple keys map to the same index.**

### Unit Tests 
**Unit tests for the program consist of JUnit tests that assess the functionality of the methods required for successful implementation of hashTable (insert, remove, lookup, size, resize, hashindex calculation, etc.). Tests empty and parameterized constuctors as well. There will also be test for checking if a hashtable is empty or not after certain operations. When program does not run as expected, programmer will be able to see which tests failed/passed.**</br>

## Questions to answer for Exercise #2

1. Name: Give your project proposal a name (and edit the top line of this file)</br></br>
   **Employee Phone Directory** 



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
   **The input of our program may come in two forms: direct input by user in Main or comma-delimited input formatted by online form.**</br>
   
   **/\* EXAMPLE INPUT FORMAT 1 (direct input to program by user)\*/**</br>
   **Please enter your name (First Last): John Doe**</br>
   **Please enter the department you belong to: UX/UI**</br>
   **For the following, please enter "N/A" if not applicable.** </br>
   **Please enter your home number: N/A**</br>
   **Please enter your mobile number: 9192403654**</br>
   **Please enter your work number: 6084074008**</br>
   
   **/\* EXAMPLE INPUT FORMAT 2 (comma-delimited input)\*/**</br>
   **John,Doe,UX/UI,N/A,919240354,6084074008** \<input format for single employee entry> </br>

4. User Interface: Describe a user interface for your program.  Use text menus or a simple graphic user interface.</br>

   **At this point, our team will simulate a simple user interface in Main to exemplify the foundational blueprint of the phone book  system. Eventually, the team will make visual and interactive enhancements to the system by implementing an online graphic user interface similar to a survey form.**
   
   **/\* EXAMPLE USER INTERFACE IN MAIN\*/**</br>
   **Please enter your name (First Last): \<*firstName lastName*>**</br>
   **Please enter the department you belong to: \<*department*>**</br>
   **For the following, please enter "N/A" if not applicable.** </br>
   **Please enter your home number: \<*home number*>**</br>
   **Please enter your mobile number: \<*mobile number*>**</br>
   **Please enter your work number: \<*work number*>**</br> 
   
    **/\* EXAMPLE USER INTERFACE USING GUI\*/**</br>
    *Please refer to Fig 1, 2, and 3 attached to submission.*</br>
    
5. Types List: Break your solution idea down into units that you think can be implemented with a single class.</br>
  * **HashTable**: Acts as the phone book that stores numbers and other information corresponding with employee names. Implements insert (insert employee entry), lookup (search for employee entry and return its index in the table), remove (delete employee entry), contains (return boolean of whether or not a piece of information exists in hashtable), size (number of employee entries in table) methods. Also resizes array when table is full and calculates hashIndex.</br>
  * **Entry (nested class within HashTable)**: Holds the information for each employee entry. Has name (String type) as key and other information (department, phone numbers in String type) as value. Has mutator and accessors to allow manipulation and retrieval of the data. </br>


Name each interface or class and briefly describe its function or purpose.</br>
  * **Main**: Acts as the user interface. Asks for input and calls different methods to store and organize the input.</br>
  * **HashTableADT (interface)**: Outlines the different methods we will use in our hashtable implementation</br>
  * **HashTable**: Creates the functionality of the hashtable. Stores the information gathered from the phone book input. Acts similar to a phone book.</br>
  * **Entry**: hold the information for each entry into the phone book (name, department, phone numbers)</br>

## Edit and Submit this file and any figures referenced by this document.

