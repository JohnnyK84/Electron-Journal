# Week 2
Talked about the importance of planning when developing apps and also covered some basic GUI practices and conventions that should be consiered during app development such as:

**Curly's Law: Do One Thing**

A variable should mean one thing, and one thing only. It should not mean one thing in one circumstance, and carry a different value from a different domain some other time. It should not mean two things at once. It must not be both a floor polish and a dessert topping. It should mean One Thing, and should mean it all of the time.

Ref: https://blog.codinghorror.com/curlys-law-do-one-thing/

### Some practices to thinkg about when planning your GUI:

1.  KISS. (Keep it simple stupid)
2.  Reduce the learning curve of a new user.
3.  Lead the expectations of the user and let your program behave according to those expectations.

**Emphasized the importance of planning**
Not only relating to wireframing but also when thinking of functionality

Also spent more time watching youtube tutorials on electron development

Went over the construction of the app made in the week 1 tutorial and explored some of the code used:

**package.json** - Completly made up of key-value pairs. Both parts are enclosed in a set of quotes **"key":"value"**

https://github.com/electron/electron-quick-start/blob/master/package.json to see a complete package.json version

**Main.js** - This file is where all the program logic happens, a number of .js files can be created as required, but *main.js* file is required because we reference it in our *package.json* file.

Note: Node (which electron is based on) follows the ES6 prescription of Javascrip, this is the current stable version of javasript.

### Using events in an application:

To trigger a javascrip function from HTML we need to use the **onclick** attribute. Say we have a function in our javascrip file called ShowMe(). We would call it from our HTML file as follows:

```<input type="button" value="Click me!" onclick="ShowMe()" >
```
```<script src="functions.js"></script>
```
As we have linked this to a functions.js file within our app this file would need to exist with the code required to execute the event:

```function ShowMe() {
    alert("I want to see a box :-)");
}
```

