# yb-react-ui-tree

Forked from [react-ui-tree](https://github.com/pqx/react-ui-tree), has changes applied from [Sean's fork](https://github.com/mockeryjones/yb-ui-tree) for removal of drag and drop.
### Installation
``` sh
npm install yb-react-ui-tree --save
```

### Usage
``` javascript
<Tree
  paddingLeft={20}              // left padding for children nodes in pixels
  tree={this.state.tree}        // tree object
  onChange={this.handleChange}  // onChange(tree) tree object changed
  renderNode={this.renderNode}  // renderNode(node) return react element
/>

// a sample tree object
// node.children, node.collapsed, node.leaf properties are hardcoded
{
  "module": "react-ui-tree",
  "children": [{
    "collapsed": true,
    "module": "dist",
    "children": [{
      "module": "node.js"
    }]
  }]
}
```
check [app.js](https://github.com/pqx/react-ui-tree/blob/master/example/app.js) for a working example

### Development
- npm install
- npm start
- http://localhost:8080/example

### License
MIT
