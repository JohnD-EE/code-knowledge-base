# Conditional Rendering
`v-if` - takes the element in and out of the DOM
`v-show` - uses CSS `display:block` to remove the element from the DOM

Adding and moving things from the DOM takes more time and impacts performance.  So if the DOM will change regularly - like in a Nav bar, then consider `v-show` - but if it doesn't change much then consider `v-if`

