1. logger.log writes error messages, warning messages, and info messages to a file so that they can persist and be analyzed later.
2. The line comes from ConditionEvaluator when a condition that was supposed to be disabled was not 
3. Assertions.assertsThrows asserts that the tested method throws an exception
4. 
	1. serialVersionUID is an identifier that is used to serialize or deserialize the object. we need this so that the object can be stored/written.
	2. Constructors cannot be overwritten, but we need to implement these constructors so that the exception will have the correct message
	3. We do not need to override the other exception methods because it has all the methods provided by Throwable available to it
5. Static blocks are run when the class gets loaded, so it sets up the LogManager when the app is started.
6. README.md is a Markdown file that BitBucket displays on the repository's source page.
7. The test fails because a NullPointerException is thrown rather than a TimerException. The variable timeNow is initialized as null, but when timeToWait is a negative value timeNow is never updated. So when System.currentTimeMillis() - timeNow is executed it throws a NullPointerException
8. The time for calling time me is not matching the values that it should be. If the time to wait is negative, a TimerException is thrown. If an InterruptedException is caught then the logger logs a severe error. Regardless of which exceptions are thrown, the code inside the finally block is excecuted. 
9.
10.
11. TimerException is a RuntimeException. NullPointerException is also a RuntimeException