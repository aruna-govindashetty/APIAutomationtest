# APIAutomationtest
API tests to create order and instruction
Solution contains:
1.Helper Folder- To generate hmac signature and bearer token
2.Request Folder- Helper methods for HttpClient and RestClient
3.Model Folder- Model of the Json payload
4.CreateOrderEndPoint Folder- Contains test methods to create order and instruction using HttpClient
Contains test methods to create order and instruction using RestClient

For running tests-
VSTest.Console.exe is the command-line tool to run tests. we can specify several options in any order on the command line.
More Information can be found here- https://docs.microsoft.com/en-us/visualstudio/test/vstest-console-options?view=vs-2019
For creating test report-
A test logger is a test platform extension to control reporting of test results. It can perform tasks when a test run message, individual test results or the test run completion events are reported by the test platform.
More Information can be found here- https://github.com/Microsoft/vstest-docs/blob/master/docs/report.md#1-console-logger

NugetPackages used-
MSTest 
Restsharp

Syntax to run the tests from the command prompt-
"path of vstest.console.exe" "project.dll" /Logger:html
Example:
"C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\Common7\IDE\Extensions\TestPlatform\vstest.console.exe" "C:\Users\Aruna\source\repos\Test\Test\bin\Debug\Test.dll" /Logger:html
Test results will be created in the folder shown in the command prompt after executing the tests. 

Note: I was not able to acess any Order API's through swagger even though I generated Hmac signature, I could not get bearer token and was getting Unauthorized error.
The tests will fail when run through command prompt because of the above issue.
I have written whatever I could without running or debugging the code.
