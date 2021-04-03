## Authentication

**Explain what a “Singleton” is (in Computer Science terms)?**
singleton in software engineering, the singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system.

**Explain how the Singleton pattern can be used with Node modules, specifically with classes?**
- Singleton instance fields don’t take up space in the global namespace
- Singletons may be lazily initialized
- Singletons can implement interfaces
- Singletons can be passed as parameters
- Singletons can have their instances swapped out (such as for testing purposes)
- Singletons can be handled polymorphically, so there may exist multiple implementation
```
class PrivateSingleton {
    constructor() {
        this.message = 'I am an instance';
    }
}
class Singleton {
    constructor() {
        throw new Error('Use Singleton.getInstance()');
    }
    static getInstance() {
        if (!Singleton.instance) {
            Singleton.instance = new PrivateSingleton();
        }
        return Singleton.instance;
    }
}
module.exports = Singleton;
```
**If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?** 
- create function that has access to the request object 
- the response object 
- the next function in the application’s request-response cycle.
- The next function is a function in the Express router which
- when invoked, executes the middleware succeeding the current middleware.

## TERMS
- Router Middleware Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of ``express.Router()``.

- Dynamic Module Loading: This allows you to dynamically load modules only when they are needed, rather than having to load everything up front.
- singleton pattern: is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system.

- CRUD -> REST Method Matches :The HTTP verbs comprise a major portion of our “uniform interface” constraint and provide us the action counterpart to the noun-based resource. The primary or most-commonly-used HTTP verbs (or methods, as they are properly called) are POST, GET, PUT, PATCH, and DELETE. These correspond to create, read, update, and delete (or CRUD) operations, respectively. There are a number of other verbs, too, but are utilized less frequently. Of those less-frequent methods, OPTIONS and HEAD are used more often than others.


- Mock testing: is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. In mock testing, the dependencies are replaced with objects that simulate the behaviour of the real ones. The purpose of mocking is to isolate and focus on the code being tested and not on the behaviour or state of external dependencies.


### Securing Passwords with Bcrypt Hashing Function
- The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords.
- Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions
- Hash Collision attack: Hash functions have infinite input length and a predefined output length, so there is inevitably going to be the possibility of two different inputs that produce the same output hash. MD5, SHA1, SHA2 are vulnerable to Hash Collision Attack i.e. two input strings of a hash function that produce the same hash result.

### Basic access authentication

In the context of an HTTP transaction, basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic ``<credentials>``, where credentials is the Base64 encoding of ID and password joined by a single colon .

Authentication: is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.



### references
- https://medium.com/swlh/node-js-and-singleton-pattern-7b08d11c726a
- https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html
- https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html