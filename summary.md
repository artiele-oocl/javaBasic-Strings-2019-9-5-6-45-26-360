# Summary

Please answer the following 4 questions for each unit test:
1. What is the knowledge point of the test? Where is the official document to the knowledge point?
2. Why the test failed at first?
3. Why you corrected the test that way?
4. Do you have further questions on this knowledge point?

## StringTest
#### should_be_immutable
1. The knowledge point of this test is about familiarity with the difference between value comparison and object comparison.
This means that assigning a string to another string does not make them occupy the same address in memory.
https://www.baeldung.com/java-immutable-object
2. Test failed because output is not empty.
3. I corrected it that way because the purpose of this test is to check if the two objects are not the same object.
If two objects are not pointing to the same location in memory, then those two objects are different.
We can check this in three different way: using method equal(), method hashCode(), or operator double equal "==".
4. None.

#### all_modification_method_will_create_new_string
1. Same as above.
2. Same as above.
3. Same as above.
4. None.

#### will_create_new_string_when_concat
1. Same as above.
2. Same as above.
3. Same as above.
4. None.

#### should_taken_string_apart
1. This test is about familiarity of method replace(). 
2. Test failed because string is not null.
3. I corrected it that way because an already existing string utility method can be reused without unnecessarily creating 
a new method of my own.
4. None.

#### should_taken_string_apart_continued
1. This test is about familiarity of method substring(). 
2. Test failed because string is not null.
3. I corrected it that way because it is an already existing utility method for object String.
4. None.
5. What if the input arguments is out of range of the string?
- It reports an exception: java.lang.StringIndexOutOfBoundsException
6. What will happen if the the starting index is greater than the ending index?
- It reports an exception: java.lang.StringIndexOutOfBoundsException because it cannot find negative index.
7. What will happen if the input string is of null reference?
- It reports an exception: java.lang.NullPointerException because it is pointing to a null object.

#### should_break_string_into_words
1. Test is about splitting string object using split().
2. Test failed because it is not expecting null object.
3. I corrected it that way because it is an already existing utility method of string object.
4. None.

#### should_break_string_into_words_customized
1. Test is about splitting string object using split().
2. Test failed because it is not expecting null object.
3. I corrected it that way because it is an already existing utility method of string object.
4. None.

#### should_create_ascii_art
1. Test is about string manipulation given some constraints.
2. Test failed because it is not empty.
3. I corrected it that way because I know i have to loop over given height and width constraints.
4. None.

#### should_calculate_checksum_of_a_string
1. Test is about getting the checksum of a string by getting the associated ASCII counterpart of a character.
2. Test failed because it is not the total checksum.
3. I corrected it that way because I know i had to loop over the string to get associated integer value of each character.
4. None.

#### should_convert_unicode_escape
1. Test is about converting unicode.
https://www.tutorialspoint.com/convert-string-to-utf-8-bytes-in-java
2. Test failed because it is not null.
3. I corrected it that way because it automatically converts unicode to characters.
4. None.

#### should_reverse_a_string
1. Test is about reversing a string.
https://www.tutorialspoint.com/java/lang/stringbuilder_reverse.htm
2. Test failed because it is not null.
3. I corrected it that way because an already existing util from StringBuilder is readily available. No need to reinvent the wheel.
4. None.

#### should_compare_string_with_different_cases
1. Test is about comparing strings of different cases.
https://docs.oracle.com/javase/8/docs/api/java/lang/String.html#contentEquals-java.lang.CharSequence-
2. Test failed because it is not empty.
3. I corrected it that way because I am comparing a sequence of character.
I was also able to realize the difference between String.equals() and String.contentEquals():
"The big difference is that equals() will only work with another String, while contentEquals() would work on any CharacterSequence (like StringBuilder)."
This means that I can use contentEquals() since String is an implementation of CharacterSequence.
4. None.

#### should_format_string
1. Test is about string format conversions.
2. Test failed because it is not empty.
3. I corrected it that way based on below list of string format conversion.
4. None.
