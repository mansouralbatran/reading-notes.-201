# INTRODUCING HTML5 STORAGE

![image](https://i.ytimg.com/vi/M-Rp8u1AAHg/hqdefault.jpg)



What I will refer to as “HTML5 Storage” is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons. Certain browser vendors also refer to it as “Local Storage” or “DOM Storage.” The naming situation is made even more complicated by some related, similarly-named, emerging standards that I’ll discuss later in this chapter.
# USING HTML5 STORAGE
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.
### we do like that 
* var foo = localStorage.getItem("bar");
// ...
* localStorage.setItem("bar", foo);
* …could be rewritten to use square bracket syntax instead:

* var foo = localStorage["bar"];
// ...
* localStorage["bar"] = foo;
