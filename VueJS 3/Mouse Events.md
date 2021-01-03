# Mouse Events
`@click`
`@mouseover`
`@mouseleave`
`@dblclick`
`@mousemove`

A mouse event gives us access to the event object which has loads of data - e.g.
- `altKey` was the alt key pressed with the mouse event?
- `ctrlKey` was ctrl pressed?
- `clientX` and `clientY` - cursor position
- `type` for the event type etc.

the first argument passed to the event handler method is the event object:
```
methods: {
	handleEvent(e) {
		console.log(e)
	}
}
```

We can also pass in a custom parameter:
`@mouseover=handleEvent($event, 87)`
Note that if we don't pass in the `$event` as the first argument, the event object will not be picked up by the handler


