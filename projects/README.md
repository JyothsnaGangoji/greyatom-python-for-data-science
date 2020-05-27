### Project Overview

 This project is to use the skills learned in 'pythhon intermediate module' ,In which our mission is to help agency decipher a message that they received from there intel.  They have multiple text files that needed to be read and have certain operations performed to get the final message sent by the intel.
To complete this project succesfully concepts like String Operations, Conditional statement and loops, File I/O, Functions have been used.


### Learnings from the project

 After completing this project , I learnt how to solve logical problems using python.
I also learnt concepts like:
1. String Operations
2. Conditional statement and loops
3. File I/O
4. Functions 


### Approach taken to solve the problem

 **Step 1** :  First thing to do is to write a function that reads the contents of the files that we have.To do so we write a function "read_file()" ,that takes path as a parameter. Then open a file associated with the 'path' in read only mode using ( 'r' ) and store it in variable 'file', after this read the contents (first line) of the file and stored in a variable called 'sentence' and then return the 'sentence' using 'return' function , later on call a function "read_file()" with 'file_path' as input parameter and store the result in a variable called 'sample_message'.print 'sample_message'
**Step 2**:  In this , we have to make use of messages of two different files in which we have one number each and then apply a certain operatioin to extract the message.To do so we have to call the function read_file() written in the previous task for file_path_1 & file_path_2 and stored their message sentences in another variables message_1 and message_2 respectively and print them.Write a function fuse_msg() that takes message_a and message_b as parameters and then we implement integer(floor) division of message_b over message_a and store the result in 'quoitent' variable. call the function fuse_msg() with message_1 & message_2 and stored the result in 'secrete_msg_1' variable.Print secrete_msg_1.
**Step 3**: In this , we have to substitute the mesage of the file for  a secret message.To do so we call the function read_file() for file_path_3 and store its message in 'message_3' variable.And Write a function substitute_msg() that takes message_c as a parameter.Now create a new variable 'sub' and it stores a messasge based on if it is Red ,Green or Blue using if else statements.Call the function "substitute_msg()" with 'messsage_3' and store the result in 'secret_msg_2'.Print secret_msg_2
**Step 4**: In this ,We nake use of messages from two different files, and then compare two messages and take only those words that appear in the first message but not in second message ,now call the function read_file() for the file_path_4 & file_path_5 and stored their message sentences in 'message_4' & 'message_5' respectively, Now write a function compare_msg() that takes message_d & messasge_e as parameters, then break down the sentences in message_d & message_e  into words using split() function and then stored them in a_list & b_list respectively.And then stored all the words that are there in a_list but not in b_list in a new list 'c_list'.later on we combine the words of c_list back to the sentence using join() and store it in a variable 'final_msg' .Now call the function "compare_msg()"  with message_4 & message_5 and stored the result in a variable 'secrete_msg_3' .
**Step 5**: In this ,We have to extract only those words from the message in the file that are of even length.Call the function read_file() for file_path_6 and stored its value in variable message_6.Write a function extract_msg() that takes message_f as parameter, and then break down the sentence in message_f into words and store them in a_list.Now create a lambda function called even_word with the condition that will return true if length of  x (lambda function variable) is even.
Implements filter() function with function parameter as even_word and sequence parameter as a_list and stores the result in 'b_list' variable.Now combines the words of b_list back to the sentence and stores it in a variable called final_msg.Call the function "extract_msg()" with 'message_6' and store the result in a variable 'secret_msg_4'.
**Step 6**: we have succesfully deciphered all the message bits that we received.In this final step we will combine all the message bits into a single message and write in a file.The message parts that have been deciphered are providedd in the order that they have to be read,in a list called message _parts.combine the contents of message_parts into a single sentence and stored in a variable 'secret_msg'.Now call the function "write_file()" with 'secret_msg' and 'final_path'.print the 'secret_msg'.


### Challenges faced

 1. While getting the quoitent value i got an issue as floor division cannot be performed on strings, to overcome this issue i converted the string into int using int() function before performing the floor division. And to return the value as string i used str() function.
2. To select one sentence out of three according to the condition. to overcome this i used if elif and else conditions.
3. To get all the words that are there in a_list but not in b_list and store in c_list ,I used c_list=set(a_list) - set(b_list)



