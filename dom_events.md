# Events
### [Back to Concepts](./README.md)

## Syntax :
```JavaScript
// How to register an event listener 
// Assuming myButton is a button element
myButton.addEventListener('click', greet, false)
function greet(event){
    // print and have a look at the event object 
    // always print arguments in case of overlooking any other arguments
    console.log('greet:', arguments)
    alert('hello world')
}
```
## Concepts :

#### Add Event Listener
The EventTarget method `addEventListener()` sets up a function that will be called whenever the specified event is delivered to the target. Common targets are Element, Document, and Window, but the target may be any object that supports events (such as XMLHttpRequest).

`addEventListener()` works by adding a function or an object that implements EventListener to the list of event listeners for the specified event type on the EventTarget on which it's called.

#### Event Handlers
The event listener can be specified as either a callback function or an object that implements EventListener, whose `handleEvent()` method serves as the callback function.

The callback function itself has the same parameters and return value as the `handleEvent()` method; that is, the callback accepts a single parameter: an object based on Event describing the event which has occurred, and it returns nothing.

#### This
It is often desirable to reference the element on which the event handler was fired, such as when using a generic handler for a set of similar elements.

If attaching a handler function to an element using addEventListener(), the value of `this` inside the handler is a reference to the element. It is the same as the value of the currentTarget property of the event argument that is passed to the handler.

#### Remove Event Listener
The `EventTarget.removeEventListener()` method removes from the EventTarget an event listener previously registered with `EventTarget.addEventListener()`. The event listener to be removed is identified using a combination of the event type, the event listener function itself, and various optional options that may affect the matching process

If an EventListener is removed from an EventTarget while it is processing an event, it will not be triggered by the current actions. An EventListener will not be invoked for the event it was registered for after being removed. However, it can be reattached.

Calling `removeEventListener()` with arguments that do not identify any currently registered EventListener on the EventTarget has no effect.

#### Class List
The `Element.classList` is a read-only property that returns a live DOMTokenList collection of the class attributes of the element. This can then be used to manipulate the class list.

Using classList is a convenient alternative to accessing an element's list of classes as a space-delimited string via element.className.

A DOMTokenList representing the contents of the element's class attribute. If the class attribute is not set or empty, it returns an empty DOMTokenList, i.e. a DOMTokenList with the length property equal to 0.

The DOMTokenList itself is read-only, although you can modify it using the add() and remove() methods.

## Common Mouse Events 

|Event Name	        |Fired When
|-------------------|---------------------------------------------------------------------------------------------------------
|auxclick	        |A pointing device button (ANY non-primary button) has been pressed and released on an element.
|click	            |A pointing device button (ANY button; soon to be primary button only) has been pressed and released on an element.
|contextmenu	    |The right button of the mouse is clicked (before the context menu is displayed).
|dblclick	        |A pointing device button is clicked twice on an element.
|mousedown	        |A pointing device button is pressed on an element.
|mouseenter	        |A pointing device is moved onto the element that has the listener attached.
|mouseleave	        |A pointing device is moved off the element that has the listener attached.
|mousemove	        |A pointing device is moved over an element. (Fired continously as the mouse moves.)
|mouseover	        |A pointing device is moved onto the element that has the listener attached or onto one of its children.
|mouseout	        |A pointing device is moved off the element that has the listener attached or off one of its children.
|mouseup	        |A pointing device button is released over an element.
|pointerlockchange	|The pointer was locked or released.
|pointerlockerror	|It was impossible to lock the pointer for technical reasons or because the permission was denied.
|select	            |Some text is being selected.
|wheel          	|A wheel button of a pointing device is rotated in any direction.

## Common Key Events
|Event Name	        |Fired When
|-------------------|-------------------------------------------------------------------------------------------
|keydown	        |ANY key is pressed
|keypress	        |ANY key except Shift, Fn, CapsLock is in pressed position. (Fired continously.)
|keyup	            |ANY key is released

## Common Progress Events
|Event Name	|Fired When
|-----------|----------------------------------------------------------------------------
|abort	    |Progression has been terminated (not due to an error).
|error      |Progression has failed.
|load	    |Progression has been successful.
|loadend	|Progress has stopped (after "error", "abort" or "load" have been dispatched).
|loadstart	|Progress has begun.
|progress	|In progress.
|timeout	|Progression is terminated due to preset time expiring.

## Refrence Links :
[DOM Events](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Events)

[Add Event Listener](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener)

[Event Types](https://developer.mozilla.org/en-US/docs/Web/Events)

[Remove Events Listener](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/removeEventListener)

[Class List](https://developer.mozilla.org/en-US/docs/Web/API/Element/classList)

## Assignments 


#### Lecture Gist :


#### Extra Practice :


#### Extra Practice Answers :


#### IC Assignment Link : 


#### IC Answers :


#### CW Assignment Link :


#### CW Answers :


## Classwork Review Video :

### [BACK TO TOP](#Events)