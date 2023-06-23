#sdk
[TestMethod]
public void IsPalindrome_ForPalindromeString_ReturnsTrue()
{
    // In the Arrange phase, we create and set up a system under test.
    // A system under test could be a method, a single object, or a graph of connected objects.
    // It is OK to have an empty Arrange phase, for example if we are testing a static method -
    // in this case SUT already exists in a static form and we don't have to initialize anything explicitly.
    PalindromeDetector detector = new PalindromeDetector(); 

    // The Act phase is where we poke the system under test, usually by invoking a method.
    // If this method returns something back to us, we want to collect the result to ensure it was correct.
    // Or, if method doesn't return anything, we want to check whether it produced the expected side effects.
    bool isPalindrome = detector.IsPalindrome("kayak");

    // The Assert phase makes our unit test pass or fail.
    // Here we check that the method's behavior is consistent with expectations.
    Assert.IsTrue(isPalindrome);
}
