### Conceptual Exercise

Answer the following questions below:

- What are important differences between Python and JavaScript?
  Javascript is making the front end or user experience side of a site work properly. It is making a
  website function.
  Python is more of how a website works behind the scenes, making a server for the website to exist on
  and it is more secure in that a user isn't able to access the code easily.

- Given a dictionary like `{"a": 1, "b": 2}`: , list two ways you
  can try to get a missing key (like "c") _without_ your programming
  crashing.

  1. values = {"a": 1, "b": 2}
     values.setdefault("c")
  2. values.get("c")

- What is a unit test?
  unit testing is when you test one component's functionality and seeing if it is working properly.
  It merely tests one function and not how it works in conjunction with other functions.

- What is an integration test?
  integration test tests how a function works with other functions along the "chain" but it doesn't
  test and see if the entire code is working together properly. It just tests a certain feature. It
  also tests and see if you have linked together different files and their functions together properly.

- What is the role of web application framework, like Flask?
  A web application framework is basically a tool based on a certain language that does work behind the
  scenes to make the development progress easier. It provides certain already made components that are
  customized to its own syntax.

- You can pass information to Flask either as a parameter in a route URL
  (like '/foods/pretzel') or using a URL query param (like
  'foods?type=pretzel'). How might you choose which one is a better fit
  for an application?
  Passing a parameter in requires the developer to make a few route directory for every single parameter
  the user is going to pass in whereas URL query is more dynamic where new queries can be generated according
  to need and not pre-hardcoded.

- How do you collect data from a URL placeholder parameter using Flask?
  you import "request" from flask and you call request.args["placeholder"]

- How do you collect data from the query string using Flask?
  you import "request" from flask and you call request.form.get("")

- How do you collect data from the body of the request using Flask?
  request.get_data(as_text=True if you want the return code to be decoded as a string, false if you are okay
  with return of bytes.)

- What is a cookie and what kinds of things are they commonly used for?
  A cookie is a small piece of data a web server stores while a user is browsing a website. It is a way for
  the website to remember certain information about the user such as username, password, preferences, etc.

- What is the session object in Flask?
  A session is almost like a cookie but it is more secure in that it stores data in an encrypted form. It is
  able to store larger sized data than a cookie. But like a cookie, it stores some type of information and sends
  it back and forth between the server and the browser each time you make a request.

- What does Flask's `jsonify()` do?
  jsonify changes data to Javascript Object Notation(JSON) format and wraps it in a response object.
