####psadvtechjsjq
#####intro
######1 see canvasv1 no param.
######2 see canvasv2 six param.
#######3-7 see respect html file

#####events
######propagation
events bubble up the dom until handled


#####using jQuery Deferred Obj
######common pattern
christmas tree effect, many indentation
######Deferred object
get use deferred, load does not.
######Negative testing.
using then(succ,fail) function, if fail multiple times, only return one error  
diff of cb and promise.
The done and fail methods are registering a handler function with the deferred object.
There is  nothing to prevent registering multiple handlers for the done and fail methods.(in fact if
we save the deferred object as a var, we can attach a handler even afer the object has been resolved or rejected.
A cb can only be called once from the original process that received it as a parameter.
Assuming we are making a call to jq get , if we pass a cb to that method,it will only get executed once the get method completes. 
There is no way to expand the func of the callback after is been executed because the get method has completed.

If we ue deferred object that isreturned from the get method instead,we can attach as many done or fail handlers as we wish in any order base on conditional processing.
We can even add a handler based on the result of the get.

######Deferred methods
defer4-promise.html observe the results

