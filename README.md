# toast.js
A simple toast/notification js library

It has support for 4 different sidebar colours.
Blue (no class)
Yellow (`warning`)
Red (`error`)
Purple (`special`)

You can easily create new colours by defining them in css with the following structure:

```css
.myColour::before{
  background:#fac
}
```
Then it's only a matter of using it

## Examples

```html
<style>
  .myColour::before{
    background:#C0C
  }
</style>

<script type="module" src="toast.mjs"></script>
<script>
  // the document field is optional and only really used for things like iframes or fragments
  toast("This is an example toast", 4000)
  toast("This is a warning toast", 4000, "warning")
  toast("This is an error toast", 4000, "error")
  toast("This is a special toast", 2000, "special")
  toast("This is a custom toast", 2000, "myColour")
</script>
```
