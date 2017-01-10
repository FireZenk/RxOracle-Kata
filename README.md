# RxOracle-Kata
https://github.com/varokas/kata-rx/wiki/Kata-RX-Oracle

An introduction Kata for you to deal with another long running process.

An oracle object will give a word of wisdom when asked but will take 2-3 seconds to compute result (you can simulate this by adding a delay or thread sleep).

List of possible quotes returned by the Oracle are:
* Insanity: doing the same thing over and over again and expecting different results.
* A person who never made a mistake never tried anything new.
* Gravitation is not responsible for people falling in love.
* Look deep into nature, and then you will understand everything better.

Write a program that ask the oracle for word of the day. Also, when the oracle is asked and the client is waiting for the response. Print a line to indicate that the request has been made.

### Point of Interests
* Make sure that the client does not blocks while waiting for the call to Oracle.
* Watch out that the main thread may quit before your async call finishes.
* It might be easier to create an object to keep track of the events in the system.

### Expected Output

    Client: program started
    Client: getting word of the day from Oracle
    Client: Oracle contacted, waiting for response... 
    Client: Quote by Oracle: "...."

## Kata implementation

https://jsfiddle.net/1z80ezau/1/
