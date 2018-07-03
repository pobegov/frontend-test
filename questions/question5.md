# Question 5
Areas addressed: JAVASCRIPT, BUG FIXING, DOM MANIPULATION

## Loop

Function _appendChildren_ should add a new child div to each existing div. New divs should be decorated by calling _decorateDiv_.

For example, after _appendChildren_ is executed, the following divs:

```
<div id="a">
  <div id="b">
  </div>
</div>
```

should take the following form (assuming _decorateDiv_ does nothing):

```
<div id="a">
  <div id="b">
    <div></div>
  </div>
  <div></div>
</div>
```

The code below should do the job, but for some reason it goes into an infinite loop. Fix the bugs.

ECMAScript 6
```
function appendChildren(decorateDivFunction) {
  var allDivs = document.getElementsByTagName("div");

  for (var i = 0; i < allDivs.length; i++) {
    var newDiv = document.createElement("div");
    decorateDivFunction(newDiv);
    allDivs[i].appendChild(newDiv);
  }
}

// Example case. 
document.body.innerHTML = `
<div id="a">
  <div id="b">
  </div>
</div>`;

//appendChildren(function(div) {});
console.log(document.body.innerHTML);
```