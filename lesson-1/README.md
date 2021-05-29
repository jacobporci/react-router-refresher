# Lesson 1 - Basic Routing

## XML-based Routing

```html
<Router>
  <Route path="/example1" component={Component}>
  <Route path="/example2">
    <Component />
  </Route>
</Router>
```

## Array-based Routing
```javascript
const routes = [
  {
    path: '/example1',
    component: Component1
  },
  {
    path: '/example2',
    component: Component2
  }
];

return (
  <Router>
    {routes.map(({ path, component}) => (
      <Route path={path} component={component} />
    ))}
  </Router>
)
```

## Exercise

### Create routing for page 1,2,3
1. Try both approaches on routing
2. Discuss w/ breakout group what are the benefits of each approach