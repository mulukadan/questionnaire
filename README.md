# questionnaire
Mock Interview Warm Up

###### What is an annotation? What does it look like? What does it do?
  Java Annotations allow us to add metadata information into our source code, although they are not a part of the program 
itself. Annotations were added to the java from JDK 5. Annotation has no direct effect on the operation of the code they 
annotate (i.e. it does not affect the execution of the program). An annotation always starts with the symbol @ followed by the 
annotation name. The symbol @ indicates to the compiler that this is an annotation. There are three built-in annotations 
available in Java (@Deprecated, @Override & @SuppressWarnings) that can be used for giving certain instructions to the compiler. For example the @override annotation is used for instructing compiler that the annotated method is overriding the 
method. Annotations can provide compile-time instructions to the compiler that can be further used by sofware build tools for 
generating code, XML files etc. We can define annotations to be available at runtime which we can access using java reflection 
and can be used to give instructions to the program at runtime.

###### What is the naming convention for JUnit test methods?
  Following are 7 popular unit tests naming conventions that are found to be used by majority of developers and compiled from
above pages:
- MethodName_StateUnderTest_ExpectedBehavior: There are arguments against this strategy that if method names change as part of
  code refactoring than test name like this should also change or it becomes difficult to comprehend at a later stage. 
- MethodName_ExpectedBehavior_StateUnderTest: Slightly tweeked from above, but a section of developers also recommend using 
  this naming technique. This technique also has disadvantage that if method names get changed, it becomes difficult to 
  comprehend at a later stage. 
- test[Feature being tested]: This one makes it easy to read the test as the feature to be tested is written as part of test 
  name. Although, there are arguments that the “test” prefix is redundant. However, some sections of developer love to use 
  this technique. 
- Feature to be tested: Many suggests that it is better to simply write the feature to be tested because one is anyway using 
  annotations to identify method as test methods. It is also recommended for the reason that it makes unit tests as alternate
  form of documentation and avoid code smells. 
- Should_ExpectedBehavior_When_StateUnderTest: This technique is also used by many as it makes it easy to read the tests. 
- When_StateUnderTest_Expect_ExpectedBehavior: 
- Given_Preconditions_When_StateUnderTest_Then_ExpectedBehavior: This approach is based on naming convention developed as part 
  of Behavior-Driven Development (BDD). The idea is to break down the tests into three part such that one could come up with 
  preconditions, state under test and expected behavior to be written in above format. 
My personal favorite is naming unit tests based on the writing features of the class under test. It helps me to make sure that a
class follows single responsibility. It also aids a great deal in code refactoring.    

###### When we compile our code with Gradle, where does Gradle place the compiled .class files?
  gradle build task compiles, tests, and assembles the code into a JAR file. You can run it like this: gradle build.
  
###### Why is Behavior-Driven Development beneficial?
- Strong collaboration. With BDD, all the involved parties have a strong understanding of the project and they can all have a
  role in the communication and actually have constructive discussions. BDD increases and improves collaboration. It enables 
  everyone involved in the project to easily engage in the product development cycle. And by using plain language, all are 
  able to write behavior scenarios.
- High visibility. By using a language understood by all, everyone gets a strong visibility into the project’s progression.The
  software design follows business value. In fact, BDD puts a great importance to the Business value & needs. By setting 
  priorities with the client, based on the value it provides, developers are able to provide better result because they have a
  strong understanding of how the client thinks. By focusing on the value, no useless features are built.
- The ubiquitous language. As mentioned earlier, the ubiquitous language is understandable by all the members of the team, 
  which reduces misconceptions and misunderstanding and makes it easier for new members to join the working process.
- Software development meets user need. By focusing on the business’ needs, you get satisfied users, and that implies a happy
  business of course. Actually with BDD, as its name says it, you focus on the behavior, which has a stronger impact than the
  implementation itself. 
- More confidence from the developer’s side. Teams using BDD are in general much more confident that they won’t break code, 
  and have better predictability when it comes to their work.
- Lower costs. By improving the quality of the code, you are basically reducing costs of maintenance and minimising the 
  project’s risks.

###### What is a stacktrace? What does it do for us?
  A stack trace is a report that provides information about program subroutines. It is commonly used for certain kinds of 
debugging, where a stack trace can help software engineers figure out where a problem lies or how various subroutines work 
together during execution. A stack trace is also known as a stack traceback or a stack backtrace. A stack trace works on the 
"call stack," which is a data structure that provides information about the current subroutine of the program being debugged.
The call stack is also known simply as the "stack" or the execution stack, runtime stack or machine stack. The stack also 
provides information about each subroutine’s priorities and how subroutines should be executed.
  Stack tracing looks at these subroutines through the stack to analyze what each subroutine contains and how it is run. 
Software experts define stack trace as a list of the subroutine calls that an application performs during execution. Stack 
tracing is important for complex codes because it helps software engineers and other developers find bugs in the program. 
Because of the nature of modern code syntax, and the complexity of the average project, looking for bugs can be very difficult.
Software companies use many different kinds of proactive testing to isolate parts of the software environment to find bugs or
glitches. A stack trace is one of many tools that can be useful in comprehensive testing.
