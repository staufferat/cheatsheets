# Map

## Map variants (bootstrap)

This in an example how you can map an array:

```react
[
  'primary',
  'secondary',
  'success',
  'danger',
  'warning',
  'info',
  'light',
  'dark',
].map((variant, idx) => (
  <Alert key={idx} variant={variant}>
    This is a {variant} alert—check it out!
  </Alert>
));
```

## Map from props

```react
{  this.props.value.map((projects) => (<div>{projects.name}</div>))}
```