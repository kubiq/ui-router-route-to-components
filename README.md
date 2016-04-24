# ui-router-route-to-component

Route to components today using Angular 1.5+ and ui-router 0.2.x+

# Usage

Add module dependency 'ui.router.components'

Example state config:

```javascript
.state('users', {
	parent		: 'header',
	url			: '/users/:id',
	component  : 'users',
})
```
Or
```javascript
.state('users', {
	parent		: 'header',
	url			: '/users/:id',
	views			: {
		'content@': {
			component  : 'users',
		}
	}
})
```
# Credits

Code mostly borrowed from https://github.com/angular-ui/ui-router/issues/2547 but extended to also support multiple named views.
