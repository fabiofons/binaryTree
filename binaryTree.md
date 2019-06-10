# BinaryTree in JS
## Methods add().
``` javascript

function BinaryTree() {
  this._root = null;
}

function TreeNode(val) {
  this.value = val;
  this.left = null;
  this.right = null;
}

BinaryTree.prototype.add = function(val, prevNode = this._root) {
  if (!this._root) {
    this._root = new TreeNode(val);
  } else if (val > prevNode.value) {
     if (!prevNode.right) {
       prevNode.right = new TreeNode(val);
     } else {
       this.add(val, prevNode.right);
     }
  } else {
    if (!prevNode.left) {
       prevNode.left = new TreeNode(val);
     } else {
       this.add(val, prevNode.left);
     }
  }
};
```

## Method traverseDFS
```javascript

function working on It

```

## Method traverseBFS
```javascript

function working on It

```
