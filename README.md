# vue-formio

A [Vue.js](http://vue.js/) component for rendering out forms based on the [Form.io](https://www.form.io) platform.

## Install

### npm

`Vue Formio` can be used on the server, or bundled for the client using an
npm-compatible packaging system such as [Browserify](http://browserify.org/) or
[webpack](http://webpack.github.io/).

```
npm install react-formio --save
```

## Props

### `src` : `string`

The form API source from [form.io](https://www.form.io) or your custom formio server.

See the [Creating a form](http://help.form.io/userguide/#new-form)
for where to set the API Path for your form.

You can also pass in the submission url as the `src` and the form will render with the data populated from the submission.

### `form` : `object`

An object representing the form. Use this instead of src for custom forms. 

**Note:** `src` will override this property if used.

### `submission`: `Object`

An object representing the default data for the form.

**Note:** `src` will override this if a submission url is entered.

### `options`: `object`

An object with the formio.js options that is passed through. See [Form.io Options](https://github.com/formio/formio.js/wiki/Form-Renderer#options).

## Events

All events triggered from the form are available via the v-on property. See [Form.io Events](https://github.com/formio/formio.js/wiki/Form-Renderer#events) for all the available events.

Then on the form set `<formio src="myform" v-on:submit="doSomething" />`

## License
Released under the [MIT License](http://www.opensource.org/licenses/MIT).