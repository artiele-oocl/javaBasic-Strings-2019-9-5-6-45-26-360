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
1. The knowledge point of this test is about familiarity with the difference between value comparison and object comparison.
This means that assigning a string to another string does not make them occupy the same address in memory.
https://www.baeldung.com/java-immutable-object
2. Test failed because output is not empty.
3. I corrected it that way because the purpose of this test is to check if the two objects are not the same object.
If two objects are not pointing to the same location in memory, then those two objects are different.
We can check this in three different way: using method equal(), method hashCode(), or operator double equal "==".
4. None.