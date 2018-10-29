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

For our employees, we have a collection of names, addresses, and phone numbers. They are all currently in an excel spread sheet, and we would like a more efficient way of accessing the contact information. It is simlpy just not efficient enough with the current way we store them. Just last week, we had an incident where an employee needed an ambulance, and we coulnd't find the proper phone number. Precious time was wasted.</br>

# Problem Context  
**A company of 5,000 people is in need of a search engine that acts as a directory of all employees and their contact information. The best way for quick and direct communication between the employees is by phone. The team of software engineers in the company hope to design a system that stores all the phone numbers (home, mobile, work, etc.) of all the employees.**

# Main class  

# Custom Data Structure  

# Unit Tests 


## Questions to answer for Exercise #2

1. Name: Give your project proposal a name (and edit the top line of this file)</br></br>
   **Phone Book** 



2. Output: Describe the output your program will produce.  Include and example format of the output produced.</br></br>
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
  **Text based menu options. Program starts by asking the user if they want to insert, remove, or lookup an entry**</br>
  **Insert - User is prompted for a name, department, home, work, mobile.**</br>
  **Remove - Prompted for a name**</br>
  **Lookup - Prompted for a name**</br>
  **After one of the three options are executed the user is prompted to pick from the previous three choices or to exit**</br>

5. Types List: Break your solution idea down into units that you think can be implemented with a single class.
  **Hashtable - Acts as the actual phone book. Has insert, lookup, and remove methods. Also deals with resizing and hashIndex generating**</br>
  **Node - Holds the information for each phone book entry. Has instance variables for Name, Department, Home, Mobile, Work. Has mutator and accessors to allow us to use the information stored inside. **</br>


Name each interface or class and briefly describe its function or purpose.</br>
  **Main - Acts as the user interface. Asks for input and calls different methods to store and organize the input.**</br>
  **HashTableADT - Outlines the different methods we will use in our hashtable implementation**</br>
  **HashTable - Creates the functionality of the hashtable. Stores the information gathered from the phone book input. Acts similar to a phone book.**</br>
  **Node - hold the information for each entry into the phone book (name, department, home, cell, and work phones)**</br>

## Edit and Submit this file and any figures referenced by this document.

