$sessionId: This generates a unique value when the session starts and sent every time a mobile subscriber response has been received.
$serviceCode: This refer to your USSD code
$text: This shows the user input. which is an empty string in the first notification of a session which after that concatenates all the user input within the session until the session ends.
$response: This hold the answer to the user input.
echo: Prints out the response for the user to read.
CON: It means an intermediate menu Or that the session is CONtinuing
END: Means the final menu and will trigger session termination i.e session is ENDing.