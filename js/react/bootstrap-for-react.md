# Bootstrap for React

##Import
Import with npm
```
npm install react-bootstrap bootstrap
```
Add the stylesheet in index.js
```javascript
import 'bootstrap/dist/css/bootstrap.min.css';
```
CDN in to the index.html
```html
<link
  rel="stylesheet"
  href="https://maxcdn.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css"
  integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T"
  crossorigin="anonymous"
/>
```

## Components
All Components can be found at https://react-bootstrap.github.io/components/alerts

## Layout
Details can be found at https://react-bootstrap.github.io/layout/grid/

A short example:
```html
<Container>
  <Row className="justify-content-md-center">
    <Col xs lg="2">
      1 of 3
    </Col>
    <Col md="auto">Variable width content</Col>
    <Col xs lg="2">
      3 of 3
    </Col>
  </Row>
  <Row>
    <Col>1 of 3</Col>
    <Col md="auto">Variable width content</Col>
    <Col xs lg="2">
      3 of 3
    </Col>
  </Row>
</Container>
```
