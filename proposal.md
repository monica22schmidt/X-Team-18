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

Briefly describe a problem that your team would like to solve.  
Describe at a high level a program that could solve that problem.</br>

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

   The program would start off by asking if the user wants to create a new phonebook entry, search for an entry, or remove an    entry. 

   Create new phonebook entry - Prompts user for name, department, home, mobile, and work numbers

   Search for an entry -  Prompts for the name of the person 

   Remove an entry - Prompts for the name of the person

   After the first entry is picked you will be prompted again to pick 1 of the 3 options but an additional option will be        available and that is exit.


5. Types List: Break your solution idea down into units that you think can be implemented with a single class.
   Hashtable - Acts as the actual phone book. Has insert, lookup, and remove methods. Also deals with resizing and hashIndex      generating.
   
   Node - Holds the information for each phone book entry. Has instance variables for Name, Department, Home, Mobile, Work.      Has mutator and accessors to allow us to use the information stored inside. 


Name each interface or class and briefly describe its function or purpose.
   Main - Acts as the user interface. Asks for input and calls different methods to store and organize the input.
   HashTableADT - Outlines the different methods we will use in our hashtable implementation
   HashTable - Creates the functionality of the hashtable. Stores the information gathered from the phone book input. Acts        similar to a phone book.
   Node - hold the information for each entry into the phone book (name, department, home, cell, and work phones)

## Edit and Submit this file and any figures referenced by this document.

